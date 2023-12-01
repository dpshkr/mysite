Energy Levels in 2D Semiconductors
===================================

2D materials are atomically thin sheets.
As a result, the electrons in a 2D material are confined in one direction while free in the other two directions.
Without loss of generality, we can assume that the electron is confined in the $z$ direction and free in the $x-y$ plane.
We will also assume that the sheet is $L$. $L$ typically has atomic length scales.

The Schrodinger equation for electrons in such a system is

 $$-\frac{\hbar^2}{2m} \nabla^2 \Psi + V(z)\Psi = E\Psi$$

The electron  potential depends only on $z$ due to its confinement.
The $V(z)$ is an infinite potential well, shown in the figure below.

.. image:: _static/infinite-potential-well.png
    :width: 300

The above problem can be easily solved by separating the variables.
We can write the wavefunction $\Psi$ of the electron as $\Psi = \Psi_{xy} \Psi_z$,
where $\Psi_{xy}$ depends only on $x$ and $y$, while $\Psi_z$ depends only on $z$.
Similarly, the total energy of the electron can be represented as $E = E_{xy} + E_z$.
We will not do the (fairly simple) mathematics to derive the results.
Rather, we will give the results and justify them physically.

The electron is free in the $x-y$ plane.
It should, therefore, have a free electron wavefunction.
$\Psi_{xy} \propto e^{i(k_xx + k_yy)}$. Here $k_x$ and $k_y$ can take any real values.
The energy component of the electron along the $x-y$ plane can then be written as

$$E_{xy} = \frac{\hbar^2}{2m} (k_x^2 + k_y^2)$$

Since $k_x$ and $k_y$ can take any real value, the energy component $E_{xy}$ can take continuous values $E_{xy} \ge 0$.

Along the $z$ direction, the electron is trapped in an infinite potential well.
From elementary quantum mechanics, we know that the wavefunction of such an electron is $\Psi_z \propto \sin\big(\frac{n\pi z}{L}\big)$.
Here $n$ is only allowed to be a positive integer ($n = 1,2,3 \dots$).
The energy component in this direction also has an exact form of electron's energy in an infinite potential well.

$$E_z = \frac{n^2\pi^2\hbar^2}{2mL^2},\ n=1,2,3\dots$$

Combining both expressions, we now get the expression for the total energy of the electron in a confined 2D sheet.

$$E = \frac{\hbar^2}{2m} (k_x^2 + k_y^2) +  \frac{n^2\pi^2\hbar^2}{2mL^2},\ n=1,2,3\dots$$

1. The energy of an electron in a 2D system is *continuous*. $E$ can take any value greater than $\frac{\pi^2\hbar^2}{2mL^2}$.  In a potential well, the total energy is *quantized*. However, here, only a part of the energy is quantized.
2. Every electronic state in the system can be uniquely described by four numbers - $n$, $k_x$, $k_y$ and spin $s$. $n$ can take only positive integer values, while $k_x$ and $k_y$ can take continuous real values. Spin $s$ can take two values $+\frac{1}{2}$ and $-\frac{1}{2}$.
3. We know from Pauli's exclusion principle that two electrons (being Fermions) cannot have identical quantum states. Therefore, no two electrons in the system can have an identical set of the four quantum numbers.
4. Often, it is convenient to define $n$ as the *principal* quantum number. All the energy states that have a given principal quantum number are said to belong to $n^{th}$ subband. For example, all the electrons having $n=2$ are said to be in the second subband.


.. image:: _static/allowed-energy-levels.png
    :width: 300

The above diagram schematically represents the energy levels of the system.
The discrete energy levels of $E_z$ are marked $E_z^1$, $E_z^2$ and $E_z^3$
which correspond to $n=1$, $n=2$ and $n=3$ respectively.
Some arbitrary energy levels $E_1$, $E_2$ and $E_3$ are also shown.

1. No electron state can have energy level $E_1$ as it is below the first quantum level of $E_z$. Such a case would lead to a negative $E_{xy}$ which is physically not possible.
2. The energy level $E_2$ is allowed for a quantum state. Such a state can have only one possible principal quantum number $n=1$. However, this state can have infinitely many possible $k_x$ and $k_y$. All the real $k_x$ and $k_y$ which satisfy the equation $\frac{\hbar^2}{2m} (k_x^2 + k_y^2) = E_1 - E_z^1$ are allowed.
3. A state with energy level $E_3$ can have two principal quantum numbers, $n=1$ and $n=2$ as shown in the figure. Again, for each state, infinitely many $k_x$ and $k_y$ are allowed.

If we extrapolate this trend, it is easy to see that energy levels between $E_z^3$ and $E_z^4$
can have three possible principle quantum numbers $n=1$, $n=2$ and $n=3$.
This subtle point, though trivial, is not usually mentioned explicitly in most works on 2D materials.
