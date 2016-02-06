# PhysConst
A collection of fundamental physical constants in various unit systems for MATLAB.

### Syntax:
`Constant.NameOfConstant` returns the value of the named constant in a predefined unit system. See the list of physical constant names below. For examples:
- `Constant.ElementaryCharge` returns the value of the elementary charge, *e*;
- `Constant.LightSpeed` returns the value of the speed of light, *c*.

By default, the values are returned in the [SI](https://en.wikipedia.org/wiki/International_System_of_Units) units. To 'pre-define' a different unit system, do one of the following:
- Make an assignment: `UnitSystem='UnitSystemCode';`, where `UnitSystemCode` refers to the unit system to be used. See the list of unit system codes below.
- Define an anonymous function: `UnitSystem=@()'UnitSystemCode';`.
- Create a function named `UnitSystem` in the current working directory or elsewhere. The function takes no input arguments and return a string specifying the unit system code.

`Constant.UnitSystemCode.NameOfConstant` returns the value of the named constant in the specified unit system, regardless of the predefined unit system. For examples:
- `Constant.SI.ElementaryCharge` returns the value of the elementary charge, *e*, in the SI units (=1.602176565);
- `Constant.P.LightSpeed` returns the value of the speed of light, *c*, in the Planck units (=1).

### List of Unit System Codes
- `HA`: Hartree Atomic Units
- `P`: Planck Units
- `QCD`: Quantum Chromodynamics Units
- `RA`: Rydberg Atomic Units
- `S`: Stoney Units
- `SI`: International System of Units

### List of Physical Constant Names
- `AtomicMass`: atomic mass unit, *m*<sub>u</sub>
- `AvogadroNumber`: Avogadro's number, *N*<sub>A</sub>
- `BohrMagneton`: Bohr magneton, *μ*<sub>B</sub>
- `BohrRadius`: Bohr radius, *a*<sub>0</sub>
- `Boltzmann`: Boltzmann constant, *k*<sub>B</sub>
- `ConductanceQuantum`: conductance quantum, *G*<sub>0</sub>
- `Coulomb`: Coulomb constant, *k*<sub>e</sub>
- `ElectronMass`: electron mass, *m*<sub>e</sub>
- `ElementaryCharge`: elementary charge, *e*
- `Faraday`: Faraday constant, *F*
- `FermiCoupling`: Fermi coupling constant, *G*<sub>F</sub>/(*ħc*)<sup>3</sup>
- `FineStructure`: fine-structure constant, *α*
- `FluxQuantum`: magnetic flux quantum, Φ<sub>0</sub>
- `Gravitational`: Newtonian constant of gravitation, *G*
- `HartreeEnergy`: Hartree energy, *E*<sub>h</sub>
- `LightSpeed`: speed of light, *c*
- `Loschmidt`: Loschmidt's number, *n*<sub>0</sub>
- `NuclearMagneton`: nuclear magneton, *μ*<sub>N</sub>
- `Planck`: Planck constant, *h*
- `ProtonMass`: proton mass, *m*<sub>p</sub>
- `ReducedPlanck`: reduced Planck constant, *ħ*
- `Rydberg`: Rydberg constant, *R*<sub>∞</sub>
- `StefanBoltzmann`: Steffan-Boltzmann constant, *σ*
- `VacuumImpedeance`: vacuum impedance, *Z*<sub>0</sub>
- `VacuumPermeability`: vacuum permeability, *μ*<sub>0</sub>
- `VacuumPermittivity`: vacuum permittivity, *ε*<sub>0</sub>
- `WienDisplacement`: Wien displacement law constant, *b*
