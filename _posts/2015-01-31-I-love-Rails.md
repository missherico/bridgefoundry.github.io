---
layout: post
title: I love Rails
---

## I love Rails
![The Gamma-cygni SNR observed by Fermi. This image was created in pointlike and is from http://arxiv.org/abs/1207.0027.](/assets/gamma_cygni_pointlike-940x935.jpg)

During graduate school, I was involved with the development of pointlike, a package for fitting data observed by the [Fermi Gamma-ray space telescope](http://fermi.gsfc.nasa.gov).

## Design

Pointlike was designed from the ground up with flexibility in mind:

* high-level code written in python with an object-oriented design.
* Interface with underlying C++ libraries to handle [HEALPix](http://healpix.jpl.nasa.gov) and [fits files](http://fits.gsfc.nasa.gov). These libraries were wrapped with [SWIG](http://www.swig.org)
* Leverage as much as possible [numpy](http://www.numpy.org), [scipy](http://www.scipy.org), [matplotlib](http://matplotlib.org), and [pywcsgrid2](http://leejjoon.github.com/pywcsgrid2).
* python interface allows great flexibility and adaptability.

## Interface

The objects and functions described below have a variety of parameters that modify their behavior. The easist way to explore pointlike's features is interactivly in ipython using the [question mark functionality](http://ipython.org/ipython-doc/dev/interactive/tutorial.html#exploring-your-objects):

$ ipython
In [1]: roi.print_summary?
Type:             instancemethod
Base Class:       <type 'instancemethod'>
String Form:   File:             /nfs/farm/g/glast/u35/ReleaseManagerBuild/redhat5-x86_64-64...
Definition:       roi.print_summary(roi, sdir=None, galactic=False, maxdist=5...
Docstring:
    formatted table point sources positions and parameter in the ROI,
        followed by summary of diffuse names, parameters values.
        values are followed by a character to indicate status:
            blank: fixed
            ?      sigma=0, not fit yet
            !      relative error<0.1
            *      otherwise
    Parameters
    ----------
         sdir : SkyDir, optional, default None for center
               for center: default will be the first source
         galactic : bool, optional, default False
             set true for l,b
         maxdist : float, optional, default 5
             radius in degrees