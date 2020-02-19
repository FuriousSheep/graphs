# Graph

```graphviz
digraph {
    <!-- label = "This is the title"
    labelloc = "t"

    D [shape=record label="{This is D|{A|B|C}}|{D|E}"]
    A [shape=circle]
    B [shape=record]
    C [shape=record]


    A -> B [label = "Une capacité\nde A sur B"]
    A -> B [label = "Une autre capacité\n de A sur B"]
    B -> C [label = "Capacité de B sur C"] -->
    ############################################################"

    subgraph cluster_p {
        label = "Parent";

        subgraph cluster_c1 {
            label = "Child one";
            a;

            subgraph cluster_gc_1 {
                label = "Grand-Child one";
                b;
            }

            subgraph cluster_gc_2 {
                label = "Grand-Child two";
                c;
                d;
            }
        }

        subgraph cluster_c2 {
            label = "Child two";
            e;
        }
    }

    subgraph cluster_name {
        label = "Name";
        name;

        subgraph test_1 {
            label= "Test 1";
            test_1;
        }

        subgraph test_2 {
            label = "Test 2";
            test_2;

            subgraph test_21 {
                label = "Test 21";
                test_21;
            }
        }
    }
}
```