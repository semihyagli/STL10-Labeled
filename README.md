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

Class | mac0 - tractor | mac1 - excavator | mac2 - rolling compactor | mac3 - full-track tank | mac4 - half-track car | mac5 - forklift | mac6 - rocket | 
--- | --- | --- | --- | --- | --- | --- | --- | 
machinery | ![mac0 - tractor](examples/machinery/mac0-tractor.png) | ![mac1 - excavator](examples/machinery/mac1-excavator.png) | ![mac2 - rolling compactor](examples/machinery/mac2-rolling_compactor.png) | ![mac3 - full-track tank](examples/machinery/mac3-full-track_tank.png) | ![mac4 - half-track car](examples/machinery/mac4-half-track_car.png) | ![mac5 - forklift](examples/machinery/mac5-forklift.png) | ![mac6 - rocket](examples/machinery/mac6-rocket.png) | 

Class | mm0 - dolphin | mm1 - whale | mm2 - narwhal | mm3 - vaquita | 
--- | --- | --- | --- | --- | 
marine mammals | ![mm0 - dolphin](examples/marine_mammals/mm0-dolphin.png) | ![mm1 - whale](examples/marine_mammals/mm1-whale.png) | ![mm2 - narwhal](examples/marine_mammals/mm2-narwhal.png) | ![mm3 - vaquita](examples/marine_mammals/mm3-vaquita.png) | 

Class | mm4 - dugong/manatee | mm5 - seal/sea lion | mm6 - walrus | mm7 - porpoise | 
--- | --- | --- | --- | --- | 
marine mammals | ![mm4 - dugong/manatee](examples/marine_mammals/mm4-dugong.png) | ![mm5 - seal/sea lion](examples/marine_mammals/mm5-seal.png) | ![mm6 - walrus](examples/marine_mammals/mm6-walrus.png) | ![mm7 - porpoise](examples/marine_mammals/mm7-porpoise.png) | 

Class | mu0 - badger | mu1 - weasel/stoat | mu2 - polecat | mu3 - ferret | mu4 - mink | mu5 - wolverine | 
--- | --- | --- | --- | --- | --- | --- | 
mustelinae | ![mu0 - badger](examples/mustelinae/mu0-badger.png) | ![mu1 - weasel/stoat](examples/mustelinae/mu1-weasel.png) | ![mu2 - polecat](examples/mustelinae/mu2-polecat.png) | ![mu3 - ferret](examples/mustelinae/mu3-ferret.png) | ![mu4 - mink](examples/mustelinae/mu4-mink.png) | ![mu5 - wolverine](examples/mustelinae/mu5-wolverine.png) | 

Class | mu6 - tayra | mu7 - skunk | mu8 - otter | mu9 - marten | mu10 - fisher | 
--- | --- | --- | --- | --- | --- | 
mustelinae | ![mu6 - tayra](examples/mustelinae/mu6-tayra.png) | ![mu7 - skunk](examples/mustelinae/mu7-skunk.png) | ![mu8 - otter](examples/mustelinae/mu8-otter.png) | ![mu9 - marten](examples/mustelinae/mu9-marten.png) | ![mu10 - fisher](examples/mustelinae/mu10-fisher.png) | 

Class | pri0 - monkey | pri1 - nightmonkey | pri2 - lemur | pri3 - tarsier | pri4 - gorilla | pri5 - mandrill | pri6 - orangutan |
--- | --- | --- | --- | --- | --- | --- | --- |
primate | ![pri0 - monkey](examples/primate/pri0-monkey.png) | ![pri1 - nightmonkey](examples/primate/pri1-nightmonkey.png) | ![pri2 - lemur](examples/primate/pri2-lemur.png) | ![pri3 - tarsier](examples/primate/pri3-tarsier.png) | ![pri4 - gorilla](examples/primate/pri4-gorilla.png) | ![pri5 - mandrill](examples/primate/pri5-mandrill.png) | ![pri6 - orangutan](examples/primate/pri6-orangutan.png) | 

Class | pri7 - proboscis | pri8 - tamarin | pri9 - colobus | pri10 - ape | pri11 - marmoset | pri12 - colugo |
--- | --- | --- | --- | --- | --- | --- |
primate | ![pri7 - proboscis](examples/primate/pri7-proboscis.png) | ![pri8 - tamarin](examples/primate/pri8-tamarin.png) | ![pri9 - colobus](examples/primate/pri9-colobus.png) | ![pri10 - ape](examples/primate/pri10-ape.png) | ![pri11 - marmoset](examples/primate/pri11-marmoset.png) | ![pri12 - colugo](examples/primate/pri12-colugo.png) |

Class | pr0 - raccoon | pr1 - ringtail | pr2 - coati | pr3 - kinkajou | pr4 - olinguito |
--- | --- | --- | --- | --- | --- | 
procyonid | ![pr0 - raccoon](examples/procyonid/pr0-raccoon.png) | ![pr1 - ringtail](examples/procyonid/pr1-ringtail.png) | ![pr2 - coati](examples/procyonid/pr2-coati.png) | ![pr3 - kinkajou](examples/procyonid/pr3-kinkajou.png) | ![pr4 - olinguito](examples/procyonid/pr4-olinguito.png) | 

Class |  re0 - snake |  re1 - turtle |  re2 - sea turtle |  re3 - lizard |  re4 - frilled-neck lizard |  
--- | --- | --- | --- | --- | --- | 
reptile |  ![re0 - snake](examples/reptile/re0-snake.png) |  ![re1 - turtle](examples/reptile/re1-turtle.png) |  ![re2 - sea_turtle](examples/reptile/re2-sea_turtle.png) |  ![re3 - lizard](examples/reptile/re3-lizard.png) |  ![re4 - frilled-neck_lizard](examples/reptile/re4-frilldneck_lizard.png) |  

Class |  re5 - monitor lizard |  re6 - chameleon |  re7 - aligator |  re8 - iguana |  re9 - gila monster |  
--- | --- | --- | --- | --- | --- | 
reptile | ![re5 - monitor_lizard](examples/reptile/re5-monitor_lizard.png) | ![re6 - chameleon](examples/reptile/re6-chameleon.png) | ![re7 - aligator](examples/reptile/re7-aligator.png) | ![re8 - iguana](examples/reptile/re8-iguana.png) | ![re9 - gila_monster](examples/reptile/re9-gila_monster.png) | 

Class |  ro0 - mouse |  ro1 - rat |  ro2 - hamster |  ro3 - guinea pig |  ro4 - squirrel |  ro5 - rabbit |  
--- | --- | --- | --- | --- | --- | --- | 
rodent | ![ro0 - mouse](examples/rodent/ro0-mouse.png) | ![ro1 - rat](examples/rodent/ro1-rat.png) | ![ro2 - hamster](examples/rodent/ro2-hamster.png) | ![ro3 - guinea pig](examples/rodent/ro3-guinea_pig.png) | ![ro4 - squirrel](examples/rodent/ro4-squirrel.png) | ![ro5 - rabbit](examples/rodent/ro5-rabbit.png) | 

Class |  ro6 - pika |  ro7 - vole |  ro8 - mouse-deer |  ro9 - agouti |  ro10 - jerboa |  ro11 - marmot |  
--- | --- | --- | --- | --- | --- | --- | 
rodent | ![ro6 - pika](examples/rodent/ro6-pika.png) | ![ro7 - vole](examples/rodent/ro7-vole.png) | ![ro8 - mouse-deer](examples/rodent/ro8-mouse-deer.png) | ![ro9 - agouti](examples/rodent/ro9-agouti.png) | ![ro10 - jerboa](examples/rodent/ro10-jerboa.png) | ![ro11 - marmot](examples/rodent/ro11-marmot.png) | 

Class |  ro12 - nutria |  ro13 - chinchilla |  ro14 - shrew |  ro15 - paca |  ro16 - lemming |  ro17 - hedgehog |  
--- | --- | --- | --- | --- | --- | --- | 
rodent | ![ro12 - nutria](examples/rodent/ro12-nutria.png) | ![ro13 - chinchilla](examples/rodent/ro13-chinchilla.png) | ![ro14 - shrew](examples/rodent/ro14-shrew.png) | ![ro15 - paca](examples/rodent/ro15-paca.png) | ![ro16 - lemming](examples/rodent/ro16-lemming.png) | ![ro17 - hedgehog](examples/rodent/ro17-hedgehog.png) | 

Class | ru0 - deer | ru1 - pronghorn | ru2 - cattle | ru3 - sheep | ru4 - goat | 
--- | --- | --- | --- | --- | --- |
ruminant | ![ru0-deer](examples/ruminant/ru0-deer.png) | ![ru1-pronghorn](examples/ruminant/ru1-pronghorn.png) | ![ru2-cattle](examples/ruminant/ru2-cattle.png) | ![ru3-sheep](examples/ruminant/ru3-sheep.png) | ![ru4-goat](examples/ruminant/ru4-goat.png) | 

Class | ru5 - markhor | ru6 - giraffe | ru7 - takin | ru8 - serow | ru9 - goral |
--- | --- | --- | --- | --- | --- |
ruminant | ![ru5-markhor](examples/ruminant/ru5-markhor.png) | ![ru6-giraffe](examples/ruminant/ru6-giraffe.png) | ![ru7-takin](examples/ruminant/ru7-takin.png) | ![ru8-serow](examples/ruminant/ru8-serow.png) | ![ru9-goral](examples/ruminant/ru9-goral.png) |

Class | sw0 - pig | sw1 - boar/peccary | sw2 - warthog | sw3 - babirusa | 
--- | --- | --- | --- | --- | 
swine | ![sw0 - pig](examples/swine/sw0-pig.png) | ![sw1 - boar/peccary](examples/swine/sw1-boar.png) | ![sw2 - warthog](examples/swine/sw2-warthog.png) | ![sw3 - babirusa](examples/swine/sw3-babirusa.png) | 

Class | tr0 - train | tr1 - tram | 
--- | --- | --- | 
train | ![tr0 - train](/examples/train/tr0-train.png) | ![tr1 - tram](/examples/train/tr1-tram.png) | 

Class | tru0 - truck-general | tru1 - truck bobtail | tru2 - freight truck | tru3 - gravel truck | tru4 - small-box truck | tru5 - mini truck | 
--- | --- | --- | --- | --- | --- | --- | 
truck | ![tru0 - truck-general](examples/truck/tru0-truck-general.png) | ![tru1 - truck bobtail](examples/truck/tru1-truck_bobtail.png) | ![tru2 - freight truck](examples/truck/tru2-freight_truck.png) | ![tru3 - gravel truck](examples/truck/tru3-gravel_truck.png) | ![tru4 - small-box truck](examples/truck/tru4-small-box_truck.png) | ![tru5 - mini truck](examples/truck/tru5-mini_truck.png) | 

Class | tru6 - pickup truck | tru7 - car carrier/trailer | tru8 - garbage truck | tru9 - firetruck | tru10 - tow truck | tru11 - snowplow | 
--- | --- | --- | --- | --- | --- | --- | 
truck | ![tru6 - pickup truck](examples/truck/tru6-pickup_truck.png) | ![tru7 - car carrier/trailer](examples/truck/tru7-car_carrier_trailer.png) | ![tru8 - garbage truck](examples/truck/tru8-garbage_truck.png) | ![tru9 - firetruck](examples/truck/tru9-firetruck.png) | ![tru10 - tow truck](examples/truck/tru10-tow_truck.png) | ![tru11 - snowplow](examples/truck/tru11-snowplow.png) | 

Class | ut0 - shopping cart | ut1 - dolly | ut2 - wheel barrow | ut3 - buffet trolley | 
--- | --- | --- | --- | --- | 
utility | ![ut0 - shopping cart](examples/utility/ut0-shopping_cart.png) | ![ut1 - dolly](examples/utility/ut1-dolly.png) | ![ut2 - wheel barrow](examples/utility/ut2-wheel_barrow.png) | ![ut3 - buffet trolley](examples/utility/ut3-buffet_trolley.png) | 

Class | ut4 - laundry cart | ut5 - stroller | ut6 - other utility | ut7 - sleigh | 
--- | --- | --- | --- | --- | 
utility | ![ut4 - laundry cart](examples/utility/ut4-laundry_cart.png) | ![ut5 - stroller](examples/utility/ut5-stroller.png) | ![ut6 - other utility](examples/utility/ut6-other_utility.png) | ![ut7 - sleigh](examples/utility/ut7-sleigh.png) | 

Class | ve0 - car | ve1 - limo | ve2 - golf-cart | ve3 - 4x4 | ve4 - bus | ve5 - minibus |  ve6 - minivan |
--- | --- | --- | --- | --- | --- | --- | --- | 
vehicle | ![ve0 - car](examples/vehicle/ve0-car.png) | ![ve1 - limo](examples/vehicle/ve1-limo.png) | ![ve2 - golf-cart](examples/vehicle/ve2-golf-cart.png) | ![ve3 - 4x4](examples/vehicle/ve3-4x4.png) | ![ve4 - bus](examples/vehicle/ve4-bus.png) | ![ve5 - minibus](examples/vehicle/ve5-minibus.png) | ![ve6 - minivan](examples/vehicle/ve6-minivan.png) |

Class | ve7 - van | ve8 - caravan | ve9 - bumper car | ve10 - go-kart | ve11 - amphibious | ve12 - soapbox car | ve13 - mini caravan | 
--- | --- | --- | --- | --- | --- | --- | --- | 
vehicle | ![ve7 - van](examples/vehicle/ve7-van.png) | ![ve8 - caravan](examples/vehicle/ve8-caravan.png) | ![ve9 - bumper car](examples/vehicle/ve9-bumper_car.png) | ![ve10 - go-kart](examples/vehicle/ve10-go-kart.png) | ![ve11 - amphibious](examples/vehicle/ve11-amphibious.png) | ![ve12 - soapbox car](examples/vehicle/ve12-soapbox_car.png) | ![ve13 - mini caravan](examples/vehicle/ve13-mini_caravan.png) | 

Class | wa0 - wooden boat | wa1 - jet boat | wa2 - catamaran boat | wa3 - yacht | wa4 - jetski | 
--- | --- | --- | --- | --- | --- |
watercraft | ![wa0-wooden_boat](examples/watercraft/wa0-wooden_boat.png) | ![wa1-jet_boat](examples/watercraft/wa1-jet_boat.png) | ![wa2-catamaran_boat](examples/watercraft/wa2-catamaran_boat.png) | ![wa3-yacht](examples/watercraft/wa3-yacht.png) | ![wa4-jetski](examples/watercraft/wa4-jetski.png) | 

Class | wa5 - sail boat | wa6 - other boat | wa7 - sail ship | wa8 - cruise ship | 
--- | --- | --- | --- | --- |
watercraft | ![wa5-sail_boat](examples/watercraft/wa5-sail_boat.png) | ![wa6-other_boat](examples/watercraft/wa6-other_boat.png) | ![wa7-sail_ship](examples/watercraft/wa7-sail_ship.png) | ![wa8-cruise_ship](examples/watercraft/wa8-cruise_ship.png) | 

Class | wa9 - military ship | wa10 - cargo ship | wa11 - other ship | wa12 - submarine | 
--- | --- | --- | --- | --- |
watercraft | ![wa9-military_ship](examples/watercraft/wa9-military_ship.png) | ![wa10-cargo_ship](examples/watercraft/wa10-cargo_ship.png) | ![wa11-other_ship](examples/watercraft/wa11-other_ship.png) | ![wa12-submarine](examples/watercraft/wa12-submarine.png) | 

Class | om0 - bat | om1 - elephant | om2 - hyrax | om3 - hippo | om4 - rhino | om5 - tapir | om6 - anteater | 
--- | --- | --- | --- | --- | --- | --- | --- | 
other mammals | ![om0 - bat](examples/other_mammals/om0-bat.png) | ![om1 - elephant](examples/other_mammals/om1-elephant.png) | ![om2 - hyrax](examples/other_mammals/om2-hyrax.png) | ![om3 - hippo](examples/other_mammals/om3-hippo.png) | ![om4 - rhino](examples/other_mammals/om4-rhino.png) | ![om5 - tapir](examples/other_mammals/om5-tapir.png) | ![om6 - anteater](examples/other_mammals/om6-anteater.png) | 

Class | om7 - armadillo | om8 - pangolin | om9 - aardvark | om10 - tasmanian devil | om11 - sloth | om12 - cuscus | om13 - possum | 
--- | --- | --- | --- | --- | --- | --- | --- | 
other mammals | ![om7 - armadillo](examples/other_mammals/om7-armadillo.png) | ![om8 - pangolin](examples/other_mammals/om8-pangolin.png) | ![om9 - aardvark](examples/other_mammals/om9-aardvark.png) | ![om10 - tasmanian devil](examples/other_mammals/om10-tasmanian_devil.png) | ![om11 - sloth](examples/other_mammals/om11-sloth.png) | ![om12 - cuscus](examples/other_mammals/om12-cuscus.png) | ![om13 - possum](examples/other_mammals/om13-possum.png) | 

Class | ou0 - restaurant | ou1 - human | ou2 - multiple subject | ou3 - unknown animal | ou4 - unclear picture | ou5 - skull | 
--- | --- | --- | --- | --- | --- | --- | 
outlier | ![ou0 - restaurant](examples/outlier/ou0-restaurant.png) | ![ou1 - human](examples/outlier/ou1-human.png) | ![ou2 - multiple subject](examples/outlier/ou2-multiple_subject.png) | ![ou3 - unknown animal](examples/outlier/ou3-unknown_animal.png) | ![ou4 - unclear picture](examples/outlier/ou4-unclear_picture.png) | ![ou5 - skull](examples/outlier/ou5-skull.png) | 

Class |  ou6 - moth |  ou7 - car-interior |  ou8 - train-interior |  ou9 - ship-interior |  ou10 - japanese giant salamander |  ou11 - tambaqui fish |  
--- | --- | --- | --- | --- | --- | --- | 
outlier | ![ou6 - moth](examples/outlier/ou6-moth.png) | ![ou7 - car-interior](examples/outlier/ou7-car-interior.png) | ![ou8 - train-interior](examples/outlier/ou8-train-interior.png) | ![ou9 - ship-interior](examples/outlier/ou9-ship-interior.png) | ![ou10 - japanese giant salamander](examples/outlier/ou10-japanese_giant_salamander.png) | ![ou11 - tambaqui fish](examples/outlier/ou11-tambaqui_fish.png) | 

Class | ou12 - seahorse | ou13 - frog | ou14 - kangaroo | ou15 - mantis | 
--- | --- | --- | --- | --- | 
outlier | ![ou12 - seahorse](examples/outlier/ou12-seahorse.png) | ![ou13 - frog](examples/outlier/ou13-frog.png) | ![ou14 - kangaroo](examples/outlier/ou14-kangaroo.png) | ![ou15 - mantis](examples/outlier/ou15-mantis.png) | 

## Notes - For future Relases
`mouse` in 0-35k needs to be redone <br/>
`rat` in 0-35k --> separate chincilla (needs to be redone) <br/>
`cat` in 0-35k --> separate civet and genet <br/>
`rocket` separate two types of rocket into mchinery and aircraft... <br/>
`mm1` separate orca from whales <br/>
`sw1` separate peccaries <br/>
`ve12` separate bobsled and soap box car <br/>
`wa6` tugboat can be separated, also check for yacht <br/>