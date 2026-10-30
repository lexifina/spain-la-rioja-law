# La Rioja: law history in git

The law of the autonomous community of La Rioja (Comunidad Autónoma de La Rioja, Spain) as a git history: one file per article, one commit per norm that changed it, dated the day the change took effect, with the amending norm as the commit's author. `git blame` names the norm behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `es-ri/`. Spain's national law is in [lexifina/spain-law](https://github.com/lexifina/spain-law).

The text is in Spanish, exactly as the BOE's consolidated text prints it. Texts in co-official languages are not included.

Basado en datos de la Agencia Estatal Boletín Oficial del Estado (<https://www.boe.es>). Every text here is a consolidated text for information only (texto consolidado de carácter meramente informativo), not an official publication.

## What this repository holds

139 norms with 516 versions so far: the Estatuto de Autonomía first, then the laws, decree-laws and legislative decrees in force that the BOE consolidates, oldest first, added in parts of about 50. 18 of them are repealed norms the BOE consolidates: their whole history is kept, and their last commit removes the text on the day the repeal took effect, credited to the repealing norm. Regulations are not included (the BOE consolidates no autonomic decrees or orders).

| Folder | Norm | Versions | History | BOE last updated |
| --- | --- | ---: | --- | --- |
| `estatuto-de-autonomia/` | Ley Orgánica 3/1982, de 9 de junio, de Estatuto de Autonomía de La Rioja. | 6 | as first published, then each change: 9 July 1982 to 18 July 2010 | 2026-07-16 |
| `ley-1985-003/` | Ley 3/1985, de 20 de mayo, sobre iniciativa legislativa del pueblo riojano. | 1 | as first published: 30 May 1985 | 2025-12-16 |
| `ley-1985-004/` | Ley 4/1985, de 31 de mayo, reguladora de signos de la identidad riojana. | 1 | as first published: 27 August 1985 | 2025-12-16 |
| `ley-1987-002/` | Ley 2/1987, de 9 de febrero, de Salud Escolar. | 2 | as first published, then each change: 25 February 1987 to 1 January 2003 | 2025-12-17 |
| `ley-1989-006/` | Ley 6/1989, de 27 de diciembre, por el que se fija la capitalidad de los Partidos Judiciales de La Rioja. | 1 | as first published: 14 January 1990 | 2025-12-17 |
| `ley-1990-004/` | Ley 4/1990, de 29 de junio, de Bibliotecas de La Rioja. | 1 | as first published: 1 September 1990 | 2025-12-17 |
| `ley-1991-002/` | Ley 2/1991, de 7 de marzo, de Carreteras de la Comunidad Autónoma de La Rioja. | 6 | as first published, then each change: 17 April 1991 to 1 January 2026 | 2026-01-19 |
| `ley-1991-003/` | Ley 3/1991, de 21 de marzo, de Elecciones a la Diputación General de La Rioja. | 1 | as first published: 24 March 1991 | 2026-07-16 |
| `ley-1994-002/` | Ley 2/1994, de 24 de mayo, de Artesanía. | 1 | as first published: 17 June 1994 | 2025-12-17 |
| `ley-1994-004/` | Ley 4/1994, de 24 de mayo, de Archivos y Patrimonio Documental de La Rioja. | 4 | oldest version available, then each change: 17 June 1994 to 1 January 2025 | 2026-05-21 |
| `ley-1994-009/` | Ley 9/1994, de 30 de noviembre, de designación de Senadores en representación de la Comunidad Autónoma de La Rioja. | 1 | as first published: 4 December 1994 | 2025-12-17 |
| `ley-1995-002/` | Ley 2/1995, de 10 de febrero, de Protección y Desarrollo del Patrimonio Forestal de La Rioja. | 9 | as first published, then each change: 16 March 1995 to 28 February 2023 | 2025-12-18 |
| `ley-1995-004/` | Ley 4/1995, de 20 de marzo, de Creación del Parque Natural de la Sierra de Cebollera. | 3 | as first published, then each change: 29 March 1995 to 1 January 2007 | 2025-12-18 |
| `ley-1997-001/` | Ley 1/1997, de 31 de marzo, de Saneamiento de las Haciendas Locales de la Comunidad Autónoma de La Rioja. | 2 | as first published, then each change: 4 April 1997 to 1 January 2004 | 2025-12-18 |
| `ley-1997-002/` | Ley 2/1997, de 31 de marzo, de creación del Colegio Oficial de Podólogos de La Rioja. | 1 | as first published: 13 April 1997 | 2025-12-18 |
| `ley-1997-006/` | Ley 6/1997, de 18 de julio, reguladora del Consejo Económico y Social de La Rioja. | 4 | as first published, then each change: 7 September 1997 to 31 March 2022 | 2025-12-18 |
| `ley-1997-007/` | Ley 7/1997, de 3 de octubre, de creación de la Agencia de Desarrollo Económico de la Comunidad Autónoma de La Rioja. | 11 | as first published, then each change: 10 October 1997 to 22 July 2025 | 2025-12-18 |
| `ley-1998-007/` | Ley 7/1998, de 6 de mayo, del Voluntariado. | 1 | as first published: 13 May 1998 | 2025-12-18 |
| `ley-1999-002/` | Ley 2/1999, de 8 de marzo, de creación del Colegio Profesional de Protésicos Dentales de La Rioja. | 2 | as first published, then each change: 12 March 1999 to 27 December 2009 | 2025-12-18 |
| `ley-1999-004/` | Ley 4/1999, de 31 de marzo, de Colegios Profesionales de La Rioja. | 4 | as first published, then each change: 28 April 1999 to 1 January 2012 | 2025-12-18 |
| `ley-2000-003/` | Ley 3/2000, de 19 de junio, de Desarrollo Rural de la Comunidad Autónoma de La Rioja. | 1 | as first published: 23 June 2000 | 2025-12-18 |
| `ley-2000-005/` | Ley 5/2000, de 25 de octubre, de Saneamiento y Depuración de Aguas Residuales de La Rioja. | 23 | as first published, then each change: 1 November 2000 to 22 July 2025 | 2025-12-18 |
| `ley-2000-004/` | Ley 4/2000, de 25 de octubre, de Espectáculos Públicos y Actividades Recreativas de la Comunidad Autónoma de La Rioja. | 7 | as first published, then each change: 18 February 2001 to 1 January 2026 | 2026-06-26 |
| `ley-2001-001/` | Ley 1/2001, de 16 de marzo, reguladora de los Honores, Distinciones y Protocolo de la Comunidad Autónoma de La Rioja. | 2 | as first published, then each change: 23 March 2001 to 13 April 2018 | 2025-12-18 |
| `ley-2001-002/` | Ley 2/2001, de 31 de mayo, de Turismo de La Rioja. | 8 | as first published, then each change: 22 June 2001 to 1 January 2025 | 2025-12-18 |
| `ley-2001-003/` | Ley 3/2001, de 31 de mayo, del Consejo Consultivo de La Rioja. | 4 | as first published, then each change: 22 June 2001 to 1 January 2012 | 2025-12-18 |
| `ley-2001-004/` | Ley 4/2001, de 2 de julio, de Cooperativas de La Rioja. | 8 | as first published, then each change: 10 September 2001 to 1 January 2023 | 2025-12-18 |
| `ley-2001-005/` | Ley 5/2001, de 17 de octubre, sobre drogodependencias y otras adicciones. | 3 | as first published, then each change: 12 November 2001 to 1 January 2004 | 2025-12-18 |
| `ley-2002-002/` | Ley 2/2002, de 17 de abril, de Salud. | 8 | as first published, then each change: 23 April 2002 to 22 July 2025 | 2025-12-18 |
| `ley-2002-004/` | Ley 4/2002, de 1 de julio, de Cooperación para el Desarrollo. | 4 | as first published, then each change: 5 July 2002 to 1 January 2026 | 2026-01-19 |
| `ley-2002-007/` | Ley 7/2002, de 18 de octubre, de Sanidad Animal de la Comunidad Autónoma de La Rioja. | 3 | as first published, then each change: 1 November 2002 to 1 January 2023 | 2025-12-18 |
| `ley-2003-001/` | Ley 1/2003, de 3 de marzo, de la Administración Local de La Rioja. | 7 | as first published, then each change: 11 June 2003 to 1 January 2025 | 2026-03-31 |
| `ley-2003-003/` | Ley 3/2003, de 3 de marzo, de Organización del Sector Público de la Comunidad Autónoma de La Rioja. | 10 | as first published, then each change: 4 April 2003 to 22 July 2025 | 2026-05-21 |
| `ley-2003-005/` | Ley 5/2003, de 26 de marzo, reguladora de La Red de Itinerarios Verdes de La Rioja. | 2 | as first published, then each change: 23 April 2003 to 1 January 2014 | 2025-12-18 |
| `ley-2003-006/` | Ley 6/2003, de 26 de marzo, del Consejo Social de la Universidad de La Rioja. | 1 | as first published: 23 April 2003 | 2025-12-18 |
| `ley-2003-007/` | Ley 7/2003, de 26 de marzo, de Inserción Sociolaboral. | 2 | as first published, then each change: 3 May 2003 to 1 January 2009 | 2025-12-18 |
| `ley-2003-008/` | Ley 8/2003, de 28 de octubre, del Gobierno e Incompatibilidades de sus miembros. | 7 | as first published, then each change: 3 December 2003 to 1 January 2026 | 2026-01-19 |
| `ley-2004-001/` | Ley 1/2004, de 16 de febrero, para la aplicación al municipio de Logroño del régimen de organización de los municipios de gran población. | 1 | as first published: 20 February 2004 | 2025-12-18 |
| `ley-2004-002/` | Ley 2/2004, de 22 de abril, de creación del Colegio Oficial de Fisioterapeutas de La Rioja. | 2 | as first published, then each change: 27 April 2004 to 27 December 2009 | 2025-12-18 |
| `ley-2004-003/` | Ley 3/2004, de 25 de junio, de Consejos Escolares de La Rioja. | 2 | as first published, then each change: 21 July 2004 to 1 February 2021 | 2025-12-18 |
| `ley-2004-006/` | Ley 6/2004, de 18 de octubre, de Cajas de Ahorros de La Rioja. | 2 | as first published, then each change: 12 November 2004 to 20 December 2010 | 2025-12-18 |
| `ley-2004-007/` | Ley 7/2004, de 18 de octubre, de Patrimonio Cultural, Histórico y Artístico de La Rioja. | 5 | as first published, then each change: 12 November 2004 to 2 April 2017 | 2026-10-09 |
| `ley-2005-002/` | Ley 2/2005, de 1 de marzo, de Estadística de La Rioja. | 2 | as first published, then each change: 23 March 2005 to 1 February 2018 | 2025-12-18 |
| `ley-2005-003/` | Ley 3/2005, de 14 de marzo, de Ordenación de la actividad comercial y las actividades feriales en la Comunidad Autónoma de La Rioja. | 4 | as first published, then each change: 22 September 2005 to 1 January 2013 | 2025-12-18 |
| `ley-2005-004/` | Ley 4/2005, de 1 de junio, de funcionamiento y régimen jurídico de la Administración de la Comunidad Autónoma de La Rioja. | 9 | as first published, then each change: 7 September 2005 to 30 April 2026 | 2026-05-11 |
| `ley-2005-005/` | Ley 5/2005, de 1 de junio, de los sistemas de protección de la calidad agroalimentaria. | 3 | as first published, then each change: 8 June 2005 to 1 January 2015 | 2025-12-18 |
| `ley-2005-006/` | Ley 6/2005, de 15 de junio, de la Comunidad Riojana en el Exterior. | 1 | as first published: 22 July 2005 | 2025-12-18 |
| `ley-2005-008/` | Ley 8/2005, de 30 de junio, reguladora del Transporte Urbano por Carretera de La Rioja. | 1 | as first published: 12 January 2006 | 2025-12-18 |
| `ley-2005-009/` | Ley 9/2005, de 30 de septiembre, reguladora del documento de instrucciones previas en el ámbito de la sanidad. | 1 | as first published: 7 October 2005 | 2025-12-18 |
| `ley-2005-011/` | Ley 11/2005, de 19 de octubre, de Patrimonio de la Comunidad Autónoma de La Rioja. | 9 | as first published, then each change: 25 December 2005 to 1 January 2025 | 2025-12-18 |
| `ley-2006-001/` | Ley 1/2006, de 28 de febrero, de protección de menores de La Rioja. | 4 | as first published, then each change: 9 September 2006 to 1 February 2021 | 2025-12-18 |
| `ley-2006-002/` | Ley 2/2006, de 28 de febrero, de Pesca de La Rioja. | 6 | as first published, then each change: 9 June 2006 to 10 March 2023 | 2025-12-18 |
| `ley-2006-004/` | Ley 4/2006, de 19 de abril, del Instituto de Estudios Riojanos. | 1 | as first published: 26 April 2006 | 2025-12-18 |
| `ley-2006-005/` | Ley 5/2006, de 2 de mayo, de Ordenación del Territorio y Urbanismo de La Rioja. | 18 | as first published, then each change: 4 November 2006 to 1 January 2026 | 2026-04-29 |
| `ley-2006-006/` | Ley 6/2006, de 2 de mayo, del Defensor del Pueblo Riojano. | 5 | as first published, then each change: 5 May 2006 to 1 February 2020 | 2025-12-18 |
| `ley-2006-008/` | Ley 8/2006, de 18 de octubre, de transporte interurbano por carretera de La Rioja. | 4 | as first published, then each change: 24 November 2006 to 23 October 2014 | 2026-04-29 |
| `ley-2007-001/` | Ley 1/2007, de 12 de febrero, de Fundaciones de la Comunidad Autónoma de La Rioja. | 5 | as first published, then each change: 17 March 2007 to 2 April 2017 | 2025-12-19 |
| `ley-2007-002/` | Ley 2/2007, de 1 de marzo, de Vivienda de la Comunidad Autónoma de La Rioja. | 11 | as first published, then each change: 8 September 2007 to 22 July 2025 | 2026-04-29 |
| `ley-2007-003/` | Ley 3/2007, de 1 de marzo, de Calidad de los Servicios Sociales. | 1 | as first published: 9 March 2007 | 2025-12-19 |
| `ley-2007-004/` | Ley 4/2007, 17 de septiembre, de homologación de retribuciones de los miembros del Gobierno y Altos Cargos de la Comunidad Autónoma y del Parlamento de La Rioja con los de la Administración General del Estado. | 3 | as first published, then each change: 19 September 2007 to 1 January 2025 | 2025-12-19 |
| `ley-2009-004/` | Ley 4/2009, de 20 de octubre, de aprovechamientos de recursos pastables. | 1 | as first published: 24 October 2009 | 2025-12-19 |
| `ley-2009-007/` | Ley 7/2009, de 22 de diciembre, de Servicios Sociales de La Rioja. | 11 | as first published, then each change: 17 January 2010 to 22 July 2025 | 2025-12-19 |
| `ley-2010-005/` | Ley 5/2010, de 14 de mayo, de coordinación de Policías Locales de La Rioja. | 9 | as first published, then each change: 22 May 2010 to 22 July 2025 | 2025-12-19 |
| `ley-2010-007/` | Ley 7/2010, de 29 de septiembre, por la que se aprueban varios convenios de colaboración con otras Comunidades Autónomas para el establecimiento de programas de actuación conjunta en diversas materias. | 1 | as first published: 26 October 2010 | 2025-12-19 |
| `ley-2011-001/` | Ley 1/2011, de 7 de febrero, de protección civil y atención de emergencias de La Rioja. | 2 | as first published, then each change: 12 March 2011 to 1 January 2025 | 2025-12-19 |
| `ley-2011-003/` | Ley 3/2011, de 1 de marzo, de prevención, protección y coordinación institucional en materia de violencia en La Rioja. | 2 | as first published, then each change: 27 March 2011 to 23 September 2022 | 2025-12-19 |
| `ley-2012-001/` | Ley 1/2012, de 12 de junio, por la que se establece y regula una red de apoyo a la mujer embarazada. | 1 | as first published: 20 July 2012 | 2025-12-19 |
| `ley-2012-007/` | Ley 7/2012, de 21 de diciembre, de Medidas Fiscales y Administrativas para el año 2013. | 5 | as first published, then each change: 1 January 2013 to 31 October 2017 | 2025-12-19 |
| `ley-2013-001/` | Ley 1/2013, de 4 de marzo, de creación del Colegio Profesional de Ingenieros Técnicos en Informática de La Rioja. | 1 | as first published: 12 March 2013 | 2025-12-19 |
| `ley-2013-002/` | Ley 2/2013, de 4 de marzo, de creación del Colegio Profesional de Ingenieros en Informática de La Rioja. | 1 | as first published: 12 March 2013 | 2025-12-19 |
| `ley-2013-003/` | Ley 3/2013, de 4 de marzo, de creación del Colegio Profesional de Terapeutas Ocupacionales de La Rioja. | 1 | as first published: 12 March 2013 | 2025-12-19 |
| `ley-2013-004/` | Ley 4/2013, de 4 de marzo, de Creación del Colegio Profesional de Educadores Sociales de La Rioja. | 1 | as first published: 12 March 2013 | 2025-12-19 |
| `ley-2013-005/` | Ley 5/2013, de 12 de abril, para la defensa de los consumidores en la Comunidad Autónoma de La Rioja. | 2 | as first published, then each change: 9 May 2013 to 1 January 2014 | 2025-12-19 |
| `ley-2013-008/` | Ley 8/2013, de 27 de septiembre, de creación del Colegio Profesional de Periodistas de La Rioja. | 1 | as first published: 8 October 2013 | 2025-12-19 |
| `ley-2013-010/` | Ley 10/2013, de 21 de octubre, de apoyo a emprendedores, autónomos y Pymes. | 1 | as first published: 26 October 2013 | 2025-12-19 |
| `ley-2013-011/` | Ley 11/2013, de 21 de octubre, de Hacienda Pública de La Rioja. | 10 | oldest version available, then each change: 1 January 2014 to 1 January 2026 | 2026-01-19 |
| `ley-2014-002/` | Ley 2/2014, de 3 de junio, de medidas para la garantía y la continuidad de los servicios públicos en la Comunidad Autónoma de La Rioja. | 1 | as first published: 7 June 2014 | 2025-12-19 |
| `ley-2014-003/` | Ley 3/2014, de 11 de septiembre, de Transparencia y Buen Gobierno de La Rioja. | 5 | as first published, then each change: 18 September 2014 to 1 February 2021 | 2025-12-19 |
| `ley-2014-004/` | Ley 4/2014, de 11 de septiembre, de creación del Colegio de Economistas de La Rioja por unión del Colegio de Economistas de La Rioja y del Colegio de Titulares Mercantiles de La Rioja. | 1 | as first published: 18 September 2014 | 2025-12-19 |
| `ley-2015-001/` | Ley 1/2015, de 23 de marzo, del ejercicio físico y del deporte de La Rioja. | 1 | as first published: 26 March 2015 | 2025-12-19 |
| `ley-2015-002/` | Ley 2/2015, de 23 de marzo, del Estatuto de capitalidad de la ciudad de Logroño. | 1 | as first published: 14 April 2015 | 2025-12-19 |
| `ley-2015-003/` | Ley 3/2015, de 23 de marzo, de la Cámara Oficial de Comercio, Industria y Servicios de La Rioja. | 1 | as first published: 16 April 2015 | 2025-12-19 |
| `ley-2015-006/` | Ley 6/2015, de 29 de diciembre, de Medidas Fiscales y Administrativas para el año 2016. | 2 | as first published, then each change: 1 January 2016 to 2 April 2017 | 2025-12-19 |
| `ley-2016-001/` | Ley 1/2016, de 4 de abril, de impulso y consolidación del diálogo social en La Rioja. | 1 | as first published: 9 April 2016 | 2025-12-19 |
| `ley-2016-002/` | Ley 2/2016, de 14 de octubre, por la que se crea el Colegio Profesional de Logopedas de La Rioja. | 1 | as first published: 20 October 2016 | 2025-12-19 |
| `ley-2017-001/` | Ley 1/2017, de 3 de enero, del control del potencial vitícola en la Comunidad Autónoma de La Rioja. | 6 | as first published, then each change: 10 January 2016 to 1 January 2025 | 2025-12-19 |
| `ley-2017-003/` | Ley 3/2017, de 31 de marzo, de Medidas Fiscales y Administrativas para el año 2017. | 2 | as first published, then each change: 2 April 2017 to 31 October 2017 | 2025-12-19 |
| `ley-2017-004/` | Ley 4/2017, de 28 de abril, por la que se regula la Renta de Ciudadanía de La Rioja. | 7 | as first published, then each change: 5 September 2017 to 1 January 2026 | 2026-01-19 |
| `ley-2017-005/` | Ley 5/2017, de 8 de mayo, de Cuentas Abiertas para la Administración de La Rioja. | 1 | as first published: 13 May 2017 | 2025-12-19 |
| `ley-2017-006/` | Ley 6/2017, de 8 de mayo, de Protección del Medio Ambiente de la Comunidad Autónoma de La Rioja. | 1 | as first published: 1 June 2017 | 2025-12-19 |
| `ley-2017-007/` | Ley 7/2017, de 22 de mayo, de Comunicación y Publicidad Institucional. | 1 | as first published: 13 June 2017 | 2025-12-19 |
| `ley-2017-008/` | Ley 8/2017, de 19 de septiembre, de perros de asistencia de La Rioja. | 1 | as first published: 26 September 2017 | 2025-12-19 |
| `ley-2017-010/` | Ley 10/2017, de 27 de octubre, por la que se consolidan las disposiciones legales de la Comunidad Autónoma de La Rioja en materia de impuestos propios y tributos cedidos. | 19 | as first published, then each change: 1 January 2017 to 29 October 2026 | 2026-10-29 |
| `ley-2018-003/` | Ley 3/2018, de 16 de febrero, para la protección, difusión y promoción de la tauromaquia en La Rioja. | 1 | as first published: 22 February 2018 | 2025-12-20 |
| `ley-2018-004/` | Ley 4/2018, de 10 de abril, de medidas a favor de las víctimas del terrorismo de la Comunidad Autónoma de La Rioja. | 1 | as first published: 13 April 2018 | 2025-12-20 |
| `ley-2018-005/` | Ley 5/2018, de 19 de octubre, de gratuidad de los libros de texto y material curricular. | 4 | as first published, then each change: 17 June 2019 to 1 January 2023 | 2025-12-20 |
| `ley-2019-004/` | Ley 4/2019, de 1 de abril, por la que se crea el Colegio Profesional de Dietistas-Nutricionistas de La Rioja. | 1 | as first published: 6 April 2019 | 2025-12-20 |
| `ley-2021-003/` | Ley 3/2021, de 28 de abril, de Mecenazgo de la Comunidad Autónoma de La Rioja. | 2 | oldest version available, then each change: 30 April 2021 to 1 January 2022 | 2025-12-20 |
| `ley-2022-001/` | Ley 1/2022, de 23 de febrero, de transformación de la organización sanitaria "Fundación Hospital Calahorra" en Fundación Pública Sanitaria, regulación de su régimen jurídico e integración en el Servicio Riojano de Salud como entidad dependiente. | 2 | as first published, then each change: 25 February 2022 to 1 January 2024 | 2025-12-20 |
| `ley-2022-002/` | Ley 2/2022, de 23 de febrero, de igualdad, reconocimiento a la identidad y expresión de género y derechos de las personas trans y sus familiares en la Comunidad Autónoma de La Rioja. | 1 | as first published: 25 February 2022 | 2025-12-20 |
| `ley-2022-003/` | Ley 3/2022, de 29 de marzo, reguladora del juego y las apuestas de La Rioja y de la prevención del juego problemático y patológico. | 3 | as first published, then each change: 31 March 2022 to 2 July 2024 | 2025-12-20 |
| `ley-2022-004/` | Ley 4/2022, de 29 de marzo, por la que se alza la suspensión del funcionamiento del Consejo Económico y Social de La Rioja. | 1 | as first published: 31 March 2022 | 2025-12-20 |
| `ley-2022-005/` | Ley 5/2022, de 25 de abril, para la recuperación de la memoria democrática en La Rioja. | 1 | as first published: 28 April 2022 | 2025-12-20 |
| `ley-2022-008/` | Ley 8/2022, de 24 de junio, de caza y gestión cinegética de La Rioja. | 3 | as first published, then each change: 29 June 2022 to 27 May 2025 | 2025-12-20 |
| `ley-2022-009/` | Ley 9/2022, de 20 de julio, sobre economía social y solidaria de La Rioja. | 3 | as first published, then each change: 23 July 2022 to 1 January 2025 | 2025-12-20 |
| `ley-2022-011/` | Ley 11/2022, de 20 de septiembre, contra la Violencia de Género de La Rioja. | 1 | as first published: 23 September 2022 | 2025-12-20 |
| `ley-2022-012/` | Ley 12/2022, de 18 de octubre, de reforma de la Ley 1/2003, de 3 de marzo, de la Administración Local de La Rioja, para la admisión extraordinaria de la participación y la votación telemáticas. | 1 | as first published: 20 January 2023 | 2025-12-20 |
| `ley-2022-014/` | Ley 14/2022, de 23 de diciembre, de Juventud de La Rioja. | 1 | as first published: 28 December 2022 | 2026-07-16 |
| `ley-2023-001/` | Ley 1/2023, de 31 de enero, de accesibilidad universal de La Rioja. | 3 | as first published, then each change: 2 May 2023 to 22 July 2025 | 2025-12-20 |
| `ley-2023-002/` | Ley 2/2023, de 31 de enero, de biodiversidad y patrimonio natural de La Rioja. | 4 | as first published, then each change: 28 February 2023 to 27 May 2025 | 2025-12-20 |
| `ley-2023-003/` | Ley 3/2023, de 7 de marzo, de familias monoparentales en La Rioja. | 1 | as first published: 9 June 2023 | 2025-12-20 |
| `ley-2023-006/` | Ley 6/2023, de 22 de marzo, de las personas con problemas de salud mental y sus familias. | 1 | as first published: 25 March 2023 | 2025-12-20 |
| `ley-2023-007/` | Ley 7/2023, de 20 de abril, de igualdad efectiva de mujeres y hombres de La Rioja. | 3 | as first published, then each change: 26 April 2023 to 1 January 2026 | 2026-01-19 |
| `ley-2023-008/` | Ley 8/2023, de 20 de abril, de la ciencia, la tecnología y la innovación de La Rioja. | 2 | as first published, then each change: 26 April 2023 to 2 July 2024 | 2025-12-20 |
| `ley-2023-009/` | Ley 9/2023, de 5 de mayo, de función pública de la Comunidad Autónoma de La Rioja. | 6 | oldest version available, then each change: 8 August 2023 to 1 January 2026 | 2026-01-19 |
| `ley-2024-004/` | Ley 4/2024, de 1 de julio, de medidas administrativas y presupuestarias urgentes para la mejora de la prestación de los servicios públicos en La Rioja. | 1 | as first published: 2 July 2024 | 2025-12-20 |
| `ley-2025-003/` | Ley 3/2025, de 23 de junio, de garantías y derechos de las personas con necesidades paliativas. | 1 | as first published: 26 June 2025 | 2025-12-20 |
| `ley-2025-004/` | Ley 4/2025, de 1 de julio, del paisaje de La Rioja. | 3 | as first published, then each change: 22 July 2025 to 7 July 2026 | 2026-07-07 |
| `ley-2025-007/` | Ley 7/2025, de 9 de septiembre, de atención y ordenación farmacéutica de la Comunidad Autónoma de La Rioja. | 1 | as first published: 11 September 2025 | 2025-12-20 |
| `ley-2026-002/` | Ley 2/2026, de 28 de abril, de simplificación administrativa, mercado abierto y calidad normativa. | 1 | as first published: 30 April 2026 | 2026-05-12 |
| `ley-2026-003/` | Ley 3/2026, de 1 de julio, de la gratuidad de los estudios oficiales de grado universitario o estudios superiores equivalentes en La Rioja. | 1 | as first published: 4 July 2026 | 2026-07-17 |
| `ley-1986-002/` | Ley 2/1986, de 5 de marzo, del Consejo de la Juventud de la Rioja. | 3 | as first published, then each change: 11 June 1986 to 28 December 2022; **repealed** 28 December 2022 by Ley 14/2022, de 23 de diciembre (BOE-A-2023-1606) | 2025-12-17 |
| `ley-1990-003/` | Ley 3/1990, de 29 de junio, de Función Pública de la Administración Pública de la Comunidad Autónoma de La Rioja. | 18 | as first published, then each change: 5 August 1990 to 8 August 2023; **repealed** 8 August 2023 by Ley 9/2023, de 5 de mayo (BOE-A-2023-12918) | 2025-12-17 |
| `ley-1994-005/` | Ley 5/1994, de 19 de julio, de supresión de barreras arquitectónicas y promoción de la accesibilidad. | 2 | as first published, then each change: 27 August 1994 to 2 May 2023; **repealed** 2 May 2023 by Ley 1/2023, de 31 de enero (BOE-A-2023-4326) | 2025-12-17 |
| `ley-1995-005/` | Ley 5/1995, de 22 de marzo, de Protección de los Animales. | 3 | as first published, then each change: 2 April 1995 to 30 November 2018; **repealed** 30 November 2018 by Ley 6/2018, de 26 de noviembre (BOE-A-2018-17064) | 2025-12-18 |
| `ley-1998-008/` | Ley 8/1998, de 16 de junio, de Ordenación Farmacéutica de la Comunidad Autónoma de La Rioja. | 10 | as first published, then each change: 2 July 1998 to 11 September 2025; **repealed** 11 September 2025 by Ley 7/2025, de 9 de septiembre (BOE-A-2025-18522) | 2026-04-29 |
| `ley-1998-009/` | Ley 9/1998, de 2 de julio, de Caza de La Rioja. | 8 | as first published, then each change: 10 October 1998 to 29 June 2022; **repealed** 29 June 2022 by Ley 8/2022, de 24 de junio (BOE-A-2022-11228) | 2026-04-29 |
| `ley-1999-005/` | Ley 5/1999, de 13 de abril, reguladora del Juego y Apuestas. | 20 | as first published, then each change: 18 April 1999 to 31 March 2022; **repealed** 31 March 2022 by Ley 3/2022, de 29 de marzo (BOE-A-2022-6677) | 2025-12-18 |
| `ley-2002-005/` | Ley 5/2002, de 8 de octubre, de Protección del Medio Ambiente en La Rioja. | 7 | as first published, then each change: 1 November 2002 to 1 June 2017; **repealed** 1 June 2017 by Ley 6/2017, de 8 de mayo (BOE-A-2017-5831) | 2025-12-18 |
| `ley-2003-004/` | Ley 4/2003, de 26 de marzo, de Conservación de Espacios Naturales de La Rioja. | 2 | as first published, then each change: 2 April 2003 to 28 February 2023; **repealed** 28 February 2023 by Ley 2/2023, de 31 de enero (BOE-A-2023-4327) | 2025-12-18 |
| `ley-2005-007/` | Ley 7/2005, de 30 de junio, de Juventud de La Rioja. | 4 | as first published, then each change: 10 July 2005 to 28 December 2022; **repealed** 28 December 2022 by Ley 14/2022, de 23 de diciembre (BOE-A-2023-1606) | 2025-12-18 |
| `ley-2009-003/` | Ley 3/2009, de 23 de junio, de la Ciencia, la Tecnología y la Innovación. | 3 | as first published, then each change: 2 July 2009 to 26 April 2023; **repealed** 26 April 2023 by Ley 8/2023, de 20 de abril (BOE-A-2023-11338) | 2025-12-19 |
| `ley-2011-002/` | Ley 2/2011, de 1 de marzo, de autoridad del profesor y de la convivencia en los centros educativos de la Comunidad Autónoma de La Rioja. | 2 | as first published, then each change: 8 March 2011 to 1 January 2022; **repealed** 1 January 2022 by Ley 7/2021, de 27 de diciembre (BOE-A-2022-341) | 2025-12-19 |
| `ley-2014-005/` | Ley 5/2014, de 20 de octubre, de administración electrónica y simplificación administrativa. | 4 | as first published, then each change: 23 October 2014 to 30 April 2026; **repealed** 30 April 2026 by Ley 2/2026, de 28 de abril (BOE-A-2026-10117) | 2026-05-11 |
| `ley-2015-004/` | Ley 4/2015, de 23 de marzo, de defensa de la calidad de la viña y el vino de la Comunidad Autónoma de La Rioja. | 2 | as first published, then each change: 28 March 2015 to 10 January 2017; **repealed** 10 January 2017 by Ley 1/2017, de 3 de enero (BOE-A-2017-588) | 2025-12-19 |
| `ley-2018-006/` | Ley 6/2018, de 26 de noviembre, de protección de los animales en la Comunidad Autónoma de La Rioja. | 4 | as first published, then each change: 30 November 2018 to 8 August 2023; **repealed** 8 August 2023 by Ley 10/2023, de 7 de agosto (BOE-A-2023-18413) | 2025-12-20 |
| `ley-2021-005/` | Ley 5/2021, de 26 de octubre, sobre enseñanza de religión y sus alternativas. | 2 | as first published, then each change: 28 October 2021 to 2 July 2024; **repealed** 2 July 2024 by Ley 4/2024, de 1 de julio (BOE-A-2024-14006) | 2025-12-20 |
| `ley-2022-013/` | Ley 13/2022, de 2 de noviembre, de creación de la Agencia Riojana de Transición Energética y Cambio Climático. | 2 | as first published, then each change: 8 November 2022 to 1 January 2024; **repealed** 1 January 2024 by Ley 13/2023, de 28 de diciembre (BOE-A-2024-1778) | 2025-12-20 |
| `ley-2024-001/` | Ley 1/2024, de 24 de enero, medidas temporales y urgentes para la protección del paisaje de La Rioja. | 2 | as first published, then each change: 25 January 2024 to 22 July 2025; **repealed** 22 July 2025 by Ley 4/2025, de 1 de julio (BOE-A-2025-14378) | 2025-12-20 |

## Source

The consolidated legislation of the Agencia Estatal Boletín Oficial del Estado (BOE), through its open-data API, <https://www.boe.es/datosabiertos/api/legislacion-consolidada>. For each consolidated norm it gives every block of the text (article, disposition, annex, heading) with every version of that block, the day each version took effect (fecha_vigencia) and the norm that made it (id_norma). Each version here is the whole text as it stood on one of those days. The last column above is the BOE's own last-update date for the consolidated text.

## Dates

- Each commit is dated at **noon, Europe/Madrid, on the day the change took effect**: the fecha_vigencia the BOE gives the new block versions.
- A day on which the BOE records a new block version that changes no words is not a version here.
- Block versions with no in-force date (the BOE's 99999999, a date not yet fixed) are left out.
- An act's first commit is its first publication when the BOE's earliest text is the act as enacted; otherwise it is the oldest version the BOE holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 bis; `da-01.md` the Disposición adicional primera, `dt-` transitional, `dd-` repealing and `df-` final dispositions (`-unica` for "única"); `preambulo.md` the preamble, `firma.md` the signature, `anexo-*.md` the annexes. The book, title, chapter and section headings sit at the top of the file of the article that follows them. One paragraph per line; a table one line per row, cells separated by ` | `.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of the BOE's own text of that day, rebuilt from the source XML by a separate reader, and every file's text appears in it.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the norm that changed the text (a law, a decree-law, a ruling of the Constitutional Court), named by its title and BOE identifier, with an e-mail address that cannot exist (`<boe id>@boe.es.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. Only the texts published in the official journals are authentic. The history starts with the oldest text the BOE consolidates for each norm. Only the norms listed above are included; norms the BOE does not consolidate are not.
