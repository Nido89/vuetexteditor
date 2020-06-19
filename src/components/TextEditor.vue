<template>
<div id="bodyTxt">
        <h3>Text-Writer-Editor</h3>
            <editor 
            v-model="editorText" 
            height="350px"
            mode="wysiwg"
            previewStyle="vertical"
            />
        
        <h3>Text-Viewer-Highlighter-Selector</h3>
      
        <viewer :value="editorText"/>
    </div>

</template>

<script>
import 'tui-editor/dist/tui-editor.css'
import 'tui-editor/dist/tui-editor-contents.css'
import 'codemirror/lib/codemirror.css'
import 'highlight.js/styles/github.css'
import { Editor,Viewer } from '@toast-ui/vue-editor'

export default {
    name:'TextEditor',
    data (){
        return {
            editorText:''
            }

    },
    
    components: {
        'editor':Editor,
        'viewer':Viewer
    }
}
</script>

<style>

</style>>

