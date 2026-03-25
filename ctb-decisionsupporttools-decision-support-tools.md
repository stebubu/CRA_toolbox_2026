# CTB decisionsupporttools

## Before you start / prerequisites

Before selecting or running any decision-support tool, practitioners should ensure the minimum prerequisites are in place.

Across the ARCADIA tutorials, recurring prerequisites include: (i) basic GIS and geodata handling skills; (ii) capacity to preprocess and quality-check inputs (projections, terrain, land cover/use, exposure proxies); (iii) basic understanding of modelling assumptions and limitations; (iv) correct interpretation of indicators and of the baseline vs NbS scenario logic used to quantify changes; and (v) adequate documentation to ensure reproducibility.

## Decision-support approaches and external resources

This section links to external tools, platforms, and methodologies that assist decision-making. Examples include early warning systems (real-time alerts and hazard mapping), scenario analysis tools (interactive modelling for climate impacts), and cost–benefit calculators to assess the viability of adaptation measures.

Selecting and prioritising adaptation measures—especially a broad set of Nature-based Solutions (NbS)—can be complex. This page introduces decision-support approaches that help officials and stakeholders make informed choices, with an emphasis on methods that better capture NbS-specific aspects (e.g., co-benefits and long-term ecosystem services) that traditional appraisal may undervalue.

Key tools and approaches include:

Multi-Criteria Analysis (MCA). A structured method to compare options against multiple criteria (e.g., cost, risk-reduction effectiveness, co-benefits, feasibility, maintenance). The ICARUS project on road resilience recommends a four-step MCA to evaluate NbS options and link criteria to key performance indicators (KPIs): ICARUS Toolbox.

Cost–Benefit Analysis (CBA) with ecosystem valuation. Economic appraisal of NbS can be strengthened by explicitly valuing ecosystem services (e.g., flood storage by wetlands, health benefits from reduced heat). For an overview of NbS appraisal resources and planning considerations, see: Deltares – Nature-based solutions tools.

Scenario planning and climate-impact modelling can support decisions under deep uncertainty. Depending on local capacity, this may range from qualitative stress-testing (e.g., dry vs wet futures) to quantitative modelling. Where modelling is used, transparent assumptions and careful uncertainty communication are essential.

Geospatial tools and risk mapping are often central to decision-making. GIS-based workflows enable visualisation and spatial analyses (e.g., overlaying hazard, exposure and vulnerability proxies; identifying priority areas; communicating results through maps and dashboards).

Policy and planning integration tools. Checklists, alignment matrices and participatory methods help ensure selected measures fit within existing planning frameworks and governance processes. For examples of planning-oriented tools and stakeholder engagement approaches, see: UNU – Tools and methods for climate adaptation planning.

Overall, decision-support should remain inclusive and transparent. Structured stakeholder engagement can build legitimacy and improve implementation readiness, especially when NbS options deliver multiple co-benefits that matter to different groups.

The CLIMAAX CRA Handbook, whose tools we refer to in some of the Arcadia tutorials, provide a concise overview of how to start and what to prepare for the use of its specific tools.

## CLIMAAX CRA workflows and tools

ARCADIA is aligned with the broader European climate risk assessment (CRA) landscape. The CLIMAAX CRA Handbook provides interoperable workflows and notebooks that can complement ARCADIA methods where appropriate (e.g., for hazard screening, risk calculation, uncertainty handling). The hazard-level workflow pages below provide entry points and contain links to the specific tools/notebooks used for each hazard:

* > ![](<.gitbook/assets/ctb-decisionsupporttools_image1 (1).png>)[Floods workflow page](https://handbook.climaax.eu/notebooks/workflows/floods.html)
* > [Heavy rainfall workflow page](https://handbook.climaax.eu/notebooks/workflows/heavy_rainfall.html)
* > [Heatwaves workflow page](https://handbook.climaax.eu/notebooks/workflows/heatwaves.html)
* > [Droughts workflow page](https://handbook.climaax.eu/notebooks/workflows/droughts.html)
* > [Fire workflow page](https://handbook.climaax.eu/notebooks/workflows/fire.html)
* > [Snow workflow page](https://handbook.climaax.eu/notebooks/workflows/snow.html)
* > [Storms workflow page](https://handbook.climaax.eu/notebooks/workflows/storms.html)

For an overview landing page (including additional assets and the toolbox entry point), see: [CLIMAAX – Handbook toolbox.](https://handbook.climaax.eu/intro.html)

## ARCADIA tools referenced in the tutorials

> <img src=".gitbook/assets/ctb-decisionsupporttools_image2 (1).png" alt="" data-size="original">
>
> The table below compiles the software/tools that are explicitly linked in the ARCADIA tutorials. Tools are grouped by a general, replicable classification (generic tools; specialised models; platforms/DSS/plugins). When a tool is included mainly as an alternative option or supporting step, it is marked as referenced.

| **Tool / platform**                                                                                                                    | **Type**                      | **Typical role in workflow**                                                                                                                      | **Status (used / referenced)**     |
| -------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- |
| [QGIS](https://qgis.org/)                                                                                                              | Generic tools (GIS)           | GIS preprocessing, mapping, and hazard–exposure overlay; used across several tutorials; often also listed as open alternative to proprietary GIS. | used / referenced (as alternative) |
| [ArcGIS Pro](https://www.esri.com/en-us/arcgis/products/arcgis-pro/overview)                                                           | Generic tools (GIS)           | GIS platform for spatial analysis, overlay, digitising planning layers, map production; used in flooding/BGI and heat-stress tutorials.           | used                               |
| [ArcGIS Pro Flood Simulation (toolset)](https://pro.arcgis.com/en/pro-app/latest/help/mapping/simulation/simulation-in-arcgis-pro.htm) | Generic tools (GIS)           | GIS-based flood simulation/visualisation workflow used in some tutorials for flood screening layers.                                              | used                               |
| [SAGA GIS (hydrology tools)](https://saga-gis.sourceforge.io/saga_tool_doc/8.1.1/ta_hydrology_25.html)                                 | Generic tools (preprocessing) | Terrain/hydrology preprocessing (e.g., flow/LS-factor derivations) used alongside GIS workflows.                                                  | used                               |
| [SaferPlaces](https://saferplaces.co/)                                                                                                 | Platforms / DSS               | Cloud platform for fluvial/pluvial/coastal hazard modelling; in some tutorials also paired with damage assessment option.                         | used                               |
| [IRRIFRAME](https://www.irriframe.it/irriframe/Content/IrriFrame_Documentation_english_version.pdf)                                    | Platforms / DSS               | Irrigation decision-support system to estimate crop water requirements and support irrigation scheduling within NbS performance assessment.       | used                               |
| [CRITERIA-3D](https://github.com/ARPA-SIMC/CRITERIA3D)                                                                                 | Specialised models            | Physically based soil–water balance and slope-stability modelling to derive landslide hazard indicators (e.g., factor of safety).                 | used                               |
| [SWAT+ (via QSWAT+ and SWAT+ Editor)](https://swat.tamu.edu/software/plus/)                                                            | Specialised models            | Catchment-scale hydrology / water-quality modelling to compare baseline vs NbS scenarios and derive runoff/nutrient indicators.                   | used                               |
| [QSWAT+ (QGIS plugin)](https://swatplus.gitbook.io/docs/installation)                                                                  | Platforms / plugins           | Pre/post-processing interface (sub-basins/HRUs, scenario comparison, visualisation) for SWAT+ projects.                                           | used                               |
| [AquaCrop (FAO)](https://www.fao.org/aquacrop/en/)                                                                                     | Specialised models            | Crop water-balance model used as an open alternative for irrigation scheduling where IRRIFRAME is unavailable.                                    | referenced (open alternative)      |
| [HEC-RAS](https://www.hec.usace.army.mil/software/hec-ras/download.aspx)                                                               | Specialised models            | 1D/2D hydraulic modelling for flood scenarios and production of flood extent/depth outputs.                                                       | used                               |
| [HEC-HMS](https://www.hec.usace.army.mil/software/hec-hms/)                                                                            | Specialised models            | Rainfall–runoff modelling to generate design hydrographs supporting flood assessments.                                                            | used                               |
| [SWMM (EPA Storm Water Management Model)](https://www.epa.gov/water-research/storm-water-management-model-swmm)                        | Specialised models            | Urban drainage / sewer hydraulics and stormwater quality modelling; supports NbS scenarios in pluvial flooding workflows.                         | used                               |
| [MIKE URBAN](https://www.dhigroup.com/upload/campaigns/mike-urban-plus/MIKE-URBAN-Plus-highlight-flyer.pdf)                            | Specialised models            | sewer network modelling, calibration and scenario testing (pluvial flooding and stormwater quality).                                              | used                               |
| [TauDEM](https://hydrology.usu.edu/taudem/taudem5/)                                                                                    | Specialised models            | Topographic hydrology analysis (flow paths, watershed delineation) supporting flood screening workflows.                                          | used                               |
| [ANUGA](https://anuga.anu.edu.au/)                                                                                                     | Specialised models            | Hydrodynamic model for coastal inundation simulation (storm surge / coastal flooding).                                                            | used                               |
| [RUSLE (soil-erosion calculation framework)](https://esdac.jrc.ec.europa.eu/content/soil-erosion-water-rusle2015/)                     | Specialised models            | Empirical erosion calculation used to estimate average annual soil loss and support baseline vs NbS comparisons.                                  | used                               |
| [UMEP (QGIS plugin)](https://umep-docs.readthedocs.io/projects/tutorial/en/latest/)                                                    | Platforms / plugins           | Urban microclimate modelling and heat/UHI scenario analysis (incl. UWG-based tools) within heat-stress tutorials.                                 | used                               |
| [ENVI-met](https://envi-met.com/)                                                                                                      | Specialised models            | 3D microclimate modelling to simulate temperature distribution, vegetation effects, and NbS cooling potential.                                    | used                               |
| [MUKLIMO\_3 (reference)](https://dwdbib.dwd.de/retrosammlung/content/titleinfo/46464)                                                  | Specialised models            | Urban climate model referenced/used in heat-stress tutorial materials.                                                                            | used                               |
| [Elements (EPW inspection/editing)](https://bigladdersoftware.com/projects/elements/)                                                  | Generic tools (support)       | Utility to inspect/edit weather files (EPW) supporting microclimate/heat workflows.                                                               | referenced (supporting step)       |

Table 1 - ARCADIA decision-support tools referenced in the current tutorials (classified by type and role; hyperlinks provided).

**Note:** in some tutorials, multiple tools are listed for the same functional step (e.g., proprietary vs open alternatives). In such cases, the tutorial indicates possible options; implementation should follow the local toolchain and data availability.
