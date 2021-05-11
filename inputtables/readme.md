All the tables used for calculations if they are not available directly as web access

*Recomendación para nombre de tablas*: todo minusculas menos siglas de nombre propio o acronimos; siempre en csv para trabajar en python y tener control de versinoes en github; sin espacios, guiones o guiones bajos en el nombre (para poder hacer dobleclick y copiar el nombre) salvo que sean tablas importadas con nombres "oficiales" y los manenemos para trazabilidad; el nombre de fichero incluye extensión: .csv

# Input tables with real figures:

1. Capacidad_Asistencial_Historico_gobes.csv: Camas y UCIs por provincia. Source: https://www.mscbs.gob.es/profesionales/saludPublica/ccayes/alertasActual/nCov/documentos/Datos_Capacidad_Asistencial_Historico_10052021.csv
2. Capacidad_Asistencialbyhospital.csv: camas y UCIS por hospital. Source:memoria GVA 2019 (tabla xxx, pag xx) solo tiene datos de camas. pendiente respuesta de petición a portal transparencia GOB.es (juan)
3. hospitales.csv:hospital por departamento de salud. Source:Catálogo Nacional de Hospitales 2020 (CNH_2020) https://www.mscbs.gob.es/ciudadanos/prestaciones/centrosServiciosSNS/hospitales/home.htm
4. municipios.csv:municipios por departamento de salud. Source:
5. censo.csv: numero de habitantes por municipio (desglosado por edad y sexo). *(no es necesaria, se sustitye por SIP_dep.csv)* Source:
7. CNErenave.csv:  diario Casos-hosp-uci-def- by sexo-edad-provincia. . Source: https://cnecovid.isciii.es/covid19/resources/casos_hosp_uci_def_sexo_edad_provres.csv
8. dataset1.csv: transito de pacientes covid por el hospital. Source:
9. dataset2.csv: altas y bajas diarias y ocupación de hospital. Source:
10. dataset3.csv: Datastes generados Marin et al (2021). Source: Marin-Garcia, J. A., Ruiz, A., Maheut, J., Garcia-Sabater, J. P. (2021). A data generator for COVID-19 patients’ care requirements inside hospitals: data paper. WPOM-Working Papers on Operations Management, 12 (in press). https://doi.org/10.4995/wpom.15332
11. SIPdep.csv: numero de personas con el SIP en cada departamento de salud. Source: (pag 55) http://www.san.gva.es/documents/157385/8958678/Memoria_2019_imprimir_es 

# Test and Work in process tables:
2. dataset1fake1.csv : modelo de prueba, con datos inventados, con las estructura del dataset1 based on COVID19simulated-1617990046-Dataset3advB-v3-rep1.xlsx (Marin Et al , 2021)
3. dataset2fake1.csv : *(ver en outputtable)* modelo de prueba, con datos inventados, con las estructura del dataset2 (generado con una consulta de python a partir dataset1fake1.csv
