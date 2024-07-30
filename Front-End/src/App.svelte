<script>
    import Form from "./lib/Form.svelte"
    import ResumePreview from "./lib/ResumePreview.svelte";
</script>
<body>
    <div class="grid-container">
        <header>
            title
        </header>
        <div class="form-div">
            <Form/>
        </div>
        <div class="preview-div">
            <ResumePreview/>
        </div>
        <footer>
            credits
        </footer>
    </div>

</body>
<style>
    .grid-container{
        display: grid;
        grid-template-areas: 
            'header header'
            'form preview'
            'footer footer';
    }
    .form-div{
        grid-area: form;
        height: 1000px;
        
        border-right: 1px solid rgb(26, 26, 26);
        text-align: center;
        background-color: aqua;
    }
    .preview-div{
        grid-area: preview;
        text-align: center;
        background-color: rgb(46, 46, 46);
    }
    header{
        grid-area: header;
        background-color: black;
        color: white;
        text-align: center;
        height: 50px;
    }
    footer{
        grid-area: footer;
        background-color: black;
        color: white;
        text-align: center;
        height: 50px;
    }
    
</style>