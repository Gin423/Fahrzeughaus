class Fahrzeug:
    def __init__(self, marke, modell, pferdestaerke, preis, farbe, baujahr):
        self.marke = marke
        self.modell = modell
        self.pferdestaerke = pferdestaerke
        self.preis = preis
        self.farbe = farbe
        self.baujahr = baujahr

class Sportwagen(Fahrzeug):
    def __init__(self, marke, modell, pferdestaerke, preis, farbe, baujahr, hoechstgeschwindigkeit, beschleunigung, verbrauch, antrieb):
        super().__init__(marke, modell, pferdestaerke, preis, farbe, baujahr)
        self.hoechstgeschwindigkeit = hoechstgeschwindigkeit
        self.beschleunigung = beschleunigung
        self.verbrauch = verbrauch
        self.antrieb = antrieb


    def __str__(self):
        return(
        f"{self.marke}\n" 
        f"{self.modell}\n" 
        f"{self.pferdestaerke}\n" 
        f"{self.preis}\n" 
        f"{self.farbe}\n" 
        f"{self.baujahr}\n" 
        f"{self.hoechstgeschwindigkeit}\n" 
        f"{self.beschleunigung}\n"
        f"{self.verbrauch}\n"
        f"{self.antrieb}"
        )

    def begruessung_spw(self):
        print("Sie befinden sich jetzt in der Kategorie: Sportwagen")


Ferrari_296_GTB = Sportwagen(
    marke = "Marke: Ferrari",
    modell = "Modell: 296 GTB",
    pferdestaerke = "PS: 830 ",
    preis = "Preis: 300.000€",
    farbe = "Farbe: Rosso Corsa",
    baujahr = "Baujahr: 2022",
    hoechstgeschwindigkeit = "Hoechstgeschwindigkeit: 330+ km/h",
    beschleunigung = "Beschleunigung: 0-100 in 2,9 Sekunden",
    verbrauch = "Verbrauch: 8,3 L/100 km",
    antrieb = "Antrieb: Hinterradantrieb"
    )

Porsche_911_Carrera_Coupe = Sportwagen(
    marke = "Marke: Porsche",
    modell = "Modell: 911 Carrera (Coupe)",
    pferdestaerke = "PS: 394",
    preis = "Preis: 140.000€",
    farbe = "Farbe: Lugano Blau",
    baujahr = "Baujahr: 2019",
    hoechstgeschwindigkeit = "Geschwindigkeit: 294 km/h",
    beschleunigung = "Beschleunigung: 0-100 in 4,1 Sekunden",
    verbrauch = "Verbrauch: 10,1 L/100 km",
    antrieb = "Antrieb: Heckantrieb"
    )

Chevrolet_Corvette_C8_Stingray = Sportwagen(
    marke = "Marke : Chevrolet",
    modell = "Modell: Corvette C8 Stingray",
    pferdestaerke = "PS: 482",
    preis = "Preis: 90.000€",
    farbe = "Farbe: Roswell Green Metallic",
    baujahr = "Baujahr: 2020",
    hoechstgeschwindigkeit = "Geschwindigkeit: 296 km/h",
    beschleunigung = "Beschleunigung: 0-100 in 3,5 Sekunden",
    verbrauch = "Verbrauch: 12,1 L/100 km",
    antrieb = "Antrieb: Hinterradantrieb/Heckmittelmotor"
    )

Mazda_MX_5_Roadster = Sportwagen(
    marke = "Marke: Mazda",
    modell = "Modell: MX-5 Roadster",
    pferdestaerke = "PS: 132 ",
    preis = "Preis: 35.000€",
    farbe = "Farbe: Soul Red Crystal",
    baujahr = "Baujahr: 2005",
    hoechstgeschwindigkeit = "Geschwindigkeit: 204 km/h",
    beschleunigung = "Beschleunigung: 0-100 in 8,3 Sekunden",
    verbrauch = "Verbrauch: 6,3 L/100 km",
    antrieb = "Antrieb: Hinterradantrieb"
    )

Lamborghini_Revuelto = Sportwagen(
    marke = "Marke: Lamborghini",
    modell = "Modell: Revuelto",
    pferdestaerke = "PS: 1015",
    preis = "Preis: 500.000€",
    farbe = "Farbe: Arancio Apodis",
    baujahr = "Baujahr: 2023",
    hoechstgeschwindigkeit = "Geschwindigkeit: 350 km/h",
    beschleunigung = "Beschleunigung: 0-100 in 2,5 Sekunden",
    verbrauch = "Verbrauch: 11,8L/100 km",
    antrieb = "Antrieb: Allradantrieb (Plug-in-Hybrid)"
    )

class Elektroauto(Fahrzeug):
    def __init__(self, marke, modell, pferdestaerke, preis, farbe, baujahr, reichweite, ladezeit, batteriegroesse):
        super().__init__(marke, modell, pferdestaerke, preis, farbe, baujahr)
        self.reichweite = reichweite
        self.ladezeit = ladezeit
        self.batteriegroesse = batteriegroesse


    def __str__(self):
        return (
        f"{self.marke}\n"
        f"{self.modell}\n"
        f"{self.pferdestaerke}\n"
        f"{self.preis}\n"
        f"{self.farbe}\n"
        f"{self.baujahr}\n"
        f"{self.reichweite}\n"
        f"{self.ladezeit}\n"
        f"{self.batteriegroesse}"
        )

    def begruessung_elkt(self):
        print("Sie befinden sich jetzt in der Kategorie: Elektroautos")


Tesla_Model_3 = Elektroauto(
    marke = "Marke: Tesla",
    modell = "Modell: Model 3",
    pferdestaerke = "PS: 283",
    preis = "Preis: 45.000€",
    farbe = "Farbe: Pearl White Multi Coat",
    baujahr = "Baujahr: 2024",
    reichweite = "Reichweite: 702 km",
    ladezeit = "Ladezeit AC: 6 Std. (11 kW) / DC: 25 Min. (250 kW Supercharger)",
    batteriegroesse = "Batteriegroesse: 79 kWh"
    )

Volkswagen_ID_3_Pro = Elektroauto(
    marke = "Marke: Volksawgen",
    modell = "Modell: ID.3 Pro",
    pferdestaerke ="PS: 204",
    preis = "Preis: 40.000€",
    farbe = "Farbe: Gletscherweiß",
    baujahr = "Baujahr: 2024",
    reichweite = "Reichweite: 434 km",
    ladezeit = "Ladezeit AC: 6:15 Std. (11 W) / DC: 35 Min. (120 kW)",
    batteriegroesse = "Batteriegroesse: 59 kWh"
    )

Hyundai_IONIQ_5 = Elektroauto(
    marke = "Marke: Hyunadi",
    modell = "Modell: IONIQ 5",
    pferdestaerke = "PS: 229",
    preis = "Preis: 48.000€",
    farbe = "Farbe: Atlas White",
    baujahr = "Baujahr: 2024",
    reichweite = "Reichweite: 507 km",
    ladezeit = "Ladezeit AC: 6:10 Std. (11 kW) / DC: 18 Min. (800V-Technik)",
    batteriegroesse = "Batteriegroesse: 77,4k Wh"
    )

BMW_i4_eDrive35_Gran_Coupe = Elektroauto(
    marke = "Marke: BMW",
    modell = "Modell: i4 eDrive35 Gran Coupe",
    pferdestaerke = "PS: 286",
    preis = "Preis: 57.000€",
    farbe = "Farbe: Alpinweiss",
    baujahr = "Baujahr: 2024",
    reichweite = "Reichweite: 483 km",
    ladezeit = "Ladezeit AC: 7 Std. (11 kW) / DC: 32 Min. (180 kW)",
    batteriegroesse = "Batteriegroesse: 70 kWh"
    )

MG_MG4_Electric = Elektroauto(
    marke = "Marke: MG",
    modell = "Modell: MG4 Electric",
    pferdestaerke = "PS: 170",
    preis = "Preis: 35.000€",
    farbe = "Farbe: Dover White",
    baujahr = "Baujahr: 2024",
    reichweite = "Reichweite: 350 km",
    ladezeit = "Ladezeit AC: 7,5 Std. (6,6 kW einphasig) / DC: 37 Min. (88 kW)",
    batteriegroesse = "Batteriegroesse: 51 kWh"
    )

class Truck(Fahrzeug):
    def __init__(self, marke, modell, pferdestaerke, preis, farbe, baujahr, nutzlast, verbrauch, kabine):
        super().__init__(marke, modell, pferdestaerke, preis, farbe, baujahr)
        self.nutzlast = nutzlast
        self.verbrauch = verbrauch
        self.kabine = kabine

    def __str__(self):
        return (
        f"{self.marke}\n"
        f"{self.modell}\n"
        f"{self.pferdestaerke}\n"
        f"{self.preis}\n"
        f"{self.farbe}\n"
        f"{self.baujahr}\n"
        f"{self.nutzlast}\n"
        f"{self.verbrauch}\n"
        f"{self.kabine}"
        )

    def begruessung_trk(self):
        print("Sie befinden sich jetzt in der Kategorie: Trucks")

MAN_TGX_18510 = Truck(
    marke = "Marke: MAN",
    modell = "Modell: TGX 18.510",
    pferdestaerke = "PS: 510",
    preis = "Preis: ca. 135.000€",
    farbe = "Farbe: Weiß",
    baujahr = "Baujahr: 2022",
    nutzlast = "Nutzlast: 11.500 kg",
    verbrauch = "Verbrauch: 28 L/100 km",
    kabine = "Kabine: GX Fernverkehrskabine"
    )

Volvo_FH_540 = Truck(
    marke = "Marke: Volvo",
    modell = "Modell: FH 540",
    pferdestaerke = "PS: 540",
    preis = "Preis: 150.000€",
    farbe = "Farbe: Silber",
    baujahr = "Baujahr: 2023",
    nutzlast = "Nutzlast: 11.000 kg",
    verbrauch = "Verbrauch: 27 L/100 km",
    kabine = "Kabine: Globetrotter XL"
    )

Scania_R_450 = Truck(
    marke = "Marke: Scania",
    modell = "Modell: R 450",
    pferdestaerke = "PS: 450",
    preis = "Preis: 125.000€",
    farbe = "Farbe: Blau",
    baujahr = "Baujahr: 2021",
    nutzlast = "Nutzlast: 11.300 kg",
    verbrauch = "Verbrauch: 28 L/100 km",
    kabine = "Kabine: R-Serie Highline"
    )

Mercedes_Actros_1845 = Truck(
    marke = "Marke: Mercedes-Benz",
    modell = "Modell: Actros 1845",
    pferdestaerke = "PS: 449",
    preis = "Preis: 145.000€",
    farbe = "Farbe: Grau",
    baujahr = "Baujahr: 2022",
    nutzlast = "Nutzlast: ca. 11.200 kg",
    verbrauch = "Verbrauch: 26 L/100 km",
    kabine = "Kabine: BigSpace"
    )

DAF_XF_480 = Truck(
    marke = "Marke: DAF",
    modell = "Modell: XF 480",
    pferdestaerke = "PS: 480",
    preis = "Preis: 130.000€",
    farbe = "Farbe: Rot",
    baujahr = "Baujahr: 2020",
    nutzlast = "Nutzlast: ca. 11.400 kg",
    verbrauch = "Verbrauch: ca. 29 L/100 km",
    kabine = "Kabine: Super Space Cab"
    )

class Motorrad(Fahrzeug):
    def __init__(self, marke, modell, pferdestaerke, preis, farbe, baujahr, hubraum, hoechstgeschwindigkeit, verbrauch,):
        super().__init__(marke, modell, pferdestaerke, preis, farbe, baujahr)
        self.hubraum = hubraum
        self.hoechstgeschwindigkeit = hoechstgeschwindigkeit
        self.verbrauch = verbrauch

    def __str__(self):
        return (
        f"{self.marke}\n"
        f"{self.modell}\n"
        f"{self.pferdestaerke}\n"
        f"{self.preis}\n"
        f"{self.farbe}\n"
        f"{self.baujahr}\n"
        f"{self.hubraum}\n"
        f"{self.hoechstgeschwindigkeit}\n"
        f"{self.verbrauch}"
        )

    def begruessung_mtrd(self):
        print("Sie befinden sich jetzt in der Kategorie: Motorrad")

Yamaha_MT_07 = Motorrad(
    marke = "Marke: Yamaha",
    modell = "Modell: MT-07",
    pferdestaerke = "PS: 73,4",
    preis = "Preis: ca. 8.524€",
    farbe = "Farbe: Tech Black",
    baujahr = "Baujahr: 2025",
    hubraum = "Hubraum: 689 ccm",
    hoechstgeschwindigkeit = "Höchstgeschwindigkeit: 205 km/h",
    verbrauch = "Verbrauch: ca. 4,2 L/100 km"
    )

Kawasaki_Z900 = Motorrad(
    marke = "Marke: Kawasaki",
    modell = "Modell: Z900",
    pferdestaerke = "PS: 125",
    preis = "Preis: 10.995€",
    farbe = "Farbe: Metallic Spark Black",
    baujahr = "Baujahr: 2026",
    hubraum = "Hubraum: 948 ccm",
    hoechstgeschwindigkeit = "Höchstgeschwindigkeit: 240 km/h",
    verbrauch = "Verbrauch: 4,8 L/100 km"
)

Honda_CB650R = Motorrad(
    marke = "Marke: Honda",
    modell = "Modell: CB650R",
    pferdestaerke = "PS: 95",
    preis = "Preis: 9.300€",
    farbe = "Farbe: Pearl Glare White",
    baujahr = "Baujahr: 2024",
    hubraum = "Hubraum: 649 ccm",
    hoechstgeschwindigkeit = "Höchstgeschwindigkeit: 220 km/h",
    verbrauch = "Verbrauch: 4,9 L/100 km"
    )

Ducati_Monster_937 = Motorrad(
    marke = "Marke: Ducati",
    modell = "Modell: Monster 937",
    pferdestaerke = "PS: 111",
    preis = "Preis: 11.000€",
    farbe = "Farbe: Ducati Red",
    baujahr = "Baujahr: 2024",
    hubraum = "Hubraum: 937 ccm",
    hoechstgeschwindigkeit = "Höchstgeschwindigkeit: 240 km/h",
    verbrauch = "Verbrauch: 5,5 L/100 km"
    )

BMW_S_1000_RR = Motorrad(
    marke = "Marke: BMW",
    modell = "Modell: S 1000 RR",
    pferdestaerke = "PS: 210",
    preis = "Preis: 20.490€ ",
    farbe = "Farbe: Racing Blue",
    baujahr = "Baujahr: 2024",
    hubraum = "Hubraum: 999 ccm",
    hoechstgeschwindigkeit = "Höchstgeschwindigkeit: 299 km/h",
    verbrauch = "Verbrauch: 6,4 L/100 km"
    )

while True:
    print("Guten Tag und willkommen in meinem Fahrzeughaus. Hier biete ich Ihnen 4 Autokategorien.")
    aktion = input("Welche der Kategorien möchten Sie wählen? (Sportwagen / Elektroauto / Truck / Motorrad / Beenden)")
    if aktion == "Sportwagen":
        print(Sportwagen.begruessung_spw)
        wahl = input("Welche der Sportwagen möchten Sie sich ansehen? (Ferrari 296 GTB / Porsche 911 Carrera Coupe / Chevrolet Corvette C8 Stingray / Mazda MX 5 Roadster / Lamborghini Revuelto / Beenden)")
        if wahl == "Ferrari 296 GTB":
            print(Ferrari_296_GTB)
        elif wahl == "Porsche 911 Carrera Coupe":
            print(Porsche_911_Carrera_Coupe)
        elif wahl == "Chevrolet Corvette C8 Stingray":
            print(Chevrolet_Corvette_C8_Stingray)
        elif wahl == "Mazda MX 5 Roadster":
            print(Mazda_MX_5_Roadster)
        elif wahl == "Lamborghini Revuelto":
            print(Lamborghini_Revuelto)
        elif wahl == "Beenden":
            print(aktion)
        else:
            print("Bitte geben Sie eine gültige Aktion ein!")

    elif aktion == "Elektroauto":
        print(Elektroauto.begruessung_elkt)
        wahl = input("Welche der E-Autos möchten Sie sich ansehen? (Tesla Model 3 / Volkswagen ID.3 Pro / Hyundai IONIQ 5 / BMW i4 eDrive Gran Coupe / MG M4 Electric / Beenden)")
        if wahl == "Tesla Model 3":
            print(Tesla_Model_3)
        elif wahl == "Volkswagen ID.3 Pro":
            print(Volkswagen_ID_3_Pro)
        elif wahl == "Hyundai IONIQ 5":
            print(Hyundai_IONIQ_5)
        elif wahl == "BMW i4 eDrive Gran Coupe":
            print(BMW_i4_eDrive35_Gran_Coupe)
        elif wahl == "MG M4 Electric":
            print(MG_MG4_Electric)
        elif wahl == "Beenden":
            print(aktion)
        else:
            print("Bitte geben Sie eine gültige Aktion ein!")

    elif aktion == "Truck":
        print(Truck.begruessung_trk)
        wahl = input("Welche der Trucks möchten Sie sich ansehen? (MAN TGX 18.510 / Volvo FH540 / Scania R450 / Mercedes Actros 1845 / DAX XF 480 / Beenden)")
        if wahl == "MAN TGX 18.510":
            print(MAN_TGX_18510)
        elif wahl == "Volvo FH540":
            print(Volvo_FH_540)
        elif wahl == "Scania R540":
            print(Scania_R_450)
        elif wahl == "Mercedes Actros 1845":
            print(Mercedes_Actros_1845)
        elif wahl == "DAX XF 480":
            print(DAF_XF_480)
        elif wahl == "Beenden":
            print(aktion)
        else:
            print("Bitte geben Sie eine gültige Aktion ein!")

    elif aktion == "Motorrad":
        print(Motorrad.begruessung_mtrd)
        wahl = input("Welche der Motorräder möchten Sie sich ansehen? (Yamaha MT07 / Kawasaki Z900 / Honda CB650R / Ducati Monster 937 / BMW S 1000 RR / Beenden)")
        if wahl == "Yamaha MT07":
            print(Yamaha_MT_07)
        elif wahl == "Kawasaki Z900":
            print(Kawasaki_Z900)
        elif wahl == "Honda CB650R":
            print(Honda_CB650R)
        elif wahl == "Ducati Monster 937":
            print(Ducati_Monster_937)
        elif wahl == "BMW S 1000 RR":
            print(BMW_S_1000_RR)
        elif wahl == "Beenden":
            print(aktion)
        else:
            print("Bitte geben Sie eine gültige Aktion ein!")

    elif aktion == "Beenden":
        print("Ich danke Ihnen für Ihren Besuch, einen schönen Tag noch.")
        break

    else:
        print("Bitte geben sie eine gültige Aktion ein!")
