# Smart Crop Insurance using Corda

## Participants
1. Insurance Providers - Who provides the insurance to Farmers to protect their crops from natural calamities.
2. Govt Org/Agricultural Dept - Who approves the insurance products offered by different insurance providers.
3. Farmers - Who enrolls/purchase the insurance policy from different providers.

## Workflow
1. Insurance providers will create a insurance product which contains information about permium, for which crop and insuredAmount they will give to farmer in case of natural calamities.
2. Govt Org or Agriculatural dept or insurance board will approve that perticular product.
3. Now farmer can select that product as insurance policy.
4. Farmer can select products from different insurance providers considering their crop, permium and insuredAmount. That purchased policy contains information/conditions about what percentage of insured amount will be given to farmers in case of crop loss due to rain or drought.
5. **Oracle** will be used to decide rainy days and drought days. Using oracles information insured amount will be given to farmers and it will be automatically done using smart contract and using **Schedulable state** feature of corda.
6. In future, we will add AI to detect/decide the loss percentage. 

## Corda Concepts/features used for solution.
1. STATE, CONTRACT, FLOW
2. ORACLE
3. Reference state
4. Schedulable State
5. Queryable state

## States
1. Product state - Initially it would be Product proposal from Insurance providers and this proposal goes to the regulator(Govt/Agri Dept/Insurnace Board) and when they accepts it then it would become Insurance Product.
