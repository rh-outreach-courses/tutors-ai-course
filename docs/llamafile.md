# Running a llamafile to help with coding

One of the simplest ways to run an LLM locally is using a [llamafile](https://github.com/Mozilla-Ocho/llamafile). 
llamafiles bundle model weights and a specially-compiled version of llama.cpp into a single file that can run on most computers any additional dependencies. 
They also come with an embedded inference server that provides an API for interacting with your model.

Continue is the leading open-source AI code assistant. You can connect any models and any context to build custom autocomplete and chat experiences inside VS Code

This exercise guides you through running a llamafile and connecting to it from vscode.

## Running a llamafile


1. Download [llava-v1.5-7b-q4.llamafile](https://huggingface.co/Mozilla/llava-v1.5-7b-llamafile/resolve/main/llava-v1.5-7b-q4.llamafile?download=true) (4.29 GB).

2. Open your computer's terminal.

3. If you're using macOS, Linux, or BSD, you'll need to grant permission
for your computer to execute this new file. (You only need to do this
once.)

```sh
chmod +x llava-v1.5-7b-q4.llamafile
```

4. If you're on Windows, rename the file by adding ".exe" on the end.

5. Run the llamafile. e.g.:

```sh
./llava-v1.5-7b-q4.llamafile
```

6. Your browser should open automatically and display a chat interface.
(If it doesn't, just open your browser and point it at http://localhost:8080)

7. When you're done chatting, return to your terminal and hit
`Control-C` to shut down llamafile.


## Using Continue in VS Code

1. Click `Install` on the [Continue extension page in the Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=Continue.continue)
2. This will open the Continue extension page in VS Code, where you will need to click `Install` again
3. The Continue logo will appear on the left sidebar. For a better experience, move Continue to the right sidebar

You can now use Continue with ChatGPT, but we want to configure it to use the local llamafile LLM.

# Configuring Continue

1. Click the "gear" icon in the bottom right corner of the Continue Chat sidebar. 

2. Add configuration so that Continue uses your local llamafile LLM:

```
 "models": [
    {
      "title": "Llama CPP",
      "provider": "llama.cpp",
      "model": "llava-v1.5-7b-q4",
      "apiBase": "http://localhost:8080"
    }
  ],

```

3. Save the file.
When you save `config.json`, Continue will automatically refresh to take into account your changes.