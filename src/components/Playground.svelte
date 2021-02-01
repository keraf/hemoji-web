<script lang="ts">	
	export let input: string;
    export let length: number;
    export let result: string;
</script>

<playground>
    <span class="result">{result}</span>
    <input bind:value={input} placeholder="Type or paste some text here">
    <input type="range" bind:value={length} min="1" max="32">
    <span class="length">Length: {length}</span>
</playground>

<style>
	playground {
        margin: 20px 0;
        max-width: 420px;
		display: flex;
        flex-direction: column;
        align-items: center;
    }

    .result {
        overflow-wrap: break-word;
        font-size: 1.2em;
        margin: 1rem;
    }
    
    .length {
        margin-top: -15px;
    }
</style>