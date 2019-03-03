![CMExtended.jpg](/Images/CMExtended.jpg)                                                                                                                

# [Download Adinkra.m](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/Adinkra.m)

## Download Instructions 

Click on the download link above. Save to your local hard drive and follow the install instructions below.

Right (command) click on [Adinkra.m](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/Adinkra.m) and the examples in the Examples directory to save to your local hard drive. You may have to delete a .txt extension from AdinkraTutorial.nb.after download.

## Alternative Download Instructions 

Click on [Adinkra.m](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/Adinkra.m) and the examples in the Examples directory, and copy the raw text into a Mathematica file to save to your local hard drive.

# Files Associated with the Adinkra repository



* [Adinkra.m](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/Adinkra.m): mathematica package with tools to research adinkras

* [AdinkraTutorial.nb](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/AdinkraTutorial.nb): full tutorial notebook file with examples on how to use the various functions of the Adinkra.m package.

* [4DTools.nb](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/Examples/4DTools.nb): tutorial notebook file with just the examples of 4D tools of the full tutorial AdinkraTutorial.nb.

* [N!=4.nb](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/Examples/N!=4.nb): tutorial notebook file with just the examples of N != 4 adinkras of the full tutorial AdinkraTutorial.nb.

* [N=4.nb](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/Examples/N=4.nb): tutorial notebook file with just the examples of N = 4 adinkras of the full tutorial AdinkraTutorial.nb.




The tutorials show in depth how to use many of the tools of the Adinkra.m package listed below on this page. 






## Installation Instructions
After downloading, install the Adinkra.m package on your local machine with the File-->Install menu in Mathematica

![FileInstall.jpg](/Images/FileInstall.jpg)

In the "Source" dropdown menu, select "From File..."

![UpdateFromFile.png](/Images/UpdateFromFile.png)

Navigate to where you downloaded "Adinkra.m" on you local machine, select it and click "ok". Import the package into a notebook as follows:

![UpdateImportAdinkra.png](/Images/UpdateImportAdinkra.png)

 **If updated from an old version of Adinkra.m, you may have to delete the old package first. Run [DeleteAdinkra.nb](https://raw.githubusercontent.com/HEPTHools/Adinkra/master/DeleteAdinkra.nb) to delete an existing Adinkra package** 
 
 The date of the latest build, in yymmdd format, can be called by running, for example

![BuildDate.jpg](/Images/BuildDate.jpg)

# About the Adinkra.m package

The Adinkra.m package includes tools to

```markdown

1. Build 4D, N=1 SUSY transfromation laws in Majorana components
2. Reduce to 1D (0-brane reduction), generating L- and R-matrices for arbitrary d
3. Graph L- and R- adinkra matrices as an adinkra for GR(4,4) matrices
4. Allows the user to encode their own arbitrary GR(d,N) L- and R- adinkra matrices and check that the GR(d,N) algebra is satisfied
4. Calculate chi_0 and holoraumy of adinkra matrices for arbitrary GR(d,N)
5. Print out L, R, holoraumy matrices and closure relationship in an l(d/4) \times l(4) tensor product basis in symbolic form ready to be LaTexed by Mathematica's TeXForm command

```



The list of functions can be found by running 

FunctionList[Adinkra] 

which outputs the following:

```markdown

SpaceTime:
IndexRange[SpaceTime][Index], Index = mu, a, or RaiseCode

coordinates, \[CapitalStigma][mu], \[Eta][mu,nu], Cmetric[[a,b]], 
InverseCmetric[[a,b]], UD[Field,\[CapitalStigma][mu]] , Lap[Field], 
UP, DOWN, RaiseSTIndex[Field,RaiseCode1,RaiseCode2,...,RaiseCoden], 
RaiseFermionIndex[Field]

****************************************************************************************
****************************************************************************************

GenerateLandR:
NColors[D,Phi,Psi], LTable[DColor,Phi,Psi], 
RTable[DColor,Phi,Psi],GenerateLandR[DColor,Phi,Psi,Rep]

****************************************************************************************
****************************************************************************************

AdinkraEssentials:
IndexRange[AdinkraEssentials][Index], Index = p1, II, ReportLevel, or 
pm

***IMPORTANT****: Default Settings are VScaleFactor = 
VtildeScaleFactor = -I, VsoNScaleFactor = -I/(2 VsoNScaleFactor), 
VtildesoNScaleFactor = -I/(2 VtildesoNScaleFactor)

Reports: AdinkraReport[Rep,ReportLevel], 
AdinkraPreliminaryReport[L,R], AdinkraPreliminaryReport[Rep], 
AdinkraPreliminaryReportO[Rep], AdinkraHoloMonoReport[Rep], 
AdinkraSummaryReport[Rep], AdinkraFullReport[Rep]

Basic Functions: nMatrices[Matrices], nRows[Matrices], 
nColumns[Matrices], Commute[Matrix1,Matrix2], NColors[Rep], 
NColors[L,R], dmin[N], dbosons[Rep], dbosons[L,R], dfermions[Rep], 
dfermions[L,R], WordW[{p1,p2,...,pN}]

Intense Calculations: Gadget[Rep1,Rep2], BosonGadget[Rep1,Rep2], 
ListOfIdenticalMonoOrHolo[MonoOrHolo,Rep], 
NumDistinctHoloOrMono[HoloOrMono,Rep]

Print Functions: PrintL[Rep][II], PrintR[Rep][II], 
PrintGALR[Rep][II,JJ], PrintGARL[Rep][II,JJ], PrintV[Rep][II,JJ], 
PrintVtilde[Rep][II,JJ], PrintZetaGen[Rep][II], 
PrintHoloraumy[Rep][{p1,p2,...,pN}], 
PrintMonodromy[Rep][{p1,p2,...,pN}],PrintZetatildeGen[Rep][II], 
PrintHoloraumytilde[Rep][{p1,p2,...,pN}], 
PrintMonodromytilde[Rep][{p1,p2,...,pN}], 
PrintVtildePM[pm][Rep][II,JJ], PrintVtildePM[pm][Rep][II,JJ], 
PrintAllL[Rep], PrintAllR[Rep], PrintAllGALR[Rep], PrintAllGARL[Rep], 
PrintAllV[Rep], PrintAllVtilde[Rep], PrintAllZetaGen[Rep], 
PrintAllHoloraumy[Rep], 
PrintAllMonodromy[Rep],PrintAllZetatildeGen[Rep], 
PrintAllHoloraumytilde[Rep], PrintAllMonodromytilde[Rep], 
PrintAllVtildePM[pm][Rep], PrintAllVtildePM[pm][Rep], 
,PrintSigmaProduct[Matrix], PrintLSigmaProduct[Rep], 
PrintRSigmaProduct[Rep]

Test Functions: CorrectDimensions[Rep], CorrectDimensions[L,R], 
TransposeTest[Rep], TransposeTest[L,R], InverseTest[Rep], 
InverseTest[L,R], RO[Rep], Chi0Report[L,R], GATest[Rep], GATest[L,R], 
soNTest[Matrices], su2Test[MgenPM[pm]][Rep], 
MutuallyCommuteTest[M1,M2], LinearlyIndependent[Mgen]

Data generated by GenerateAdinkraData[Rep], 
GenerateAdinkraData[Rep,Orthogonal], GenerateAdinkraDataO[Rep], 
GenerateAdinkraData[Rep,L], or GenerateAdinkraData[Rep,L,R]:
L[Rep], R[Rep], GALR[Rep], GARL[Rep], chi0[Rep], ncis[Rep], 
ntrans[Rep], V[Rep], Vtilde[Rep], VsoN[Rep], VtildesoN[Rep], 
ZetaGen[Rep], Holoraumy[Rep], Monodromy[Rep], ZetatildeGen[Rep], 
Holoraumytilde[Rep], Monodromytilde[Rep], VPM[pm][Rep], 
VtildePM[pm][Rep], VsoNPM[pm][Rep], VtildesoNPM[pm][Rep] 
cSoln[V[Rep]], cSoln[Vtilde[Rep]]

****************************************************************************************
****************************************************************************************

BasisDecomposition:
IndexRange[BasisDecomposition][Index], Index = mu, ahat, a, d, or n

General Matrix Tools:
sigma[mu], \[Alpha]matrix[ahat], \[Beta]matrix[ahat], 
SigmaProduct[mu1,mu2,...,mun], SigmaProductMF[mu1,mu2,...,mun], 
SigmaMatrixProduct[mu,AnyMatrix], \[Rho]matrix[mu,nu], 
\[Omega]matrix[n][a], Basis[d][a,mu,nu], TestOrthogonal\[Sigma], Test
\[Rho]Orthogonal, Test\[Omega]Orthogonal[n], TestBasisOrthogonal[d], 
Coeffs[d][Matrix][a,mu,nu]

GenerateCoeffs[Rep] generates adinkra representation specific 
functions:
LCoeffs[Rep][II], CheckLCoeffs[Rep], RCoeffs[Rep][II], 
CheckRCoeffs[Rep], VCoeffs[Rep][II,JJ], CheckVCoeffs[Rep], 
VtildeCoeffs[Rep][II,JJ], CheckVtildeCoeffs[Rep], 
VPMCoeffs[pm][Rep][II,JJ], CheckVPMCoeffs[pm][Rep], 
VtildePMCoeffs[pm][Rep][II,JJ], CheckVtildePMCoeffs[pm][Rep], 
NumberNonZero[LCoeffsMat], CoeffsSummaryReport[Rep], 
CoeffsFullReport[Rep_]

Print Functions:
 PrintSigmaProduct[Matrix], PrintBasis[Matrix], PrintLBasis[Rep][II], 
PrintRBasis[Rep][II], PrintGALRBasis[Rep][II,JJ], 
PrintGARLBasis[Rep][II,JJ], PrintVBasis[Rep][II,JJ], 
PrintVtildeBasis[Rep][II,JJ], PrintVPMBasis[pm][Rep][II,JJ], 
PrintVtildePMBasis[pm][Rep][II,JJ], PrintLSigmaProduct[Rep], 
PrintRSigmaProduct[Rep]

****************************************************************************************
****************************************************************************************

BC4Tools:

IndexRange[BC4Tools][Index], Index = n, a, [Mu], A, II, or tt

Functions: 
HPerm[a], H[[a]], S3Perm[\[Mu]], S3[[\[Mu]]], VierPerm[A], Vier[[A]], 
BC4[[n,a,\[Mu],A,II,JJ]] , BC4Perm[n,a,\[Mu],A][[II,JJ]], 
QuaternionTestIJK[Quat], QuaternionTestKJI[Quat], Digit[Num,Pow], 
ell[Rep][tt,a][II,JJ], kappa[Rep][ti,a][II,JJ], 
IellABColor[Rep][[a]], PrintIell[Rep][[a]], IellABCode[Rep][[a]], 
AntisymmetryCheck[Object1], BC4Color[n,a,\[Mu],A][L], 
BC4ColorPerm[n,a,\[Mu],A][L],BC4Boson[n,a,\[Mu],A][L],BC4BosonPerm[n,
a,\[Mu],A][L], 
HList,S3List,VierList,PrintBC4Perm[n,a,\[Mu],A],PrintBC4BosonPerm[n,a,
\[Mu],A],PrintBC4FermionPerm[n,a,\[Mu],A],PrintBC4ColorPerm[n,a,\[Mu],
A],L[Q],L[Qtilde],L[RepCode]

****************************************************************************************
****************************************************************************************

GraphingTools:
IndexRange[GraphingTools][list]

 AdinkraGreen, AdinkraViolet, AdinkraOrange, AdinkraRed, 
padLmatrix[L], adjacencyToEdge[mat,col], buildrules[list], Valise, 
GraphAdinkra[L], GraphAdinkra[L,BuildRules[list], 
ExportAdinkra[L,BuildRules[list],filename]

****************************************************************************************
****************************************************************************************


```

In the above list, the functions are organized in terms of the notebooks with which they are created. The FunctionList for each sub-notebook may be called independently. If for instance just a list of GraphingTools is desired, run

FunctionList[GraphingTools]


