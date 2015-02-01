# m! source code map

    src/
      embang/
        # Running inference and processing results
        core.clj       --- Running inference
        results.clj    --- Handling of inference results

        # Inference 
        ## General
        inference.clj  --- General inference functions
        state.clj      --- Particle state
        runtime.clj    --- Runtime support

        ## Algorithms
        importance.clj --- Importance sampling
        lmh.clj        --- Lightweight Metropolis-Hastings
        rdb.clj        --- Alias for lmh
        almh.clj       --- Adaptive Lightweight Metropolis-Hastings
        smc.clj        --- Particle Filter
        pgibbs.clj     --- Particle Gibbs
        siman.clj      --- MAP estimation via simulated annealing

        # Code transformations
        xlat.clj       --- Anglican to Clojure
        trap.clj       --- Clojure to CPS
        emit.clj       --- Compiling CPS 

      angsrc/
        # Anglican source code modules
        ## In particular: 
        dp_mem.clj     --- Implementation of DPmem
        crp.clj        --- Wrapped CRP for compatibility
                           with the original Anglican syntax