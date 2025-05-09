<script lang="ts">
    import type { Meal } from '$lib/types';
    export let meal: Meal;
</script>

<div class="food-card">
    <h2>{meal.name}</h2>
    <p>Type: {meal.dish_type}</p>
    <ul>
        {#each meal.labels as label}
            <li>{label}</li>
        {/each}
    </ul>
</div>