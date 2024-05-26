# DFier
A directed fuzzer for Ethereum smart contracts
 # Code Structure Descriptions
   Some details about the repository structure as following:  
   <ul>
 includes the patch generation system <code>Aroc</code>.  </li>
<li>  <code>countSubTreesCpp.zip</code> includes the implementations of the sub-paths counting system in section 4.2.2. </li>
<li>  <code>DFierSFuzz.zip</code> is used to directly fuzzing the testing smart contracts with given target lines. </li>
<li>  <code>Datasets</code>  includes all experimental datasets. Specifically,
          <ul>
          <li> <code>contractfuzzer_DataSet.zip</code> is the ground-truth dataset provided by contractFuzzer[1].    </li>  
         <li> <code>etherscanDataset.zip</code> includes the contracts downloaded from the etherscan website, a blockchain explorer.  </li>  
          <li> <code>OsirisResultsOnEtherscanData.zip</code> includes the Osiris detection results on <code>etherscanDataset.zip</code>.  By using Osiris, the target potential vulnerable lines are given. </li>    
        </ul>
      </li>
    </ul>
    
    
 # References
  [1] Rodler, M., Li, W., Karame, G. O., & Davi, L. (2021). EVMPatch: timely and automated patching of ethereum smart contracts. In 30th {USENIX} Security Symposium ({USENIX} Security 21).  
  [2] Torres, C. F., Schütte, J., & State, R. (2018, December). Osiris: Hunting for integer bugs in ethereum smart contracts. In Proceedings of the 34th Annual Computer Security Applications Conference (pp. 664-676).  
  [3] Nguyen T D , Pham L H , Sun J ,et al.sFuzz: An Efficient Adaptive Fuzzer for Solidity Smart Contracts[C]//ICSE '20: 42nd International Conference on Software Engineering.2020.DOI:10.1145/3377811.3380334. 
