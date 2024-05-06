digraph G {
    node [shape=plaintext]

    // Ciencia y Tecnología
    Ciencia -> Tecnología [label="se aplica en", fontsize=10]
    Tecnología -> Ciencia [label="se basa en", fontsize=10]

    // Ciencia y Conocimiento
    Ciencia -> Conocimiento [label="genera", fontsize=10]
    Conocimiento -> Ciencia [label="se adquiere a través de", fontsize=10]

    // Tecnología y Conocimiento
    Tecnología -> Conocimiento [label="emplea", fontsize=10]
    Conocimiento -> Tecnología [label="provee", fontsize=10]

    // Definiciones
    subgraph cluster_definiciones {
        label = "Definiciones"
        style = rounded
        color = lightgrey
        fontcolor = black
        fontsize = 12

        Ciencia [label="Ciencia:\nConjunto de conocimientos sistemáticos y comprobables\n", fontsize=10, shape=box]
        Tecnología [label="Tecnología:\nSuma de técnicas, habilidades y métodos\n", fontsize=10, shape=box]
        Conocimiento [label="Conocimiento:\nAcción de adquirir información valiosa\n", fontsize=10, shape=box]
    }
}

