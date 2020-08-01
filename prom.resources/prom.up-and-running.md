
## Prometheus, 
    - The metrics-based monitoring system used by tens of thousands of organizations in production. 
    - application developers, sysadmins, and DevOps practitioners with a hands-on introduction to the most important aspects of Prometheus, 
    - including dashboarding and alerting, direct code instrumentation, and metric collection from third-party systems with exporters.

    - Prometheus does one thing, and it does it well. 
    - Prometheus setup, the Node exporter, and the Alertmanager, then demonstrates how to use them for application and infrastructure monitoring.

    - Know where and how much to apply instrumentation to your application code
    - Identify metrics with labels using unique key-value pairs
    - Get an introduction to Grafana, a popular tool for building dashboards
    - Learn how to use the Node Exporter to monitor your infrastructure
    - Use service discovery to provide different views of your machines and services
    - Use Prometheus with Kubernetes and examine exporters you can use with containers
    - Convert data from other monitoring systems into the Prometheus format


I. Introduction
                1. What Is Prometheus?
                            What Is Monitoring?
                            A Brief and Incomplete History of Monitoring
                            Categories of Monitoring
                            Prometheus Architecture
                            Client Libraries
                            Exporters
                            Service Discovery
                            Scraping
                            Storage
                            Dashboards
                            Recording Rules and Alerts
                            Alert Management
                            Long-Term Storage
                            What Prometheus Is Not
                2. Getting Started with Prometheus
                            Running Prometheus
                            Using the Expression Browser
                            Running the Node Exporter
                            Alerting


II. Application Monitoring
                3. Instrumentation
                            A Simple Program
                            The Counter
                            Counting Exceptions
                            Counting Size
                            The Gauge
                            Using Gauges
                            Callbacks
                            The Summary
                            The Histogram
                            Buckets
                            Unit Testing Instrumentation
                            Approaching Instrumentation
                            What Should I Instrument?
                            How Much Should I Instrument?
                            What Should I Name My Metrics?
                4. Exposition
                            Python
                            WSGI
                            Twisted
                            Multiprocess with Gunicorn
                            Go
                            Java
                            HTTPServer
                            Servlet
                            Pushgateway
                            Bridges
                            Parsers
                            Exposition Format
                            Metric Types
                            Labels
                            Escaping
                            Timestamps
                            check metrics
                5. Labels
                            What Are Labels?
                            Instrumentation and Target Labels
                            Instrumentation
                            Metric
                            Multiple Labels
                            Child
                            Aggregating
                            Label Patterns
                            Enum
                            Info
                            When to Use Labels
                            Cardinality
                6. Dashboarding with Grafana
                            Installation
                            Data Source
                            Dashboards and Panels
                            Avoiding the Wall of Graphs
                            Graph Panel
                            Time Controls
                            Singlestat Panel
                            Table Panel
                            Template Variables


III. Infrastructure Monitoring
                7. Node Exporter
                            CPU Collector
                            Filesystem Collector
                            Diskstats Collector
                            Netdev Collector
                            Meminfo Collector
                            Hwmon Collector
                            Stat Collector
                            Uname Collector
                            Loadavg Collector
                            Textfile Collector
                            Using the Textfile Collector
                            Timestamps

                8. Service Discovery
                            Service Discovery Mechanisms
                            Static
                            File
                            Consul
                            EC2
                            Relabelling
                            Choosing What to Scrape
                            Target Labels
                            How to Scrape
                            metric_relabel_configs
                            Label Clashes and honor_labels

                9. Containers and Kubernetes
                            cAdvisor
                            CPU
                            Memory
                            Labels
                            Kubernetes
                            Running in Kubernetes
                            Service Discovery
                            kube-state-metrics

                10. Common Exporters
                            Consul
                            HAProxy
                            Grok Exporter
                            Blackbox
                            ICMP
                            TCP
                            HTTP
                            DNS
                            Prometheus Configuration

                11. Working with Other Monitoring Systems
                            Other Monitoring Systems
                            InfluxDB
                            StatsD

                12. Writing Exporters
                            Consul Telemetry
                            Custom Collectors
                            Labels
                            Guidelines


        IV. PromQL

                13. Introduction to PromQL
                            Aggregation Basics
                            Gauge
                            Counter
                            Summary
                            Histogram
                            Selectors
                            Matchers
                            Instant Vector
                            Range Vector
                            Offset
                            HTTP API
                            query
                            query_range
                14. Aggregation Operators
                            Grouping
                            without
                            by
                            Operators
                            sum
                            count
                            avg
                            stddev and stdvar
                            min and max
                            topk and bottomk
                            quantile
                            count_values
                15. Binary Operators
                            Working with Scalars
                            Arithmetic Operators
                            Comparison Operators
                            Vector Matching
                            One-to-One
                            Many-to-One and group_left
                            Many-to-Many and Logical Operators
                            Operator Precedence
                
                16. Functions
                            Changing Type
                            vector
                            scalar
                            Math
                            abs
                            ln, log2, and log10
                            exp
                            sqrt
                            ceil and floor
                            round
                            clamp_max and clamp_min
                            Time and Date
                            time
                            minute, hour, day_of_week, day_of_month, days_in_month, month, and year
                            timestamp
                            Labels
                            label_replace
                            label_join
                            Missing Series and absent
                            Sorting with sort and sort_desc
                            Histograms with histogram_quantile
                            Counters
                            rate
                            increase
                            irate
                            resets
                            Changing Gauges
                            changes
                            deriv
                            predict_linear
                            delta
                            idelta
                            holt_winters
                            Aggregation Over Time

        17. Recording Rules
                            Using Recording Rules
                            When to Use Recording Rules
                            Reducing Cardinality
                            Composing Range Vector Functions
                            Rules for APIs
                            How Not to Use Rules
                            Naming of Recording Rules

        V. Alerting

                    18. Alerting
                                Alerting Rules
                                for
                                Alert Labels
                                Annotations and Templates
                                What Are Good Alerts?
                                Configuring Alertmanagers
                                External Labels
                    19. Alertmanager
                                Notification Pipeline
                                Configuration File
                                Routing Tree
                                Receivers
                                Inhibitions
                                Alertmanager Web Interface

        VI. Deployment

                    20. Putting It All Together
                                Planning a Rollout
                                Growing Prometheus
                                Going Global with Federation
                                Long-Term Storage
                                Running Prometheus
                                Hardware
                                Configuration Management
                                Networks and Authentication
                                Planning for Failure
                                Alertmanager Clustering
                                Meta- and Cross-Monitoring
                                Managing Performance
                                Detecting a Problem
                                Finding Expensive Metrics and Targets
                                Reducing Load
                                Horizontal Sharding
                                Managing Change