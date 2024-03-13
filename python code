<!DOCTYPE html>
<html>
<head>
    <title>Image to Text and Translation</title>
</head>
<body>
    <h1>TEXT RECOGNIZER AND TRANSLATOR</h1>

    <form method="POST" enctype="multipart/form-data">
        <input type="file" name="image" accept="image/*" required>
        <button type="submit">Extract Text and Translate</button>
    </form>

    {% if extracted_text %}
        <div>
            <h2>Extracted Text:</h2>
            <p>{{ extracted_text }}</p>
        </div>
    {% endif %}

    {% if translated_text %}
        <div>
            <h2>Translated Text:</h2>
            <p>{{ translated_text }}</p>
            {% if audio_path %}
                <audio controls>
                    <source src="{{ audio_path }}" type="audio/mpeg">
                    Your browser does not support the audio element.
                </audio>
            {% endif %}
        </div>
    {% endif %}
</body>
</html>
