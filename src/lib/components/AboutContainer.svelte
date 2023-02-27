<script></script>

<div class="container">
    <div class="content">
        <h1>About Me</h1>
        <ul class="primary-list">
            <li>Software engineer with 2+ years professional experience developing RESTful APIs in a cloud-based microservices oriented architecture.</li>
            <li>Languages/Frameworks/Etc I have worked with professionally:
                <ul class="experience-in">
                    <li><strong>Java (Spring Boot/Spring Reactive/Spring Gateway)</strong></li>
                    <li><strong>Keycloak (IAM)</strong></li>
                    <li><strong>Mongodb</strong></li>
                    <li><strong>Elasticsearch (ELK stack)</strong></li>
                    <li>RabbitMQ</li>
                    <li>Oracle/Postgres</li>
                    <li>Docker/Docker Compose</li>
                </ul>
            </li>
            <li>Examples of projects I have worked on:
                <ul class="projects">
                    <li>Redesigned a recommendation service that accepts a CSV file containing eleven million or more recommendations from an S3 bucket and ingests that data
                        into mongodb. Recommendations are ingested in parallel using Java threads
                        and a producer/consumer pattern. This data is automatically synced into an elastic index via Monstache.
                    </li>
                    <li>Managed and developed extensions for Keycloak, an open source Identity Access Management solution. Configured Keycloak clients with values
                        expected such that users are redirected to the Keycloak login/registration pages as desired. Developed extensions for user login to persist users to
                        an additional data store (user federation) from both the registration page and via third party providers (Google, Microsoft, LinkedIn, etc).
                        Configured groups, roles, and other security configurations within Keycloak. Led research and development on upgrading from Keycloak legacy (jboss as the application server)
                        to Keycloak v20+ (quarkus as the application server).
                    </li>
                    <li>Utilized Spring Reactive for an API Gateway to automatically rewrite a location header when a condition was met in the request.
                        The location header would have an updated redirect value to successfully redirect to the expected URL.
                    </li>
                    <li>Developed an ingestion service for Elastic AppSearch - based on events received via RabbitMQ, ingest documents into AppSearch that could
                        then be viewed via AppSearch search endpoint.
                    </li>
                </ul>
            </li>
            <li>Programming related hobbies: 
                <ul class="programming-hobbies">
                    <li>REST API development using Node.js and Go</li>
                    <li>Game development using Unity (C#)</li>
                    <li>Frontend development using Svelte/SvelteKit - this site was made with SvelteKit!</li>
                </ul>
            </li>
        </ul>
    </div>
</div>

<style>
    .primary-list {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        margin: 20px;
        padding: 20px;
    }
    .experience-in {
        padding: 20px;
    }
    .projects {
        padding: 20px;
    }
    .projects {
        display: flex;
        flex-direction: column;
        gap: 20px;
    }
    .programming-hobbies {
        padding: 20px;
    }

    .projects  {
        list-style-type: square;
    }
</style>