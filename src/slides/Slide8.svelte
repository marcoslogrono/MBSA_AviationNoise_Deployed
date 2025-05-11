<script>
    // export let active = false;
    import {observerStore} from '../lib/panelComponents/Scrolly_slide';

    // export let value;
    let isVisible = false;

    const unsubscribe = observerStore.subscribe(store => {
        isVisible = store.isVisible;
    });

</script>

<div class="slide">
    <h1>References & Acknowledgements</h1>
    
    <div class="references">
        <h3>References</h3>
        <ul class="reference-list">
            <li>
                <span class="reference-number">[1]</span> 
                Massport. (2025, January). <i>Airport Traffic Summary</i>. Retrieved from 
                <a href="https://www.massport.com/sites/default/files/2025-02/0125-avstats-airport-traffic-summary.pdf" target="_blank">
                    https://www.massport.com/sites/default/files/2025-02/0125-avstats-airport-traffic-summary.pdf
                </a>
            </li>
            <li>
                <span class="reference-number">[2]</span>
                Smith, M. G., Cordoza, M. , and Basner, M (2022). 
                <i>Environmental Noise and Effects on Sleep: An Update to the WHO Systematic Review and Meta-Analysis</i>. 
                National Library of Medicine. Retrieved from 
                <a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9272916/" target="_blank">
                    https://pmc.ncbi.nlm.nih.gov/articles/PMC9272916/
                </a>
            </li>
            <li>
                <span class="reference-number">[3]</span>
                Yale Environmental Health & Safety. (2023). <i>Decibel Level Comparison Chart</i>. Retrieved from 
                <a href="https://ehs.yale.edu/sites/default/files/files/decibel-level-chart.pdf" target="_blank">
                    https://ehs.yale.edu/sites/default/files/files/decibel-level-chart.pdf
                </a>
            </li>
        </ul>
    </div>

    <div class="acknowledgements">
        <h3>Acknowledgements</h3>
        </div>
</div>

<style>
    @import url("$lib/slide.css");
    @import url("$lib/arrow.css");

    .slide {
        padding-bottom: 3rem;
    }

    .references, .acknowledgements {
        margin-bottom: 2rem;
    }

    .reference-list {
        list-style-type: none;
        padding-left: 0;
    }

    .reference-list li {
        margin-bottom: 1rem;
        padding-left: 2.5rem;
        text-indent: -2.5rem;
        font-size: 0.9rem;
        line-height: 1.4;
    }

    .reference-number {
        font-weight: bold;
        margin-right: 0.5rem;
    }

    h3 {
        margin-bottom: 0.75rem;
        font-size: 1.3rem;
        color: #444;
        border-bottom: 1px solid #ddd;
        padding-bottom: 0.5rem;
    }

    a {
        color: #1976d2;
        text-decoration: none;
        word-break: break-all;
    }

    a:hover {
        text-decoration: underline;
    }
</style>
