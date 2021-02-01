<script lang="ts">
    export let input: string;
    export let length: number;
    export let result: string;
</script>

<usage>
    <h3>Getting started</h3>
    <p>Install it using NPM: </p>
    <pre>
        <code>
npm i hemoji
        </code>
    </pre>
    <p>Import it and use it!</p>
    <pre>
        <code>
<span class="keyword">import</span> hemoji <span class="keyword">from</span> <span class="string">'hemoji'</span>;

{#if length === 6}
hemoji(<span class="string">'{input}</span>'); <span class="comment">// {result}</span>
{:else}
hemoji(<span class="string">'{input}'</span>, &lbrace; length: <span class="number">{length}</span> &rbrace;); <span class="comment">// {result}</span>
{/if}
        </code>
    </pre>
    <p>More information and source code on Github at <a href="https://github.com/keraf/hemoji">keraf/hemoji</a>.</p>
</usage>

<style>
    usage {
        width: 100%;
        min-width: 350px;
        max-width: 460px;
    }

    code {
        display: block;
        padding: 1em;
        border-radius: 5px;
        background-color: #1e1e1e;
        color: #d4d4d4;
        overflow-x: auto;
    }

    .comment {
        color: #5e9548;
    }

    .string {
        color: #b28d61;
    }

    .number {
        color: #8acea8;
    }

    .keyword {
        color: #469cd6;
    }
</style>