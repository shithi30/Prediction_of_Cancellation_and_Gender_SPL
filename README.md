*Note: Links may not redirect outside org. Some data may be hidden due to policy.*

## Completion Analysis: Which orders will get canceled?

<img width="570" alt="fl1" src="https://github.com/shithi30/Sheba_Predictions--Cancels_Gender/assets/43873081/e934ce97-d625-4609-b24c-a7c3c408f15b"><br>

Sheba Platform Limited (SPL) was able to reduce cancellation of service-orders by leveraging the results of an ML model twice a day. I use data of last 4 months' to form the training set (for the sake of recency) and prepare a store of 22 features containing:

- <strong>Customer Info</strong>
  - How long has the customer been with Sheba Platform?
  - When was his/her last order?
  - How many orders has the customer placed so far?
  - How many services has the customer received so far?
  - How many complaints did the customer lodge so far?
  - Customer's avg. satisfaction (CSAT) score 
  - Customer's avg. satisfaction (CSAT) count
  - How many times did the customer reschedule?
  - What GMV has the customer caused to SPL so far?
- <strong>Order Info</strong>
  - When was the order placed?
  - When is the order to be served?
  - Delay between order and service
  - How many times did the SP got changed?
  - How many times did the order get rescheduled?
  - Is there any promotional activity?
  - Is there a discount?
- <strong>Service Provider (SP) Info:</strong> Which SP got assigned?
- <strong>System Info</strong>
    - SBU, Master category, Service category, location of the order
    - Which channel landed the order?

Past records help me label if the order got canceled or not (0/1). This a binary classification problem is formed and training renders ~85% accurate results on test-set. DSAI & CX operationalized the findings the following way:

#### During the Day
- Train: http://mb.sheba.xyz/question/14853
- Test: http://mb.sheba.xyz/question/16702
- Daily prospective cancels: http://mb.sheba.xyz/question/16708?st=risky&dt=2020-06-24
- Tracking daily prospective cancels: http://mb.sheba.xyz/question/16744?dt=2020-06-23

#### End of Day
- MX and CX | Daily Health Report: http://mb.sheba.xyz/question/13109?target=5600
- Prediction performance: https://docs.google.com/spreadsheets/d/1BChwHjBSPakqboYORU4Ukd1bhltUoff1thDjB1G9_oI/edit#gid=0
- CX followup: https://docs.google.com/spreadsheets/d/1rt68jnf4LPONOY4Raq5M5K-jUQJKUXrxrGTTfDvxmuk/edit#gid=2019316536

## Identification of Gender from Names
<p align="center">
<img width="520" alt="fl1" src="https://github.com/shithi30/Sheba_Predictions--Cancels_Gender/assets/43873081/63365c45-12c1-45f5-bb52-9c8b4b89910c">
<img width="317" alt="fl1" src="https://github.com/shithi30/Sheba_Predictions--Cancels_Gender/assets/43873081/69771ee6-26cf-4c60-bf1b-f6abc9e588fd">
<br>
</p>

