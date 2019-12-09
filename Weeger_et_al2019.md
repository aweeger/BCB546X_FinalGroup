This project aims to replicate Figure 2a and 2e of Leininger, S., Adamski, M., Bergum, B. et al, 2014. This paper uses differential gene expretion analysis of developmental genes to investigate the relationship between sponges (specifically *Sycon ciliatum*) and eumetazoan body plans. 

Figure 2 provides a phylogenetic analysis based on the developmental genes identified as important earlier in the paper, as well as a heatmap of their expression based on different developmental stages and different locations in the adult body plan. 

### Here, we attempt to replicate these two segements of figure two, by using only the information provided in the methods. 

This proved to be a challenge, for multiple reasons. 

While obtaining the DNA data needed for the phylogenetic tree was easy, getting the RNA data for the heatmap was more challenging. The repository used to store the files did not have quick "all files" download option, which means that we needed to download each file individually. To do this, we wrote a small iterative script using the wget command, and iterating over each file name. Doing this, we also ran into the fact that these files are quite large (averaging 3G, over 66 files), something we had not considered when planning the analysis. 

Once we had the data, we also needed to perform multiple formatting steps that were not described in the methods, most likely because they are assumed to be common knowledge. Nontheless, as we formatted our DNA file for analysis on MrBayes, we were presented with mutiple different options to acheive our result. As a result, we cannot be sure that we followed the same steps that were performed in the paper, or that the Nexus file we generated for analysis is the same that was used in the paper. 

We also cannot be sure that we used the same parameters within MrBayes as were used in the paper, as they only stated that "Model parameters were estimated using the ProtTest3 package" to allow for an LG analysis. 
No further information was provided on how ProtTest3 was used, so we can only guess at best practice. 

Finally, no software version was provided in the paper, so while we assume that the most recent version was used (and therefore we were able to properly replicate this part) we cannot be sure. 

Overall, the method for the generation of phylogenetic trees seems extremely incomplete and poorly documented in this paper, as a lot of steps are implicitly assumed to be performed, and other do not contain enough details to guarentee replication. 

