##Welcome to Github pages 
Markdown is an easy-to-use tool for styling your writing. 

Here's the JSON data:

<div id="json-data"></div>

<script>
fetch('resorts.json')
  .then(response => response.json())
  .then(data => {
    const jsonData = JSON.stringify(data, null, 2);
    document.getElementById('json-data').textContent = jsonData;
  })
  .catch(error => {
    console.error('Failed to load JSON:', error);
  });
</script>

