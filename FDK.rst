.. AXITOM documentation master file, created by
   sphinx-quickstart on Tue Jun 25 21:12:55 2019.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

FDK
===




.. math::
   :nowrap:


    \begin{equation}
    f_{FDK}(x,y,z) = \int_0^{2\pi} \frac{R^2}{U(x,y,\beta)^2} \tilde{p}^F (\beta, a(x,y,\beta),b(x,y,z,\beta))d\beta
    \end{equation}

where 

.. math::
   :nowrap:

    \begin{equation}
    \tilde{p}^F(\beta,a,b) = (\frac{R}{\sqrt[]{R^2+a^2+b^2}} p (\beta,a,b)) * g^P(a)
    \end{equation}

.. math::
   :nowrap:

    \begin{equation}
    a(x,y,\beta) = R \frac{-x \sin \beta + y \cos \beta}{R + x \cos \beta + y \sin \beta}
    \end{equation}

.. math::
   :nowrap:

    \begin{equation}
    b(x,y,z\beta) = z \frac{R}{R+x\cos \beta + y \sin \beta}
    \end{equation}

.. math::
   :nowrap:

    \begin{equation}
    U(x,y,\beta) = R +x\cos \beta + y \sin \beta
    \end{equation}
    
calculating for $x=0$ gives:

.. math::
   :nowrap:

    \begin{equation}
    f_{FDK}(y,z) = \int_0^{2\pi} \frac{R^2}{U(y,\beta)^2} \tilde{p}^F (\beta, a(y,\beta),b(y,z,\beta))d\beta
    \end{equation}

where 

.. math::
   :nowrap:

    \begin{equation}
    a(y,\beta) = R \frac{ y \cos \beta}{R + y \sin \beta}
    \end{equation}

.. math::
   :nowrap:

    \begin{equation}
    b(y,z\beta) = z \frac{R}{R+ y \sin \beta}
    \end{equation}
    
    The values of $\tilde{p}^F (\beta, a(x,y,\beta),b(x,y,z,\beta)) $ are obtained by means of interpolation employing bi-cubic splines.



