# STL10-Labeled 

Please consider sponsoring this repo so that we can continue to develop high-quality datasets for the ML/AI research.

To become a sponsor:

[GitHub Sponsors](https://github.com/sponsors/semihyagli) <br/>
[Buy me a coffee](https://buymeacoffee.com/semihyagli) <br/>

You can also sponsor us by downloading our free application, **_Etiqueta_**, to your devices:

[Etiqueta on iOS or Apple Chip Macs](https://apps.apple.com/us/app/etiqueta/id6504646776) <br/>
[Etiqueta on Android](https://play.google.com/store/apps/details?id=com.aidatalabel.etiqueta) <br/>


This public repo contains labels for the unlabeled pictures in the stl10 dataset. <br/>
More information on the original STL-10 dataset can be found here: https://cs.stanford.edu/~acoates/stl10/ <br/>
Thanks to Martin Tutek, the original STL-10 dataset can be downloaded via the python code here: https://github.com/mttk/STL10

If you use this dataset in your research please do not forget to cite: <br/>

```
@techreport{yagli2025etiqueta,
  author      = {Semih Yagli},
  title       = {Etiqueta: AI-Aided, Gamified Data Labeling to Label and Segment Data},
  year        = {2025},
  number      = {TR-2025-0001},
  address     = {NJ, USA},
  month       = Apr.,
  url         = {https://www.aidatalabel.com/technical_reports/aidatalabel_tr_2025_0001.pdf},
  institution = {AI Data Label},
}
```
```
@inproceedings{coates2011analysis,
  title     = {An analysis of single-layer networks in unsupervised feature learning},
  author    = {Coates, Adam and Ng, Andrew and Lee, Honglak},
  booktitle = {Proceedings of the fourteenth international conference on artificial intelligence and statistics},
  pages     = {215--223},
  year      = {2011},
  organization={JMLR Workshop and Conference Proceedings}
}
```

Note: If you notice any errors and/or if you have comments/ideas relevant to this dataset or Etiqueta in general, please reach me out at [contact@aidatalabel.com](mailto:contact@aidatalabel.com).

## Instructions 
To download the dataset, run:
```
python stl10
```
1. This will create a folder named `data` download and extract the stl10 dataset inside that folder. 
2. Then it will show one example picture in a new window.
3. Once you close this example picture, images will then be saved to disk under a folder called `img`

If you just want to load images as `numpy.array`:
```
import stl10
images = read_all_images(DATA_PATH_TO_BINARY_FILE)
```
where by default `DATA_PATH_TO_BINARY_FILE` can be either of the following: <br/>
* `./data/stl10_binary/test_X.bin`
* `./data/stl10_binary/train_X.bin`
* `./data/stl10_binary/unlabeled_X.bin`

This repo specifically contains the labels for the images inside `unlabeled_X.bin`


## Examples

Class |  ai0 - passenger plane |  ai1 - small plane |  ai2 - sea plane |  ai3 - military plane |  ai4 - toy plane |  ai5 - helicopter |  
--- | --- | --- | --- | --- | --- | --- | 
airplane | ![ai0 - passenger plane](examples/airplane/ai0-passenger%20plane.png) | ![ai1 - small plane](examples/airplane/ai1-small%20plane.png) | ![ai2 - sea plane](examples/airplane/ai2-sea%20plane.png) | ![ai3 - military plane](examples/airplane/ai3-military%20plane.png) | ![ai4 - toy plane](examples/airplane/ai4-toy%20plane.png) | ![ai5 - helicopter](examples/airplane/ai5-helicopter.png) |

Class | ai6 - hot air balloon | ai7 - zeppelin | ai8 - spaceship | ai9 - other balloon | ai10 - kite | 
--- | --- | --- | --- | --- | --- | 
airplane |  ![ai6 - balloon](examples/airplane/ai6-balloon.png) | ![ai7 - zeppelin](examples/airplane/ai7-zeppelin.png) | ![ai8 - spaceship](examples/airplane/ai8-spaceship.png) |![ai9 - other balloon](examples/airplane/ai9-otherballoon.png) |![ai10 - kite](examples/airplane/ai10-kite.png) |

Class | an0 - antelope | an1 - wildebeest | an2 - oryx | an3 - dikdik | an4 - eland | an5 - kudu | 
--- | --- | --- | --- | --- | --- | --- | 
antelope | ![an0 - antelope](examples/antelope/an0-antelope.png) | ![an1 - wildebeest](examples/antelope/an1-wildebeest.png) | ![an2 - oryx](examples/antelope/an2-oryx.png) | ![an3 - dikdik](examples/antelope/an3-dikdik.png) | ![an4 - eland](examples/antelope/an4-eland.png) | ![an5 - kudu](examples/antelope/an5-kudu.png) | 

Class | an6 - gerenuk | an7 - springbok | an8 - hartebeest | an9 - waterbuck | an10 - blackbuck | an11 - gazelle | 
--- | --- | --- | --- | --- | --- | --- | 
antelope | ![an6 - gerenuk](examples/antelope/an6-gerenuk.png) | ![an7 - springbok](examples/antelope/an7-springbok.png) | ![an8 - hartebeest](examples/antelope/an8-hartebeest.png) | ![an9 - waterbuck](examples/antelope/an9-waterbuck.png) | ![an10 - blackbuck](examples/antelope/an10-blackbuck.png) | ![an11 - gazelle](examples/antelope/an11-gazelle.png) | 

Class | an12 - impala | an13 - saiga | an14 - addax | an15 - kob | an16 - topi | 
--- | --- | --- | --- | --- | --- |
antelope | ![an12 - impala](examples/antelope/an12-impala.png) | ![an13 - saiga](examples/antelope/an13-saiga.png) | ![an14 - addax](examples/antelope/an14-addax.png) | ![an15 - kob](examples/antelope/an15-kob.png) | ![an16 - topi](examples/antelope/an16-topi.png) | 

Class | be0 - black bear | be1 - brown bear | be2 - polar bear | be3 - panda bear | be4 - red panda | 
--- | --- | --- | --- | --- | --- | 
bear | ![be0 - black bear](examples/bear/be0-black_bear.png) | ![be1 - brown bear](examples/bear/be1-brown_bear.png) | ![be2 - polar bear](examples/bear/be2-polar_bear.png) | ![be3 - panda bear](examples/bear/be3-panda_bear.png) | ![be4 - red panda](examples/bear/be4-red_panda.png) | 

Class | bi0 - bird | bi1 - chicken | bi2 - duck | 
--- | --- | --- | --- | 
bird | ![bi0 - bird](examples/bird/bi0-bird.png) | ![bi1 - chicken](examples/bird/bi1-chicken.png) | ![bi2 - duck](examples/bird/bi2-duck.png) | 

Class | cam0 - camel | cam1 - lama/alpaca | 
--- | --- | --- | 
camelid | ![cam0 - camel](examples/camelid/cam0-camel.png) | ![cam1 - lama/alpaca](examples/camelid/cam1-lama.png) | 

Class | ca0 - dog | ca1 - fox | ca2 - wolf | ca3 - coyote | ca4 - jackal | ca5 - maned wolf | ca6 - dog sled
--- | --- | --- | --- | --- | --- | --- | --- |
canine | ![ca0 - dog](examples/canine/ca0-dog.png) | ![ca1 - fox](examples/canine/ca1-fox.png) | ![ca2 - wolf](examples/canine/ca2-wolf.png) | ![ca3 - coyote](examples/canine/ca3-coyote.png) | ![ca4 - jackal](examples/canine/ca4-jackal.png) | ![ca5 - maned wolf](examples/canine/ca5-maned%20wolf.png) | ![ca6 - dog sled](examples/canine/ca6-dog%20sled.png)

Class | car0 - horse carriage | car1 - cattle carriage | car2 - human carriage | car3 - donkey carriage | car4 - goat carriage | car5 - other carriage | 
--- | --- | --- | --- | --- | --- | --- | 
carriage | ![car0 - horse carriage](examples/carriage/car0-horse_carriage.png) | ![car1 - cattle carriage](examples/carriage/car1-cattle_carriage.png) | ![car2 - human carriage](examples/carriage/car2-human_carriage.png) | ![car3 - donkey carriage](examples/carriage/car3-donkey_carriage.png) | ![car4 - goat carriage](examples/carriage/car4-goat_carriage.png) | ![car5 - other carriage](examples/carriage/car5-other_carriage.png) | 

Class | cy0 - motorcycle | cy1 - monocycle | cy2 - bicycle | cy3 - tricycle | cy4 - snowmobile | cy5 - skateboard | cy6 - scooter | 
--- | --- | --- | --- | --- | --- | --- | --- | 
cycle | ![cy0 - motorcycle](examples/cycle/cy0-motorcycle.png) | ![cy1 - monocycle](examples/cycle/cy1-monocycle.png) | ![cy2 - bicycle](examples/cycle/cy2-bicycle.png) | ![cy3 - tricycle](examples/cycle/cy3-tricycle.png) | ![cy4 - snowmobile](examples/cycle/cy4-snowmobile.png) | ![cy5 - skateboard](examples/cycle/cy5-skateboard.png) | ![cy6 - scooter](examples/cycle/cy6-scooter.png) | 

Class | eq0 - horse | eq1 - donkey | eq2 - onager | eq3 - zorse | eq4 - zebra | eq5 - okapi | 
--- | --- | --- | --- | --- | --- | --- | 
equine | ![eq0 - horse](examples/equine/eq0-horse.png) | ![eq1 - donkey](examples/equine/eq1-donkey.png) | ![eq2 - onager](examples/equine/eq2-onager.png) | ![eq3 - zorse](examples/equine/eq3-zorse.png) | ![eq4 - zebra](examples/equine/eq4-zebra.png) | ![eq5 - okapi](examples/equine/eq5-okapi.png) | 

Class | fe0 - cat | fe1 - lion | fe2 - tiger | fe3 - leopard | fe4 - hyena | fe5 - meerkat | 
--- | --- | --- | --- | --- | --- | --- | 
feline | ![fe0 - cat](examples/feline/fe0-cat.png) | ![fe1 - lion](examples/feline/fe1-lion.png) | ![fe2 - tiger](examples/feline/fe2-tiger.png) | ![fe3 - leopard](examples/feline/fe3-leopard.png) | ![fe4 - hyena](examples/feline/fe4-hyena.png) | ![fe5 - meerkat](examples/feline/fe5-meerkat.png) | 

Class | fe6 - fossa | fe7 - caracal | fe8 - lynx | fe9 - bearcat | fe10 - jaguar | 
--- | --- | --- | --- | --- | --- | 
feline | ![fe6 - fossa](examples/feline/fe6-fossa.png) | ![fe7 - caracal](examples/feline/fe7-caracal.png) | ![fe8 - lynx](examples/feline/fe8-lynx.png) | ![fe9 - bearcat](examples/feline/fe9-bearcat.png) | ![fe10 - jaguar](examples/feline/fe10-jaguar.png) | 

Class | fe11 - cougar | fe12 - civet | fe13 - mongoose | fe14 - genet | fe15 - kusimanse | 
--- | --- | --- | --- | --- | --- | 
feline | ![fe11 - cougar](examples/feline/fe11-cougar.png) | ![fe12 - civet](examples/feline/fe12-civet.png) | ![fe13 - mongoose](examples/feline/fe13-mongoose.png) | ![fe14 - genet](examples/feline/fe14-genet.png) | ![fe15 - kusimanse](examples/feline/fe15-kusimanse.png) | 

Class | pri0 - monkey | pri1 - nightmonkey | pri2 - lemur | pri3 - tarsier | pri4 - gorilla | pri5 - mandrill |
--- | --- | --- | --- | --- | --- | --- |
primate | ![pri0 - monkey](examples/primate/pri0-monkey.png) | ![pri1 - nightmonkey](examples/primate/pri1-nightmonkey.png) | ![pri2 - lemur](examples/primate/pri2-lemur.png) | ![pri3 - tarsier](examples/primate/pri3-tarsier.png) | ![pri4 - gorilla](examples/primate/pri4-gorilla.png) | ![pri5 - mandrill](examples/primate/pri5-mandrill.png) |

Class | pri6 - orangutan | pri7 - proboscis | pri8 - tamarin | pri9 - colobus | pri10 - ape | pri11 - marmoset | pri12 - colugo |
--- | --- | --- | --- | --- | --- | --- | --- |
primate | ![pri6 - orangutan](examples/primate/pri6-orangutan.png) | ![pri7 - proboscis](examples/primate/pri7-proboscis.png) | ![pri8 - tamarin](examples/primate/pri8-tamarin.png) | ![pri9 - colobus](examples/primate/pri9-colobus.png) | ![pri10 - ape](examples/primate/pri10-ape.png) | ![pri11 - marmoset](examples/primate/pri11-marmoset.png) | ![pri12 - colugo](examples/primate/pri12-colugo.png) |

Class |  re0 - snake |  re1 - turtle |  re2 - sea turtle |  re3 - lizard |  re4 - frilled-neck lizard |  
--- | --- | --- | --- | --- | --- | 
reptile |  ![re0 - snake](examples/reptile/re0-snake.png) |  ![re1 - turtle](examples/reptile/re1-turtle.png) |  ![re2 - sea_turtle](examples/reptile/re2-sea_turtle.png) |  ![re3 - lizard](examples/reptile/re3-lizard.png) |  ![re4 - frilled-neck_lizard](examples/reptile/re4-frilldneck_lizard.png) |  


Class |  re5 - monitor lizard |  re6 - chameleon |  re7 - aligator |  re8 - iguana |  re9 - gila monster |  
--- | --- | --- | --- | --- | --- | 
reptile | ![re5 - monitor_lizard](examples/reptile/re5-monitor_lizard.png) | ![re6 - chameleon](examples/reptile/re6-chameleon.png) | ![re7 - aligator](examples/reptile/re7-aligator.png) | ![re8 - iguana](examples/reptile/re8-iguana.png) | ![re9 - gila_monster](examples/reptile/re9-gila_monster.png) | 


Class | ru0 - deer | ru1 - pronghorn | ru2 - cattle | ru3 - sheep | ru4 - goat | 
--- | --- | --- | --- | --- | --- |
ruminant | ![ru0-deer](examples/ruminant/ru0-deer.png) | ![ru1-pronghorn](examples/ruminant/ru1-pronghorn.png) | ![ru2-cattle](examples/ruminant/ru2-cattle.png) | ![ru3-sheep](examples/ruminant/ru3-sheep.png) | ![ru4-goat](examples/ruminant/ru4-goat.png) | 

Class | ru5 - markhor | ru6 - giraffe | ru7 - takin | ru8 - serow | 
--- | --- | --- | --- | --- |
ruminant | ![ru5-markhor](examples/ruminant/ru5-markhor.png) | ![ru6-giraffe](examples/ruminant/ru6-giraffe.png) | ![ru7-takin](examples/ruminant/ru7-takin.png) | ![ru8-serow](examples/ruminant/ru8-serow.png)


Class | tr0 - train | tr1 - tram | 
--- | --- | --- | 
train | ![tr0 - train](/examples/train/tr0-train.png) | ![tr1 - tram](/examples/train/tr1-tram.png) | 

Class | ve0 - car | ve1 - limo | ve2 - golf-cart | ve3 - jeep | ve4 - bus | ve5 - minibus 
--- | --- | --- | --- | --- | --- | --- |
vehicle | ![ve0 - car](examples/vehicle/ve0-car.png) | ![ve1 - limo](examples/vehicle/ve1-limo.png) | ![ve2 - golf-cart](examples/vehicle/ve2-golf-cart.png) | ![ve3 - jeep](examples/vehicle/ve3-jeep.png) | ![ve4 - bus](examples/vehicle/ve4-bus.png) | ![ve5 - minibus](examples/vehicle/ve5-minibus.png) |

Class | ve6 - minivan | ve7 - van | ve8 - caravan | ve9 - ambulance_van | ve10 - ambulance_truck |
--- | --- | --- | --- | --- | --- |
vehicle | ![ve6 - minivan](examples/vehicle/ve6-minivan.png) | ![ve7 - van](examples/vehicle/ve7-van.png) | ![ve8 - caravan](examples/vehicle/ve8-caravan.png) | ![ve9 - ambulance_van](examples/vehicle/ve9-ambulance_van.png) | ![ve10 - ambulance_truck](examples/vehicle/ve10-ambulance_truck.png) |

Class | ve11 - garbage truck | ve12 - firetruck | ve13 - car carrier trailer | ve14 - freight truck | ve15 - gravel truck |
--- | --- | --- | --- | --- | --- |
vehicle | ![ve11 - garbage truck](examples/vehicle/ve11-garbage_truck.png) | ![ve12 - firetruck](examples/vehicle/ve12-firetruck.png) | ![ve13 - car carrier trailer](examples/vehicle/ve13-car_carrier_trailer.png) | ![ve14 - freight truck](examples/vehicle/ve14-freight_truck.png) | ![ve15 - gravel truck](examples/vehicle/ve15-gravel_truck.png) |

Class | ve16 - mini truck | ve17 - pickup truck | ve18 - tractor | ve19 - excavator | ve20 - rolling compactor |
--- | --- | --- | --- | --- | --- |
vehicle | ![ve16 - mini truck](examples/vehicle/ve16-mini_truck.png) | ![ve17 - pickup truck](examples/vehicle/ve17-pickup_truck.png) | ![ve18 - tractor](examples/vehicle/ve18-tractor.png) | ![ve19 - excavator](examples/vehicle/ve19-excavator.png) | ![ve20 - rolling compactor](examples/vehicle/ve20-rolling_compactor.png) |

Class | ve21 - full-track tank | ve22 - half-track car | ve23 - bumper car | ve24 - go-kart | ve25 - amphibious car | ve26 - soapbox car |
--- | --- | --- | --- | --- | --- | --- |
vehicle | ![ve21 - full-track tank](examples/vehicle/ve21-full-track_tank.png) | ![ve22 - half-track car](examples/vehicle/ve22-half-track_car.png) | ![ve23 - bumper car](examples/vehicle/ve23-bumper_car.png) | ![ve24 - go-kart](examples/vehicle/ve24-go-kart.png) | ![ve25 - amphibious car](examples/vehicle/ve25-amphibious_car.png) | ![ve26 - soapbox car](examples/vehicle/ve26-soapbox_car.png) |


Class | wa0 - wooden boat | wa1 - jet boat | wa2 - catamaran boat | wa3 - yacht | wa4 - jetski | 
--- | --- | --- | --- | --- | --- |
watercraft | ![wa0-wooden_boat](examples/watercraft/wa0-wooden_boat.png) | ![wa1-jet_boat](examples/watercraft/wa1-jet_boat.png) | ![wa2-catamaran_boat](examples/watercraft/wa2-catamaran_boat.png) | ![wa3-yacht](examples/watercraft/wa3-yacht.png) | ![wa4-jetski](examples/watercraft/wa4-jetski.png) | 

Class | wa5 - sail boat | wa6 - other boat | wa7 - sail ship | wa8 - cruise ship | 
--- | --- | --- | --- | --- |
watercraft | ![wa5-sail_boat](examples/watercraft/wa5-sail_boat.png) | ![wa6-other_boat](examples/watercraft/wa6-other_boat.png) | ![wa7-sail_ship](examples/watercraft/wa7-sail_ship.png) | ![wa8-cruise_ship](examples/watercraft/wa8-cruise_ship.png) | 

Class | wa9 - military ship | wa10 - cargo ship | wa11 - other ship | wa12 - submarine | 
--- | --- | --- | --- | --- |
watercraft | ![wa9-military_ship](examples/watercraft/wa9-military_ship.png) | ![wa10-cargo_ship](examples/watercraft/wa10-cargo_ship.png) | ![wa11-other_ship](examples/watercraft/wa11-other_ship.png) | ![wa12-submarine](examples/watercraft/wa12-submarine.png) | 



`antelope` in 0-55k will be redone <br/>
`rat` in 0-35k --> separate chincilla <br/>
`cat` in 0-35k --> separate civet  and genet <br/>
`cougar` --> may be moved to lion, because of lack of clarity <br/>
`fe15` until 75k, there should only be 1.
