# Robust focal length estimation

This is my Bachelors thesis at CTU in Prague under the supervision of Tomas Pajdla. I worked on testing the existing and  developing new algorithms for more robust focal length estimation. The result of the work was a procedure that was more robust than the direct existing method. The method was curiously also applicable to estimation of focal lengths even when the other camera parameters such as the principal point position were misspecified. This could open up the possibility of creating stable SfM reconstructions even from very challenging currently data, such as data from the internet that are missing camera specifications, are noisy or have undergone significant postprocessing.  

## Structure

- The code is in another repo: https://github.com/orybkin/AlFocal
- The thesis pdf: https://github.com/orybkin/Bachelor-Thesis/blob/master/Robust_Focal_Length_Computation.pdf
- The slides pdf: https://github.com/orybkin/Bachelor-Thesis/blob/master/Bachelor_presentation%20no%20notes.pdf

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
