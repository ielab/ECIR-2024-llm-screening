# ECIR-2024-llm-screening

## This file serves as a appendix table for result in Section 6: Discussion and outlook; only pure results are showed without further explaination.

***Table 1. Uncalibrated results comparison when inclusion-exclusion criteria is used in the prompt (note only four datasets are available here: CLEF-2017, CLEF-2018, CLEF-2019-dta, CLEF-2019-Intervention), Seed Collection does not contain extractable information. Inclusion-exclusion criteria extracted using protocol file, topics that does not contain protocol files are disregarded. 2-tailed t-test with bofferoni correction (p<0.05) are compared with LlaMa-2-7b-chat.***

|                  | Model            | P              | R              | B-AC           | F3            | Suc            | WSS            |
|------------------------------------------------|------------------|----------------|----------------|----------------|---------------|----------------|----------------|
| CLEF-2017 | BioBERT | 0.06 | 0.95 | 0.61* | 0.30 | 0.74* | 0.26* |
|                  | LlaMa-7b         | 0.04           | 0.92           | 0.48*          | 0.24          | 0.46           | 0.03*          |
|                  | LlaMa-2-7b       | 0.07           | 0.50*          | 0.60*          | 0.23*         | 0.02*          | 0.70*          |
|                  | LlaMa-2-13b      | 0.04           | 1.00*          | 0.50*          | 0.25          | 0.98*          | 0.00*          |
|                  | Falcon-7b        | 0.05           | 0.92           | 0.52*          | 0.25          | 0.44           | 0.12*          |
|                  | Alpaca-7b        | 0.04           | 0.92           | 0.51*          | 0.25          | 0.38           | 0.11*          |
|                  | Guanaco-7b       | 0.04           | 1.00*   | 0.50*          | 0.25          | 1.00* | 0.00*          |
|                  | LlaMa-2-7b-chat  | 0.08           | 0.87           | 0.72* | 0.35 | 0.26*          | 0.56*          |
|                  | LlaMa-2-13b-chat | 0.19* | 0.41*          | 0.66           | 0.31          | 0.04*          | 0.91* |
| CLEF-2018     | BioBERT          | 0.06           | 0.97*          | 0.59*          | 0.29          | 0.87*          | 0.19*          |
|                  | LlaMa-7b         | 0.05*          | 0.92           | 0.48*          | 0.25          | 0.33           | 0.04*          |
|                  | LlaMa-2-7b       | 0.07           | 0.49*          | 0.59*          | 0.22*         | 0.03*          | 0.69*          |
|                  | LlaMa-2-13b      | 0.05*          | 1.00*          | 0.50*          | 0.26          | 1.00* | 0.00*          |
|                  | Falcon-7b        | 0.05*          | 0.92           | 0.51*          | 0.25          | 0.40           | 0.11*          |
|                  | Alpaca-7b        | 0.05*          | 0.91           | 0.51*          | 0.25          | 0.30*          | 0.11*          |
|                  | Guanaco-7b       | 0.05*          | 1.00* | 0.50*          | 0.26          | 1.00* | 0.00*          |
|                  | LlaMa-2-7b-chat  | 0.09           | 0.88           | 0.75  | 0.37 | 0.27*          | 0.59           |
|                  | LlaMa-2-13b-chat | 0.26* | 0.36*          | 0.66*          | 0.30          | 0.00*          | 0.94* |
| CLEF-2019-dta | BioBERT          | 0.07           | 0.99*          | 0.58           | 0.30          | 0.88*          | 0.18           |
|                  | LlaMa-7b         | 0.07           | 0.93           | 0.48*          | 0.27          | 0.25           | 0.03*          |
|                  | LlaMa-2-7b       | 0.08           | 0.48*          | 0.58           | 0.23          | 0.00           | 0.68*          |
|                  | LlaMa-2-13b      | 0.07           | 1.00*          | 0.50*          | 0.28          | 1.00* | 0.00*          |
|                  | Falcon-7b        | 0.07           | 0.95           | 0.54*          | 0.29          | 0.50           | 0.12*          |
|                  | Alpaca-7b        | 0.07           | 0.91           | 0.52*          | 0.28          | 0.25           | 0.12*          |
|                  | Guanaco-7b       | 0.07           | 1.00* | 0.50*          | 0.28          | 1.00* | 0.00*          |
|                  | LlaMa-2-7b-chat  | 0.09           | 0.92           | 0.71  | 0.35 | 0.62           | 0.49           |
|                  | LlaMa-2-13b-chat | 0.19  | 0.49*          | 0.69           | 0.32          | 0.00           | 0.87* |
| CLEF-2019-Int | BioBERT          | 0.10           | 0.98*          | 0.58*          | 0.32          | 0.90*          | 0.16*          |
|                  | LlaMa-7b         | 0.05*          | 0.86           | 0.47*          | 0.26          | 0.30           | 0.08*          |
|                  | LlaMa-2-7b       | 0.08           | 0.30*          | 0.55*          | 0.18*         | 0.05*          | 0.80*          |
|                  | LlaMa-2-13b      | 0.05           | 1.00*          | 0.50*          | 0.29          | 0.97*          | 0.00*          |
|                  | Falcon-7b        | 0.05*          | 0.91           | 0.50*          | 0.27          | 0.57           | 0.09*          |
|                  | Alpaca-7b        | 0.05*          | 0.87           | 0.49*          | 0.27          | 0.30           | 0.12*          |
|                  | Guanaco-7b       | 0.05           | 1.00* | 0.50*          | 0.29          | 1.00* | 0.00*          |
|                  | LlaMa-2-7b-chat  | 0.08           | 0.90           | 0.70  | 0.35 | 0.42           | 0.48           |
|                  | LlaMa-2-13b-chat | 0.17* | 0.45*          | 0.67           | 0.33          | 0.05*          | 0.87* |

***Table 2. Calibrated results comparison when inclusion-exclusion criteria is used in the prompt (fused method unavilable due to inclusion-excllusion criteria contain too much token for BioBERT model),2-tailed t-test with bofferoni correction (p<0.05) is compred with Uncalibrated setting.***

| Dataset       | Model    | Setting    | P      | R      | B-AC   | F3     | Suc    | WSS    |
|---------------|----------|------------|--------|--------|--------|--------|--------|--------|
| CLEF-2017     | 7b-chat  | Unc        | 0.049  | 0.728  | 0.533  | 0.245  | 0.400  | 0.329  |
|               |          | Cal (0.95) | 0.060* | 0.921  | 0.671  | 0.300  | 0.500  | 0.410* |
|               |          | Cal (1)    | 0.050* | 0.981  | 0.613  | 0.270* | 0.925  | 0.239  |
|               | 13b-chat | Unc        | 0.193  | 0.270  | 0.518  | 0.228  | 0.000  | 0.755  |
|               |          | Cal (0.95) | 0.067* | 0.933* | 0.693  | 0.311* | 0.500* | 0.438  |
|               |          | Cal (1)    | 0.054* | 0.978  | 0.613  | 0.273* | 0.825* | 0.240  |
| CLEF-2018     | 7b-chat  | Unc        | 0.102  | 0.880  | 0.711  | 0.356  | 0.567  | 0.521  |
|               |          | Cal (0.95) | 0.106* | 0.885* | 0.731* | 0.368  | 0.500  | 0.555  |
|               |          | Cal (1)    | 0.065* | 0.975* | 0.623* | 0.311  | 0.900  | 0.258  |
|               | 13b-chat | Unc        | 0.333  | 0.362  | 0.666  | 0.321  | 0.000  | 0.958  |
|               |          | Cal (0.95) | 0.106  | 0.918* | 0.748  | 0.381  | 0.500* | 0.557* |
|               |          | Cal (1)    | 0.069  | 0.976  | 0.627* | 0.317  | 0.800* | 0.265* |
| CLEF-2019-dta | 7b-chat  | Unc        | 0.088  | 0.924  | 0.676  | 0.340  | 0.375  | 0.416  |
|               |          | Cal (0.95) | 0.087* | 0.928* | 0.664  | 0.323  | 0.500  | 0.388  |
|               |          | Cal (1)    | 0.082* | 0.958* | 0.626  | 0.312  | 0.625  | 0.283  |
|               | 13b-chat | Unc        | 0.226  | 0.427  | 0.661  | 0.301  | 0.000  | 0.880  |
|               |          | Cal (0.95) | 0.105  | 0.902  | 0.687  | 0.373  | 0.500* | 0.451* |
|               |          | Cal (1)    | 0.087* | 0.962  | 0.617  | 0.326  | 0.750* | 0.258* |
| CLEF-2019-Int | 7b-chat  | Unc        | 0.080  | 0.809  | 0.640  | 0.332  | 0.400  | 0.456  |
|               |          | Cal (0.95) | 0.074* | 0.921* | 0.652* | 0.335  | 0.486  | 0.369  |
|               |          | Cal (1)    | 0.068* | 0.956* | 0.625  | 0.327  | 0.649  | 0.282  |
|               | 13b-chat | Unc        | 0.243  | 0.485  | 0.662  | 0.367  | 0.075  | 0.821  |
|               |          | Cal (0.95) | 0.103* | 0.914  | 0.732  | 0.390  | 0.514* | 0.530* |
|               |          | Cal (1)    | 0.084* | 0.961  | 0.693  | 0.365  | 0.730* | 0.407* |
