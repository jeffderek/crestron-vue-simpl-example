# crestron-vue-simpl-example
```mermaid
flowchart LR;
    counter[Counter Mutations] & display[Display Mutations] & other[Other Mutations]-->vuex((Vuex));
    vuex((Vuex))-->|processMutations|processor[Crestron Processor]
    processor[Crestron Processor]-->|processFeedback|vuex((Vuex))
    processor[Crestron Processor]-->counter2[Counter Device Controls] & display2[Display Device Controls] & other2[Other Device Controls]
 ```
