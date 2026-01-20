<script>
// VIDEO
function bukaVideo(file) {
    let url = URL.createObjectURL(file);
    video.src = url;
    videoLink.href = url;
    videoLink.innerText = "Buka: " + file.name;
}

// FOTO
function bukaFoto(file) {
    let url = URL.createObjectURL(file);
    foto.src = url;
    fotoLink.href = url;
    fotoLink.innerText = "Buka: " + file.name;
}

// FILE
function bukaFile(file) {
    let url = URL.createObjectURL(file);
    fileLink.href = url;
    fileLink.innerText = "Buka: " + file.name;

    filePreview.src = "";

    if (file.type === "application/pdf") {
        filePreview.src = url;
    } 
    else if (
        file.name.endsWith(".docx") ||
        file.name.endsWith(".pptx") ||
        file.name.endsWith(".xlsx")
    ) {
        filePreview.src =
          "https://docs.google.com/gview?url=" + url + "&embedded=true";
    } 
    else {
        filePreview.srcdoc = "Preview tidak tersedia.<br>Gunakan tombol Buka File.";
    }
}
</script>