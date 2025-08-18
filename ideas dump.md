## Ideas for what we might want to add for the ACCESS training day

I'm not going to prescribe a format for this document; if anyone else wants it to be formatted nicely they can go for it. I just can't be bothered.
The aim here is to put down a whole bunch of ideas that we can then sort through and build on my COSIMA training for the ACCESS NRI workshop. 
I'd really appreciate external input at this point so that we don't end up with a training that's just the things that have bothered me in the past.

* Examples are pretty much all COSIMA, I'd like to include a combination of CMIP datasets, intake stuff, open_mfdataset,
* In a perfect universe we'd find a way to have people bring their own data too? Are they likely to have datasets? 
I'm guessing if they've got some previous experience then they've got data that they're analysing suboptimally, so then it'd be good to have a 
chance to try fix that. Also, having examples applicable to one-self is always good. Failing that, I can ask around for some datasets that are ATMO/OCEAN/CM/LAND/ML.
* I'm wondering if we want to use everyone in the room as a parallel computer? I can't tell if this is a terrible idea or a brilliant idea, to start with a list of numbers we need
  to sum and distribute them as single numbers or as bigger piles. Maybe it works in small groups of 3-4?
* I think we want everyone to have 4 hours of 7 cores - enough to see that parallelisation is important, but few enought that you actually want to be smart about it
* I'm not sure how much more useful content is worth adding to the slides, so maybe we slow down a little bit along the way with everyone going through my notebooks not just me, 
and then we make the end freeform "try fix this code" or "try and improve your own code" depending on your propensity.
* xr.apply_ufunc needs to be more broadly updated, which means I need to learn how to use it better :)
* Try put Charles' cell magic to check for storage in there



## Additional examples of broken code
* Fishing out bottom age with a full 4D mask or a 2D index changes behaviour a lot


## Please put some more stuff in here! I'll go through the week of the 18th August and turn this brainstorm into an actual plan

## Paige's comments

### Slides

* For the "Why bother writing good code?" slide, perhaps we could add "Code less error prone". I'm thinking specifically about using Xarray and how its labeled dimensions, etc. make writing code less prone to human error.
* Maybe we could add a bit more on chunking before diving into the "Black magic of chunking" slide (eg the human parallel computer idea!)
* It might be nice to have a bit more "stage setting" at the start - eg a quick reminder intro of what Xarray and Dask are
* Maybe this is just me being too used to Xarray and Dask, but it's not entirely clear to me what is being "rethought" in the 4 coding examples. Perhaps I should rewatch the recording of your COSIMA training... :)

### Notebooks/code examples

* It might be nice to have some examples or exercises that help participants to understand how Dask works on Gadi specifically. During the COSIMA training, there were a few times when you mentioned that it's often best to include specific flags in Gadi workflows, so maybe some examples that could show how/why some of those tips and tricks work could be useful.
* Possibly related to the previous comment, maybe we could give an exercise using Dask that will crash the kernel and use that as a learning moment (either demonstrate why that happened or have them try to fix it)
* It is always nice to have an example that shows a calculation where Dask makes things faster - maybe we could add one of those? We could also find one where Dask makes the calculation run slower to show that it's not always helpful in every situation.
* Not sure if this was the plan, but I think it would be useful to have some coding exercises associated with the examples shown in the slides. This would make the session a bit more hands-on.

### Overall comments
* I like the idea of people bringing their own data that they've had trouble with, but we'd probably need to do some planning to make sure that it can be pulled off and actually useful for everyone. For instance, I could imagine people coming with their own data, but then it takes them time to figure out how to read it in or the trouble they had with their data has nothing to do with Xarray and Dask even if they thought it did. So anyway, we'd likely want to have some specific instructions for what types of data and data troubles people should bring in if we go this way. Also, we would want to make sure that it doesn't just become a help session for those that brought their own data - or maybe this would be a good thing?
* We should probably point participants at the end toward resources where they can learn more about Xarray/Dask (eg the docs pages) and ask for help (the Hive Forum). Maybe it would also be nice to point them to some specific COSIMA recipes that demonstrate various uses of Xarray and Dask on Gadi?
