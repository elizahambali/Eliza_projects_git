{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "60ed452d-89c1-4dfc-b4e8-2d952dadae9c",
   "metadata": {},
   "source": [
    "### Project 1: Exploring climate data of Singapore\n",
    "\n",
    "### Overview\n",
    "This project looks at the rainfall and tidal data to find recommendations for National Outdoor Adventure Singapore (NOAS). NOAS is an outdoor adventure provider that designs and conducts programme for Institure of Higher Learning (IHL) students in Singapore. \n",
    "\n",
    "One of the key programme is the 9-days, Singapore Youth Outdoor (SYO) programme that is held annually for all IHL students. The programme objectives is to build social cohesion and resilience amongst the IHL students. \n",
    "\n",
    "SYO has been well-received and it is in its 5th year running. However, lately there were multiple feedback on one of the programme's activities i.e. Kayaking.\n",
    "\n",
    "### Problem Statement\n",
    "SYO students feedback that the kayaking expedition route is too short and easy. They are looking for a longer expedition route that is challenging and stretches them physically, emotionally and mentally. \n",
    "NOAS has been tasked to looked into extending the expedition route. However, before the new route can be implemented, a trial needs to conducted and assessed by NOAS Safety Committee Members (SCM). Hence NOAS is looking for the ideal month to conduct the new expedition trial route. Key considerating factors are:\n",
    "- low to minimal rainfall for the month; \n",
    "- longer duration of sunshine hours with reasonable humidity level; and \n",
    "- favorable tidal conditions.\n",
    "\n",
    "The assumption is that with heavy rainfall comes thunderstorms which will significantly impact the success of the trial. Hence mitigating those factors will greatly increase the chance of success because students can paddle confidently and safely. \n",
    "\n",
    "### Datasets / Data Dictionary\n",
    "The following datasets were sourced from data.gov.sg and MPA (tidal data).\n",
    "\n",
    "|Feature|Type|Dataset|Description|\n",
    "|---|---|---|---|\n",
    "|total_rainfall_by_month|float|rainfall-monthly-total|Total rainfall in mm| \n",
    "|rainy_days_by_month|float|rainfall-monhtly-number-of-rain-days|days that have recorded rainfall at 2mm, are considered rainy days|\n",
    "|humidity_by_month|float|relative-humidity-monthly-mean|average humidity for the month|\n",
    "|sunshine_hours_by_month|float|sunshine-duration-monthly-mean|average sunshine hours for the month|\n",
    "|tide_table|float|2022_tidetable|tidal conditions for the month|\n",
    "\n",
    "### Brief Summary of Analysis\n",
    "From the analysis, Jan 2022 seem to be the ideal month to conduct the new expedition trial route due to the following reasons:\n",
    "- minimal rainfall;\n",
    "- longer duration of sunshine hours;\n",
    "- reasonable humidity level; and\n",
    "- favorable tide conditions.\n",
    "\n",
    "### Visualisations Used\n",
    "The following visualisations were used: \n",
    "- scatter plot to measure the distribution of rainfall, humidity and sunshine hours\n",
    "- line plot to measure the distribution of the tidal height across the months and the tidal difference \n",
    "- histograms(pairplot) and heatmap to measure the correlations between the features\n",
    "\n",
    "### Conclusions and Recommendations\n",
    "In summary, NOAS recommends to SCM to conduct the kayaking expedition trial route from Pulau Ubin to East Coast campus at an estimated distance of 33km during Jan 2022. It is projected to be a success considering Jan has the lowest rainfall and the longest duration of sunshine hours including favorable tidal conditions. "
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "dsi-sg",
   "language": "python",
   "name": "dsi-sg"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.9.13"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
