# NuSTEAM23

install Singularity: [link](https://docs.sylabs.io/guides/3.0/user-guide/installation.html)


get scripts:
```
git clone https://github.com/HaiwangYu/nusteam23.git
```


get container:
```
cd nusteam23
singularity pull larwire-kokkos_2.2.sif docker://hepcce2/larwire-kokkos:2.2
```


run container:
```
./run-singularity.sh
```

run:
```
wire-cell -l stdout -L debug -c sim.jsonnet
```

inspect the root file:
Open the file with `root`
```
root -l protodune.root
```

Within the root interactive session:
```
.ls
hu_gauss0->Draw("colz")
hu_gauss0->Integral()
```
