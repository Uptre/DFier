# DFier
A directed fuzzer for Ethereum smart contracts
 # Code Structure Descriptions
   Some details about the repository structure as following:  
   <ul>
<li>  <code>countSubTreesCpp.zip</code> includes the implementations of the sub-paths counting tool in section 4.2.2 of the paper. </li>
<li>  <code>DFierSFuzz.zip</code> is used to directly fuzzing the testing smart contracts with given target lines, which is implemented based on sFuzz[1]. </li>
<li>  <code>Datasets</code>  includes all experimental datasets. Specifically,
          <ul>
          <li> <code>contractfuzzer_DataSet.zip</code> is the ground-truth dataset provided by contractFuzzer[2].    </li>  
         <li> <code>etherscanDataset.zip</code> includes the contracts downloaded from the etherscan website[3], a blockchain explorer.  </li>  
          <li> <code>OsirisResultsOnEtherscanData.zip</code> includes the Osiris detection results on <code>etherscanDataset.zip</code>.  By using Osiris[4], an integer vulnerabilities detection tool, the target potential vulnerable lines are given. </li>    
        </ul>
      </li>
    </ul>

# The operation instructions of DFier System
   <ul>
   <li>Prepare the data for the system: in the DFierSFuzz/contracts, put the testing contract including the source codes (.sol file) and the path constraint file (.json file). Several examples are put in the directory.</li>  
    <li> Launch the system: go to the directory: DFierSFuzz/build/fuzzer, execute the command: ./fuzzer -g -r 0 -d 120 && chmod +x fuzzMe && ./fuzzMe</li>  
   </ul>

    
 # References
  [1] Nguyen T D , Pham L H , Sun J ,et al.sFuzz: An Efficient Adaptive Fuzzer for Solidity Smart Contracts[C]//ICSE '20: 42nd International Conference on Software Engineering.2020.DOI:10.1145/3377811.3380334. 
  
  [2] Bo Jiang, Ye Liu, and W. K. Chan. 2018. ContractFuzzer: fuzzing smart contracts for vulnerability detection. In Proceedings of the 33rd ACM/IEEE International Conference on Automated Software Engineering (ASE '18), 2018, pp.259–269. 

  [3]Etherscan, the Ethereum Blockchain Explorer. https://goto.etherscan.com/.
  
  [4] Torres, C. F., Schütte, J., & State, R. Osiris: Hunting for integer bugs in ethereum smart contracts. In Proceedings of the 34th Annual Computer Security Applications Conference, 2018, pp. 664-676.  
