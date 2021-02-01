<info>
    <h3>What is Hemoji?</h3>
    <p>Hemoji is a small single function JavaScript/TypeScript library that hashes a string into a sequence of emojis. Just like hashes, two identical strings passed through Hemoji will produce the same result.</p>
    <h3>But why?</h3>
    <p>This library is not intended to replace traditional hashing functions as collision are more likely. But as it provides more possibilities than alphanumeric characters for its length, it makes it a more convenient method to compare two pieces of information where it would not be possible, practical or secure to do so programmatically. Examples would include oral confirmation between two people or self confirmation in separate contexts, i.e., across separate devices.</p>
</info>

<style>
    info {
        display: flex;
        flex-direction: column;
        max-width: 460px;
    }
</style>