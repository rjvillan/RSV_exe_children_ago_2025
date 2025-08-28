# RSV_exe_children_ago_2025
Executables to simulate RSV transmission dynamics in children under 1

These are the executables where the agent-based model of respiratory syncytial virus described in the paper "Optimal immunization strategy for protection of children < 1 year against Respiratory Syncytial Virus infection and hospitalisation" co-authored by Juan-Carlos Cortés, Mónica López-Lacort, Ainara Mira-Iglesias, Cristina-Luisovna Pérez, Rafael-Jacinto Villanueva, and Javier Villanueva-Oller.

# Instructions for use
1) Put the model executable and the task file in the same folder. Ensure that the task file is named "problema.pro", which is the default file name.
2) Execute the model. It will look for the default task file name "problema.pro", and process it.
3) Wait for the model to end the simulation.
4) Once completed, there will be a result file named "xxx.sol", being xxx the task identifier assigned in the task file under the tag "Identificador".
5) If the model could not complete the simulation (this usually will mean a problem in the contents of the task file), the result file with contain the word "ERROR".
6) If the model could complete the simulation, the result file will be composed of several vectors. The first one, "Problema", contains the values used to do the simulation. After that, there come the simulation results with the following pattern:

   * "Infecciosos unicos primerizos":[new infectious agents for each simulated day],
   * "Susceptibles totales":[[total susceptible agents for each age from 0 to 100 years for day 1], [total susceptible agents for each age from 0 to 100 years for day 2], etc],
   * "Susceptibles totales => 0 y <= 5 meses":[total susceptible agents between 0 and 5 months for each simulated day],
   * "Susceptibles totales => 6 y <= 12 meses":[total susceptible agents between 6 and 12 months for each simulated day],
   * "Latentes totales":[[total latent agents for each age from 0 to 100 years for day 1], [total latent agents for each age from 0 to 100 years for day 2], etc],
   * "Latentes totales => 0 y <= 5 meses":[total latent agents between 0 and 5 months for each simulated day],
   * "Latentes totales => 6 y <= 12 meses":[total latent agents between 6 and 12 months for each simulated day],
   * "Infecciosos totales":[[total infectious agents for each age from 0 to 100 years for day 1], [total infectious agents for each age from 0 to 100 years for day 2], etc],
   * "Infecciosos totales => 0 y <= 5 meses":[total infectious agents between 0 and 5 months for each simulated day],
   * "Infecciosos totales => 6 y <= 12 meses":[total infectious agents between 6 and 12 months for each simulated day],
   * "Hospitalizados totales":[[total hospitalized agents for each age from 0 to 100 years for day 1], [total latent agents for each age from 0 to 100 years for day 2], etc],
   * "Hospitalizados totales => 0 y <= 5 meses":[total hospitalised agents between 0 and 5 months for each simulated day],
   * "Hospitalizados totales => 6 y <= 12 meses":[total hospitalised agents between 6 and 12 months for each simulated day],
   * "Recuperados totales":[[total recovered agents for each age from 0 to 100 years for day 1], [total recovered agents for each age from 0 to 100 years for day 2], etc],
   * "Recuperados totales => 0 y <= 5 meses":[total recovered agents between 0 and 5 months for each simulated day],
   * "Recuperados totales => 6 y <= 12 meses":[total recovered agents between 6 and 12 months for each simulated day],
   * "Infecciosos vacunados unicos":[[new infectious agents for each age from 0 to 100 years for day 1], [new infectious agents for each age from 0 to 100 years for day 2], etc],
   * "Infecciosos vacunados unicos => 0 y <= 5 meses":[new infectious agents between 0 and 5 months for each simulated day],
   * "Infecciosos vacunados unicos => 6 y <= 12 meses":[new infectious agents between 6 and 12 months for each simulated day],
   * "Infecciosos no vacunados unicos":[[new infectious non-vaccinated agents for each age from 0 to 100 years for day 1], [new infectious non-vaccinated agents for each age from 0 to 100 years for day 2], etc],
   * "Infecciosos no vacunados unicos => 0 y <= 5 meses":[new infectious non-vaccinated agents between 0 and 5 months for each simulated day],
   * "Infecciosos no vacunados unicos => 6 y <= 12 meses":[new infectious non-vaccinated agents between 6 and 12 months for each simulated day],
   * "Hospitalizados vacunados unicos":[[new hospitalised agents for each age from 0 to 100 years for day 1], [new hospitalised agents for each age from 0 to 100 years for day 2], etc],
   * "Hospitalizados vacunados unicos => 0 y <= 5 meses":[new hospitalised vaccinated agents between 0 and 5 months for each simulated day],
   * "Hospitalizados vacunados unicos => 6 y <= 12 meses":[new hospitalised vaccinated agents between 6 and 12 months for each simulated day],
   * "Hospitalizados no vacunados unicos":[[new hospitalised vaccinated agents for each age from 0 to 100 years for day 1],[new hospitalised vaccinated agents for each age from 0 to 100 years for day 1],etc],
   * "Hospitalizados no vacunados unicos => 0 y <= 5 meses":[new hospitalised non-vaccinated agents between 0 and 5 months for each simulated day],
   * "Hospitalizados no vacunados unicos => 6 y <= 12 meses":[new hospitalised non-vaccinated agents between 6 and 12 months for each simulated day],
   * "Vacunados totales (menores+maternos+mayores) unicos":[[new vaccinated agents for each age from 0 to 100 years for day 1],[new vaccinated agents for each age from 0 to 100 years for day 2],etc],
   * "Vacunados totales (menores => 0 y <= 5 meses) unicos":[new vaccinated agents between 0 and 5 months for each simulated day],
   * "Vacunados totales (menores => 6 y <= 12 meses) unicos":[new vaccinated agents between 6 and 12 months for each simulated day]

# Excel files
The Excel files contain a summary of the obtained results for all the strategies simulated, separated into children younger than a year old, "Summary_results_strategies_younger_than_1.xlsx" and children 0-5 months old, "Summary_results_strategies_0_5.xlsx".


