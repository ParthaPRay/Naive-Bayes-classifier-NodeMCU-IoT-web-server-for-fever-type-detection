# Naive-Bayes-classifier-NodeMCU-IoT-web-server-for-fever-type-detection

This study presents a novel NodeMCU based web server to validate cost-effective and smart e-health
diagnosis. Proposed work implements a novel Naïve Bayes Classifier for automatic fever type detection
as a proof of concept. The application is currently accessible on local network. Network users (patients)
are first required to submit eight symptoms e.g. “fatigue”, “fever”, “chills”, “sore throat”, “cough”,
“headache”, “muscle pain”, and “sneezing” on web portal in form of yes “y” or no “n”. Implied Naïve
Bayes Classifier engine predicts the probability of occurrence of fever either from flu or common cold as
per symptoms provided earlier. The patients are simultaneously diagnosed by a medical practitioner
from whom patient wise predictive percentage was received. The probabilistic values were then paired
against flu and common cold typed fever patients independently. 22 patients were voluntarily gone
through this experiment where p (0.089>0.05) and p (0.068>0.05) were not found to be statistically
significant (i.e. no difference between proposed classifier and doctor’s diagnosis) for flu and common
cold fever types, respectively.

![Untitled](https://user-images.githubusercontent.com/1689639/162980850-a532acc5-263f-4da3-83fc-eab1c1e94df1.png)

This study involves two main components such as (1)
NodeMCU; (2) PC. As stated earlier, NodeMCU is a 5 USD
hardware platform to facilitate user’s query over IEEE 802.11
b/g/n Wi-Fi connectivity. Thus, it has promising nature to act
as the resource-constrained network gateway. Besides that, it
comprises of an L106 32-bit RISC microprocessor core
running at 80 MHz clock frequency. Further, 16 GPIO pins,
SPI, I2C, I2S, UART, and 10-bit ADC are also integrated with
it. Moreover, the Lua-scripting firmware provides descent
flexibility over programing and debugging instructions.
Subsequently, a Dell Inspiron model with 8 GB RAM, 1 TB
HDD is used to burn the algorithm into the USB powered User provides 8 health status indicator values in yes (“y”) or no
(“n”) text valued form via HTTP/Post to the web server. Upon
successful reception of user’s symptom related information,
NBC engine performs a supervised learning technique to
retrieve appropriate type of fever (i.e. common cold or flu).
The diagnosed results are then forwarded to the user via
HTTP/Get method call.
