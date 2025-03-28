body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #1a1a1a;
    color: #fff;
    margin: 0;
    padding: 0;
}

header {
    background: #ff9800;
    padding: 20px;
    font-size: 1.5em;
    color: black;
    animation: fadeIn 1.5s ease-in-out;
}

.book-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
    padding: 20px;
}

.book {
    background: #333;
    padding: 15px;
    border-radius: 10px;
    width: 250px;
    text-align: center;
    animation: slideUp 1s ease-in-out;
}

.upload {
    margin: 30px;
}

/* ✅ Responsive Design */
@media (max-width: 768px) {
    header {
        font-size: 1.2em;
        padding: 15px;
    }

    .book-list {
        flex-direction: column;
        align-items: center;
    }

    .book {
        width: 90%;
    }

    .upload {
        width: 100%;
        padding: 10px;
    }
}

.admin-controls {
    margin-top: 20px;
}

@keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
}

@keyframes slideUp {
    from { transform: translateY(20px); opacity: 0; }
    to { transform: translateY(0); opacity: 1; }
}
