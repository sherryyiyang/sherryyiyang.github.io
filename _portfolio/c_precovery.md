---
title: "Precovery"
excerpt: "Precovery of planetoids is a census of minor planets in by optimize condense data searching algorithm. Utilized Python, SQL, bash, and Git to process raw data and enhance the ADAM database. Expanded the database by 20%, adding over 500 million objects and 5 billion observations. [Github repository](https://github.com/B612-Asteroid-Institute/precovery)
<br/><img src='/images/precovery.png'>"
collection: "https://github.com/B612-Asteroid-Institute/precovery"

---

[https://github.com/B612-Asteroid-Institute/precovery](https://github.com/B612-Asteroid-Institute/precovery)

Precovery returns observations that lie within the angular tolerance of the predicted location of an input orbit propagated and mapped to the indexed observations. These observations are termed PrecoveryCandidates. Optionally, precovery can also return FrameCandidates which are frames where the orbit intersected the Healpix-mapped exposure for a specific dataset but no observations were found within the angular tolerance. In this case, quantities specific to individual observations will be returned as NaNs (mjd, ra_deg, dec_sigma_arcsec, ra_sigma_arcsec, mag, mag_sigma, observation_id, delta_ra_arcsec, delta_dec_arcsec, distance_arcsec), with the remaining quantities that define the Healpix-mapped exposure returned as normal.
