# Robust focal length estimation

This is my Bachelors thesis at CTU in Prague under the supervision of Tomas Pajdla. I worked on testing the existing and  developing new algorithms for more robust focal length estimation. The result of the work was a procedure that was more robust than the direct existing method. The method was curiously also applicable to estimation of focal lengths even when the other camera parameters such as the principal point position were misspecified. This could open up the possibility of creating stable SfM reconstructions even from very challenging currently data, such as data from the internet that are missing camera specifications, are noisy or have undergone significant postprocessing.  

## Structure

- The code is in another repo: https://github.com/orybkin/AlFocal
- The thesis pdf: https://github.com/orybkin/Bachelor-Thesis/blob/master/Robust_Focal_Length_Computation.pdf
- The slides pdf: https://github.com/orybkin/Bachelor-Thesis/blob/master/Bachelor_presentation%20no%20notes.pdf

## Abstract

The problem of automatically computing focal lengths of a pair of cameras from corresponding
pair of images has long been a daunting task for 3D reconstruction community.
A number of methods were developed, but the commonly held view is that neither of
them works good enough to be used in practical situations. We focus on the particular
task of computing focal lengths from the point correspondences, which we deem to be
the missing link for the problem solution.

We especially focus on existing algebraic solvers for computing the fundamental matrix
and the Bougnoux formula for computing the focal lengths therefrom. We survey
these methods, as well as iterative methods [10, 4] proposed as their extensions, and
analyze their performance. Our results show that the number of imaginary estimates,
as well as the error of the estimation, declines with growing number of correspondences
used. Moreover, based on our analysis we suggest that the computation of the ratio of
focal length r = f2/f1 is more robust than computation of f1 or f2 alone. We propose
an improvement to the solver of [10] based on this suggestion.

We furthermore assess performance of the methods in degenerate situations, and
show that for bigger levels of noise the effect of the degeneracies signicantly decreases.
Specifically, the degenerate case of intersecting optical axes is shown to almost vanish
for realistic levels of noise.

We finally analyze the problem of computing focal length from the theoretical standpoint
of algebraic geometry, and give two new formulae for computing camera focal
length from a fundamental matrix. We show that using the right of them might help
to avoid a known degeneracy. Specifically, the degeneracy where the plane defined by
the baseline and the optical axis of one camera is perpendicular to the plane defined by
the baseline and optical axis of the other camera, and where Bougnoux ([3]) formula
fails can in some cases be avoided. The degeneracy reduces to the case where all three
formulae fail.

## Wordle

![alt text](https://github.com/orybkin/Bachelor-Thesis/blob/master/bach.png "Wordle")

## BibTex

```
@mastersthesis{rybkin2017robustni,
  title={Robust focal length computation},
  author={Rybkin, Oleh},
  type={{B.S.} thesis},
  year={2017},
  school={Czech Technical University in Prague}
}
```
