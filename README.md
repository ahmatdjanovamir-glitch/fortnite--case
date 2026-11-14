# fortnite--case

/* ЗОЛОТОЙ ЖЕТОН FORTNITE */
.token {
    color: #ffd700;
    font-size: 70px;
    text-shadow:
        0 0 10px gold,
        0 0 25px orange,
        0 0 45px yellow;
    animation: goldenGlow 1s infinite alternate;
}

@keyframes goldenGlow {
    from {
        transform: scale(1);
        filter: brightness(1);
    }

    to {
        transform: scale(1.2);
        filter: brightness(1.6);
    }
}

.case {
    transition: transform 0.3s, box-shadow 0.3s;
}

.case:hover {
    transform: scale(1.08) rotate(-2deg);
    box-shadow: 0 0 25px #00bfff;
}

.item {
    animation: itemAppear 0.8s ease;
}

@keyframes itemAppear {
    0% {
        transform: scale(0) rotate(360deg);
        opacity: 0;
    }

    100% {
        transform: scale(1) rotate(0);
        opacity: 1;
    }
}
