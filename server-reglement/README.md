# Reglement for servere plassert hos Tromsøstudentenes Dataforening(TD)

_Endret: 2021-04-09_




## §1 Generell informasjon
Reglementet for servere plassert hos Tromsøstudentenes Dataforening(TD) gjelder for alt utstyr i TDs besittelse, både eid av TD selv, og av privatpersoner og organisasjoner som benytter seg av TDs infrastruktur.

### Kontaktinformasjon
#### Teknisk Ansvarlig
- Joakim Aalstad Alslie
    - Tlf: 91315181
    - Mail: Jal029@uit.no
- Bjørn Johansen
    - Tlf: 48237095
    - Mail: bjorn.l.johansen@uit.no

#### TDs styre
- Mail: td@list.uit.no


## §2 Protokoller og standarder
### DNS
- TDs DNS-soner td.org.uit.no og 219.242.129.IN-ADDR.ARPA. reguleres av TDs DNS-server(e).
    - Det kan på forespørsel delegeres undersoner av td.org.uit.no.
    - Gjeldende autorativ DNS-server goto.td.org.uit.no(129.242.219.9) og slaveserver opereres av UiT(i skrivende stund benoni.uit.no)
- Ved manuelt oppsett skal følgende servere brukes(i prioritert rekkefølge): 129.242.9.253, 129.242.4.254

### NTP
- UiT opererer to separate NTP-tjenere som synkroniseres mot GPS, disse distribueres av TD via DHCP til utstyr tilkoblet TDs nettverk. For manuelt oppsett kan følgende tjenere brukes: 129.242.4.240(ntp.uit.no), 129.242.4.241(ntp-public.uit.no)
		

### ICMP
- Alle maskiner som plasseres hos TD skal være satt til å svare på ICMP Echo/Reply(i henhold til RFC1122 3.2.2.6) på all

### IP
- TD administrerer et IPv4 adresserom bestående av 129.242.219.0/25 og vil erverve IPv6-adresserom i nær fremtid.
    - Det er forbudt å ta i bruk andre adresser på grensesnitt tilknyttet TDs nettverk enn de man har fått tildelt/avtalt med teknisk ansvarlige hos TD.


### Begrensninger
- Følgende protokoller og programvare er ikke tillatt å kjøre hos TD:
    - Egne DNS-servere
    - IRC-servere
    - NTP-servere
    - E-post-servere
    - RDP-servere

- TDs servernett er omfattet av UiT og Uninetts grenseaksesslister og Uninett/Nordunets DDoS-beskyttelse. Medlemmer av TD forplikter seg til enhver tid å respektere disse, og det vil ikke være aktuelt å åpne opp i disse på grunnlag av ønsker fra TD.

- TDs nettverk, utstyr og infrastruktur er en delt ressurs, og det forventes av brukere av dette viser skjønn og hensyn ovenfor andre brukere. Dette vil si at applikasjoner og bruk som skaper hinder eller brudd for andre bør unngås.Dersom det oppstår situasjoner der utstyr eller applikasjoner skaper problemer, vil ansvarlig eier bli kontaktet for å rette problemet. Det forventes at ansvarlig eier retter seg etter forslag og pålegg fra teknisk ansvarlig hos TD.

- Utstyr plassert i TDs infrastruktur er i utgangspunktet ment for personlig benyttelse for TDs medlemmer. Videreformidling av tilgang til utstyr til tredjepart i form av brukernavn/passord og lignende skal ikke foregå.

## §3 Oppsett av utstyr
- Alt utstyr som plasseres i TDs nettverk skal(med mindre annet er avtalt):
    - Settes opp med DHCP for adressetildeling
	- Dersom utstyret eller på grunn av tjenestens art ikke støtter eller har mulighet til adressetildeling via DHCP, må dette avtales med teknisk ansvarlige hos TD i forkant av utplassering/idriftsettelse.
    - Settes opp til å svare på ICMP echo/reply for alle adresser tildelt av TD
    - Merkes med hostname, eiers/ansvarliges navn, telefonnummer og e-postadresse.
    - Være avklart med teknisk ansvarlig før innplassering, og utstyr som fjernes skal meldes fra til teknisk ansvarlig, slik at dette kan fjernes fra administrative systemer og driftsdokumentasjon.
- TD forbeholder seg retten til å nekte innplassering av utstyr som ikke møter de kravene som stilles til utstyr som skal plasseres i TDs infrastruktur.
    - Dette ombefatter utstyr som:
	- Er brannfarlig eller mangler deler for å fungere som normalt
	- Tilsynelatende misligholdt eller skittent utstyr
	    - Kan medføre en sikkerhetsrisiko som følge av manglende sikring av operativsystem og programvare
	- Bruk av TDs infrastruktur er å regne som et privilege, og misbruk av denne kan medføre frakobling eller fjerning av utstyr og/eller server.
	    - Delt infrastruktur som strøm, nettverk og regnekraft må brukes med tanke på felleskapet. Utstrakt utnyttelse av ressursene som medfører ulempe for andre, vil kunne medføre sanksjoner eller frakobling.

## §4 Ansvarforhold
- Eiere av servere(både fysiske og virtuelle) er selv ansvarlig for sikkerhetskopi av sine data. TD er ikke ansvarlig for tap av data eller utstyr, uavhengig av årsak.
- Servere skal sikres fra å gi uvedkommende tilgang, både fysisk og via nettverk. Eiere er selv ansvarlig for sikring, og manglende sikring eller avdekking av sikkerhetshull som kan sette driften av TD eller omkringliggende tjenester i fare er grunnlag for midlertidig eller permanent fjerning av maskinen fra TDs infrastruktur.
- Enhver som plasserer sin server hos TD er selv jurisk ansvarlig for trafikk til og fra serveren, data som er lagret på denne, og hva den brukes til.
- TD vil i utgangspunktet etterkomme forespørsler fra myndigheter om tilgang til, eller informasjon om utstyr som er plassert hos TD. Det antas at gjeldende myndighet er ansvarlig for avklaringer rundt informasjonsutlevering, og eventuelle forhold mellom nevnte myndighet og eier er å anse som en sak mellom disse to parter.

- Teknisk ansvarlige har i utgangspunktet taushetsplikt om forhold som kan ramme tap av personvern, omdømme eller andre forhold.

## §5 Sanksjoner og mislighold
- Ved manglende etterkommelse av krav beskrevet i §3, vil utstyr kunne midlertidig eller permanent kobles fra TDs infrastruktur og fjernes, og dersom eier ikke melder seg innen rimelig tid, så vil utstyret bli lagret og til slutt tilfalle TDs eie.
