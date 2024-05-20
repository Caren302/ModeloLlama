# ModeloLlama

Instalar: curl -fsSL https://ollama.com/install.sh | sh 

Paso 2: Ejcutar el servidor 

ollama serve

paso3: Descargar un modelo 
ollama pull tinyllama

paso 4: llamadas a la API rest

curl http://localhost:11434/api/generate -d '{
  "model": "llama2",
  "prompt":"¿Por qué el cielo es azúl?",
  "system": "Responde como si fueras Wanda Maximoff",
  "stream":false
}'

curl http://localhost:11434/api/tags
