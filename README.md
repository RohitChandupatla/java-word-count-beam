# java-word-count-beam by Rohit Reddy Chandupatla


### Use the following command to generate a Maven project that contains Beam’s WordCount examples and builds against the most recent Beam release:

```
mvn archetype:generate `
 -D archetypeGroupId=org.apache.beam `
 -D archetypeArtifactId=beam-sdks-java-maven-archetypes-examples `
 -D archetypeVersion=2.36.0 `
 -D groupId=org.example `
 -D artifactId=word-count-beam `
 -D version="0.1" `
 -D package=org.apache.beam.examples `
 -D interactiveMode=false

```
### Get sample text

In the word-count-beam directory, create a file called [sample.txt.](https://github.com/RohitChandupatla/python-word-count-beam/blob/main/sample.txt)
Add some text to the file. For this example, you can use the text of Shakespeare’s [Sonnets](https://00f74ba44b0dc016a7c9b360b480054ed0a128d336-apidata.googleusercontent.com/download/storage/v1/b/apache-beam-samples/o/shakespeare%2Fsonnets.txt?jk=AFshE3WcHn94BgMO_Xbvah8Gaebzpd3aqoZhIupaAjP7igbZSAik_ve5UWZBup0ZUTWK-GlaEKnKk0Tg9p45Twgw_MxRb7ftv7qPUcqTCG2s3J5KHE0kfMzK56RMkA_zXYafTIEMD7tL1d5ZAtBjCuZgfWsqObCLTQ_wR8kbvzoWckI4NR7-MOd98NGm7Gc7kGxxly2hkhgQqMC7knsmUpZMN-2g0hq_Eq3pD-y7idpZUaBo3CWvhbZzEuTcgDBPu42ISG_ap4D4DkFMKOwLsyB6Ghsb3f9x_fmaGBPeaNZHUJFXDmxgbYcx292vd_IedfvPgoXFE0to0twNGGMKHPIfUKpbMPiT54Qc5WiICPAmInGQQfQBYiWA6MLzOFUhcac_NaoDWPiy8Nxk7zismifs2jNIh3sa5bwvPhb1oXIfEcdVBjYFXe8U-cHniPHrRhNKSWxPTApa7Gjwl-VFdTntCU2jlzQY-3F1j_BZyzRATpT9gaqHgpWFk36myx6O9cqFh75BQDXgu1oHg9WdrRTsB0CmPn7cO2sA-ejmWGmpSx-2_dXsQTCQRzo03WFw8RuR-hjgqr8PcCAUByW4Ibyu1tkgDvXjNCScIyiDl8bO8shK6AmjB_X7Vuwef-LohcUrzPgmKOEbiisDCBiSNgaIR97j-X0BLdNQmsHzYghwNi387fEG06uGD0FH-zb5twjs9B7Gs5e9MOhA3ziZPWsS6Mqai-php9EPAWc0hC_graYrYHErPlqYKVDeKVblw2WRzzFY8cHrO2HSwaIh2ss2Nx0_WZn_Qc4JLDIPAEFQJssOySZq9TjFugx-BuPaVJ73UZsS59AxTiG27o9krLYic3m7N4BNQq1XmbxoqUMq9uVieKMEwLHwnOMx1Ir_aacYRBje2zcuOgb2_vd_pN8TjygoHjd0OyGVW4Y9a3-jQ3Cu6KfShppLM5tfq0hmpCovTkrLz8vUisqyY5uWrbd2sJ_R1aA&isca=1).

### Run WordCount Using Maven For Windows PowerShell:
```
mvn compile exec:java -D exec.mainClass=org.apache.beam.examples.WordCount `
 -D exec.args="--inputFile=sample.txt --output=counts" -P direct-runner
``` 
