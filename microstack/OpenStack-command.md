## Openstack command list ###
```
ubuntu@openstack:~$ microstack.openstack --help
usage: openstack [--version] [-v | -q] [--log-file LOG_FILE] [-h] [--debug] [--os-cloud <cloud-config-name>] [--os-region-name <auth-region-name>] [--os-cacert <ca-bundle-file>]
                 [--os-cert <certificate-file>] [--os-key <key-file>] [--verify | --insecure] [--os-default-domain <auth-domain>] [--os-interface <interface>]
                 [--os-service-provider <service_provider>] [--os-remote-project-name <remote_project_name> | --os-remote-project-id <remote_project_id>]
                 [--os-remote-project-domain-name <remote_project_domain_name> | --os-remote-project-domain-id <remote_project_domain_id>] [--timing] [--os-beta-command]
                 [--os-profile hmac-key] [--os-compute-api-version <compute-api-version>] [--os-identity-api-version <identity-api-version>]
                 [--os-image-api-version <image-api-version>] [--os-network-api-version <network-api-version>] [--os-object-api-version <object-api-version>]
                 [--os-volume-api-version <volume-api-version>] [--os-dns-api-version <dns-api-version>] [--os-key-manager-api-version <key-manager-api-version>]
                 [--os-auth-type <auth-type>] [--os-auth-url <auth-auth-url>] [--os-domain-id <auth-domain-id>] [--os-domain-name <auth-domain-name>]
                 [--os-project-id <auth-project-id>] [--os-project-name <auth-project-name>] [--os-project-domain-id <auth-project-domain-id>]
                 [--os-project-domain-name <auth-project-domain-name>] [--os-system-scope <auth-system-scope>] [--os-trust-id <auth-trust-id>]
                 [--os-identity-provider <auth-identity-provider>] [--os-protocol <auth-protocol>] [--os-identity-provider-url <auth-identity-provider-url>]
                 [--os-service-provider-endpoint <auth-service-provider-endpoint>] [--os-service-provider-entity-id <auth-service-provider-entity-id>]
                 [--os-username <auth-username>] [--os-password <auth-password>] [--os-client-id <auth-client-id>] [--os-client-secret <auth-client-secret>]
                 [--os-openid-scope <auth-openid-scope>] [--os-access-token-endpoint <auth-access-token-endpoint>] [--os-discovery-endpoint <auth-discovery-endpoint>]
                 [--os-access-token-type <auth-access-token-type>] [--os-default-domain-id <auth-default-domain-id>] [--os-default-domain-name <auth-default-domain-name>]
                 [--os-token <auth-token>] [--os-consumer-key <auth-consumer-key>] [--os-consumer-secret <auth-consumer-secret>] [--os-access-key <auth-access-key>]
                 [--os-access-secret <auth-access-secret>] [--os-redirect-uri <auth-redirect-uri>] [--os-code <auth-code>] [--os-user-id <auth-user-id>]
                 [--os-user-domain-id <auth-user-domain-id>] [--os-user-domain-name <auth-user-domain-name>] [--os-passcode <auth-passcode>]
                 [--os-auth-methods <auth-auth-methods>] [--os-endpoint <auth-endpoint>] [--os-application-credential-secret <auth-application-credential-secret>]
                 [--os-application-credential-id <auth-application-credential-id>] [--os-application-credential-name <auth-application-credential-name>]
                 [--os-access-token <auth-access-token>]

Command-line interface to the OpenStack APIs

optional arguments:
  --version             show program's version number and exit
  -v, --verbose         Increase verbosity of output. Can be repeated.
  -q, --quiet           Suppress output except warnings and errors.
  --log-file LOG_FILE   Specify a file to log output. Disabled by default.
  -h, --help            Show help message and exit.
  --debug               Show tracebacks on errors.
  --os-cloud <cloud-config-name>
                        Cloud name in clouds.yaml (Env: OS_CLOUD)
  --os-region-name <auth-region-name>
                        Authentication region name (Env: OS_REGION_NAME)
  --os-cacert <ca-bundle-file>
                        CA certificate bundle file (Env: OS_CACERT)
  --os-cert <certificate-file>
                        Client certificate bundle file (Env: OS_CERT)
  --os-key <key-file>   Client certificate key file (Env: OS_KEY)
  --verify              Verify server certificate (default)
  --insecure            Disable server certificate verification
  --os-default-domain <auth-domain>
                        Default domain ID, default=default. (Env: OS_DEFAULT_DOMAIN)
  --os-interface <interface>
                        Select an interface type. Valid interface types: [admin, public, internal]. default=public, (Env: OS_INTERFACE)
  --os-service-provider <service_provider>
                        Authenticate with and perform the command on a service provider using Keystone-to-keystone federation. Must also specify the remote project option.
  --os-remote-project-name <remote_project_name>
                        Project name when authenticating to a service provider if using Keystone-to-Keystone federation.
  --os-remote-project-id <remote_project_id>
                        Project ID when authenticating to a service provider if using Keystone-to-Keystone federation.
  --os-remote-project-domain-name <remote_project_domain_name>
                        Domain name of the project when authenticating to a service provider if using Keystone-to-Keystone federation.
  --os-remote-project-domain-id <remote_project_domain_id>
                        Domain ID of the project when authenticating to a service provider if using Keystone-to-Keystone federation.
  --timing              Print API call timing info
  --os-beta-command     Enable beta commands which are subject to change
  --os-profile hmac-key
                        HMAC key for encrypting profiling context data
  --os-compute-api-version <compute-api-version>
                        Compute API version, default=2.1 (Env: OS_COMPUTE_API_VERSION)
  --os-identity-api-version <identity-api-version>
                        Identity API version, default=3 (Env: OS_IDENTITY_API_VERSION)
  --os-image-api-version <image-api-version>
                        Image API version, default=2 (Env: OS_IMAGE_API_VERSION)
  --os-network-api-version <network-api-version>
                        Network API version, default=2.0 (Env: OS_NETWORK_API_VERSION)
  --os-object-api-version <object-api-version>
                        Object API version, default=1 (Env: OS_OBJECT_API_VERSION)
  --os-volume-api-version <volume-api-version>
                        Volume API version, default=3 (Env: OS_VOLUME_API_VERSION)
  --os-dns-api-version <dns-api-version>
                        DNS API version, default=2 (Env: OS_DNS_API_VERSION)
  --os-key-manager-api-version <key-manager-api-version>
                        Barbican API version, default=1 (Env: OS_KEY_MANAGER_API_VERSION)
  --os-auth-type <auth-type>
                        Select an authentication type. Available types: v3tokenlessauth, v3adfspassword, v3oidcpassword, token, v3token, v3oauth1, v3oidcauthcode, v3totp,
                        v3multifactor, password, admin_token, v2password, none, v3samlpassword, v3applicationcredential, noauth, v3password, v3oidcclientcredentials,
                        v3oidcaccesstoken, v1password, v2token. Default: selected based on --os-username/--os-token (Env: OS_AUTH_TYPE)
  --os-auth-url <auth-auth-url>
                        With v3tokenlessauth: Authentication URL With v3adfspassword: Authentication URL With v3oidcpassword: Authentication URL With token: Authentication URL
                        With v3token: Authentication URL With v3oauth1: Authentication URL With v3oidcauthcode: Authentication URL With v3totp: Authentication URL With
                        v3multifactor: Authentication URL With password: Authentication URL With v2password: Authentication URL With v3samlpassword: Authentication URL With
                        v3applicationcredential: Authentication URL With v3password: Authentication URL With v3oidcclientcredentials: Authentication URL With v3oidcaccesstoken:
                        Authentication URL With v1password: Authentication URL With v2token: Authentication URL (Env: OS_AUTH_URL)
  --os-domain-id <auth-domain-id>
                        With v3tokenlessauth: Domain ID to scope to With v3adfspassword: Domain ID to scope to With v3oidcpassword: Domain ID to scope to With token: Domain ID to
                        scope to With v3token: Domain ID to scope to With v3oidcauthcode: Domain ID to scope to With v3totp: Domain ID to scope to With v3multifactor: Domain ID to
                        scope to With password: Domain ID to scope to With v3samlpassword: Domain ID to scope to With v3applicationcredential: Domain ID to scope to With
                        v3password: Domain ID to scope to With v3oidcclientcredentials: Domain ID to scope to With v3oidcaccesstoken: Domain ID to scope to (Env: OS_DOMAIN_ID)
  --os-domain-name <auth-domain-name>
                        With v3tokenlessauth: Domain name to scope to With v3adfspassword: Domain name to scope to With v3oidcpassword: Domain name to scope to With token: Domain
                        name to scope to With v3token: Domain name to scope to With v3oidcauthcode: Domain name to scope to With v3totp: Domain name to scope to With
                        v3multifactor: Domain name to scope to With password: Domain name to scope to With v3samlpassword: Domain name to scope to With v3applicationcredential:
                        Domain name to scope to With v3password: Domain name to scope to With v3oidcclientcredentials: Domain name to scope to With v3oidcaccesstoken: Domain name
                        to scope to (Env: OS_DOMAIN_NAME)
  --os-project-id <auth-project-id>
                        With v3tokenlessauth: Project ID to scope to With v3adfspassword: Project ID to scope to With v3oidcpassword: Project ID to scope to With token: Project ID
                        to scope to With v3token: Project ID to scope to With v3oidcauthcode: Project ID to scope to With v3totp: Project ID to scope to With v3multifactor:
                        Project ID to scope to With password: Project ID to scope to With v3samlpassword: Project ID to scope to With v3applicationcredential: Project ID to scope
                        to With noauth: Project ID With v3password: Project ID to scope to With v3oidcclientcredentials: Project ID to scope to With v3oidcaccesstoken: Project ID
                        to scope to (Env: OS_PROJECT_ID)
  --os-project-name <auth-project-name>
                        With v3tokenlessauth: Project name to scope to With v3adfspassword: Project name to scope to With v3oidcpassword: Project name to scope to With token:
                        Project name to scope to With v3token: Project name to scope to With v3oidcauthcode: Project name to scope to With v3totp: Project name to scope to With
                        v3multifactor: Project name to scope to With password: Project name to scope to With v3samlpassword: Project name to scope to With v3applicationcredential:
                        Project name to scope to With v3password: Project name to scope to With v3oidcclientcredentials: Project name to scope to With v3oidcaccesstoken: Project
                        name to scope to With v1password: Swift account to use (Env: OS_PROJECT_NAME)
  --os-project-domain-id <auth-project-domain-id>
                        With v3tokenlessauth: Domain ID containing project With v3adfspassword: Domain ID containing project With v3oidcpassword: Domain ID containing project With
                        token: Domain ID containing project With v3token: Domain ID containing project With v3oidcauthcode: Domain ID containing project With v3totp: Domain ID
                        containing project With v3multifactor: Domain ID containing project With password: Domain ID containing project With v3samlpassword: Domain ID containing
                        project With v3applicationcredential: Domain ID containing project With v3password: Domain ID containing project With v3oidcclientcredentials: Domain ID
                        containing project With v3oidcaccesstoken: Domain ID containing project (Env: OS_PROJECT_DOMAIN_ID)
  --os-project-domain-name <auth-project-domain-name>
                        With v3tokenlessauth: Domain name containing project With v3adfspassword: Domain name containing project With v3oidcpassword: Domain name containing
                        project With token: Domain name containing project With v3token: Domain name containing project With v3oidcauthcode: Domain name containing project With
                        v3totp: Domain name containing project With v3multifactor: Domain name containing project With password: Domain name containing project With
                        v3samlpassword: Domain name containing project With v3applicationcredential: Domain name containing project With v3password: Domain name containing project
                        With v3oidcclientcredentials: Domain name containing project With v3oidcaccesstoken: Domain name containing project (Env: OS_PROJECT_DOMAIN_NAME)
  --os-system-scope <auth-system-scope>
                        With v3adfspassword: Scope for system operations With v3oidcpassword: Scope for system operations With token: Scope for system operations With v3token:
                        Scope for system operations With v3oidcauthcode: Scope for system operations With v3totp: Scope for system operations With v3multifactor: Scope for system
                        operations With password: Scope for system operations With v3samlpassword: Scope for system operations With v3applicationcredential: Scope for system
                        operations With v3password: Scope for system operations With v3oidcclientcredentials: Scope for system operations With v3oidcaccesstoken: Scope for system
                        operations (Env: OS_SYSTEM_SCOPE)
  --os-trust-id <auth-trust-id>
                        With v3adfspassword: Trust ID With v3oidcpassword: Trust ID With token: Trust ID With v3token: Trust ID With v3oidcauthcode: Trust ID With v3totp: Trust ID
                        With v3multifactor: Trust ID With password: Trust ID With v2password: Trust ID With v3samlpassword: Trust ID With v3applicationcredential: Trust ID With
                        v3password: Trust ID With v3oidcclientcredentials: Trust ID With v3oidcaccesstoken: Trust ID With v2token: Trust ID (Env: OS_TRUST_ID)
  --os-identity-provider <auth-identity-provider>
                        With v3adfspassword: Identity Provider's name With v3oidcpassword: Identity Provider's name With v3oidcauthcode: Identity Provider's name With
                        v3samlpassword: Identity Provider's name With v3oidcclientcredentials: Identity Provider's name With v3oidcaccesstoken: Identity Provider's name (Env:
                        OS_IDENTITY_PROVIDER)
  --os-protocol <auth-protocol>
                        With v3adfspassword: Protocol for federated plugin With v3oidcpassword: Protocol for federated plugin With v3oidcauthcode: Protocol for federated plugin
                        With v3samlpassword: Protocol for federated plugin With v3oidcclientcredentials: Protocol for federated plugin With v3oidcaccesstoken: Protocol for
                        federated plugin (Env: OS_PROTOCOL)
  --os-identity-provider-url <auth-identity-provider-url>
                        With v3adfspassword: An Identity Provider URL, where the SAML authentication request will be sent. With v3samlpassword: An Identity Provider URL, where the
                        SAML2 authentication request will be sent. (Env: OS_IDENTITY_PROVIDER_URL)
  --os-service-provider-endpoint <auth-service-provider-endpoint>
                        With v3adfspassword: Service Provider's Endpoint (Env: OS_SERVICE_PROVIDER_ENDPOINT)
  --os-service-provider-entity-id <auth-service-provider-entity-id>
                        With v3adfspassword: Service Provider's SAML Entity ID (Env: OS_SERVICE_PROVIDER_ENTITY_ID)
  --os-username <auth-username>
                        With v3adfspassword: Username With v3oidcpassword: Username With v3totp: Username With password: Username With v2password: Username to login with With
                        v3samlpassword: Username With v3applicationcredential: Username With v3password: Username With v1password: Username to login with (Env: OS_USERNAME)
  --os-password <auth-password>
                        With v3adfspassword: Password With v3oidcpassword: Password With password: User's password With v2password: Password to use With v3samlpassword: Password
                        With v3password: User's password With v1password: Password to use (Env: OS_PASSWORD)
  --os-client-id <auth-client-id>
                        With v3oidcpassword: OAuth 2.0 Client ID With v3oidcauthcode: OAuth 2.0 Client ID With v3oidcclientcredentials: OAuth 2.0 Client ID (Env: OS_CLIENT_ID)
  --os-client-secret <auth-client-secret>
                        With v3oidcpassword: OAuth 2.0 Client Secret With v3oidcauthcode: OAuth 2.0 Client Secret With v3oidcclientcredentials: OAuth 2.0 Client Secret (Env:
                        OS_CLIENT_SECRET)
  --os-openid-scope <auth-openid-scope>
                        With v3oidcpassword: OpenID Connect scope that is requested from authorization server. Note that the OpenID Connect specification states that "openid" must
                        be always specified. With v3oidcauthcode: OpenID Connect scope that is requested from authorization server. Note that the OpenID Connect specification
                        states that "openid" must be always specified. With v3oidcclientcredentials: OpenID Connect scope that is requested from authorization server. Note that
                        the OpenID Connect specification states that "openid" must be always specified. (Env: OS_OPENID_SCOPE)
  --os-access-token-endpoint <auth-access-token-endpoint>
                        With v3oidcpassword: OpenID Connect Provider Token Endpoint. Note that if a discovery document is being passed this option will override the endpoint
                        provided by the server in the discovery document. With v3oidcauthcode: OpenID Connect Provider Token Endpoint. Note that if a discovery document is being
                        passed this option will override the endpoint provided by the server in the discovery document. With v3oidcclientcredentials: OpenID Connect Provider Token
                        Endpoint. Note that if a discovery document is being passed this option will override the endpoint provided by the server in the discovery document. (Env:
                        OS_ACCESS_TOKEN_ENDPOINT)
  --os-discovery-endpoint <auth-discovery-endpoint>
                        With v3oidcpassword: OpenID Connect Discovery Document URL. The discovery document will be used to obtain the values of the access token endpoint and the
                        authentication endpoint. This URL should look like https://idp.example.org/.well-known/openid-configuration With v3oidcauthcode: OpenID Connect Discovery
                        Document URL. The discovery document will be used to obtain the values of the access token endpoint and the authentication endpoint. This URL should look
                        like https://idp.example.org/.well-known/openid-configuration With v3oidcclientcredentials: OpenID Connect Discovery Document URL. The discovery document
                        will be used to obtain the values of the access token endpoint and the authentication endpoint. This URL should look like https://idp.example.org/.well-
                        known/openid-configuration (Env: OS_DISCOVERY_ENDPOINT)
  --os-access-token-type <auth-access-token-type>
                        With v3oidcpassword: OAuth 2.0 Authorization Server Introspection token type, it is used to decide which type of token will be used when processing token
                        introspection. Valid values are: "access_token" or "id_token" With v3oidcauthcode: OAuth 2.0 Authorization Server Introspection token type, it is used to
                        decide which type of token will be used when processing token introspection. Valid values are: "access_token" or "id_token" With v3oidcclientcredentials:
                        OAuth 2.0 Authorization Server Introspection token type, it is used to decide which type of token will be used when processing token introspection. Valid
                        values are: "access_token" or "id_token" (Env: OS_ACCESS_TOKEN_TYPE)
  --os-default-domain-id <auth-default-domain-id>
                        With token: Optional domain ID to use with v3 and v2 parameters. It will be used for both the user and project domain in v3 and ignored in v2
                        authentication. With password: Optional domain ID to use with v3 and v2 parameters. It will be used for both the user and project domain in v3 and ignored
                        in v2 authentication. (Env: OS_DEFAULT_DOMAIN_ID)
  --os-default-domain-name <auth-default-domain-name>
                        With token: Optional domain name to use with v3 API and v2 parameters. It will be used for both the user and project domain in v3 and ignored in v2
                        authentication. With password: Optional domain name to use with v3 API and v2 parameters. It will be used for both the user and project domain in v3 and
                        ignored in v2 authentication. (Env: OS_DEFAULT_DOMAIN_NAME)
  --os-token <auth-token>
                        With token: Token to authenticate with With v3token: Token to authenticate with With admin_token: The token that will always be used With v2token: Token
                        (Env: OS_TOKEN)
  --os-consumer-key <auth-consumer-key>
                        With v3oauth1: OAuth Consumer ID/Key (Env: OS_CONSUMER_KEY)
  --os-consumer-secret <auth-consumer-secret>
                        With v3oauth1: OAuth Consumer Secret (Env: OS_CONSUMER_SECRET)
  --os-access-key <auth-access-key>
                        With v3oauth1: OAuth Access Key (Env: OS_ACCESS_KEY)
  --os-access-secret <auth-access-secret>
                        With v3oauth1: OAuth Access Secret (Env: OS_ACCESS_SECRET)
  --os-redirect-uri <auth-redirect-uri>
                        With v3oidcauthcode: OpenID Connect Redirect URL (Env: OS_REDIRECT_URI)
  --os-code <auth-code>
                        With v3oidcauthcode: OAuth 2.0 Authorization Code (Env: OS_CODE)
  --os-user-id <auth-user-id>
                        With v3totp: User ID With password: User id With v2password: User ID to login with With v3applicationcredential: User ID With noauth: User ID With
                        v3password: User ID (Env: OS_USER_ID)
  --os-user-domain-id <auth-user-domain-id>
                        With v3totp: User's domain id With password: User's domain id With v3applicationcredential: User's domain id With v3password: User's domain id (Env:
                        OS_USER_DOMAIN_ID)
  --os-user-domain-name <auth-user-domain-name>
                        With v3totp: User's domain name With password: User's domain name With v3applicationcredential: User's domain name With v3password: User's domain name
                        (Env: OS_USER_DOMAIN_NAME)
  --os-passcode <auth-passcode>
                        With v3totp: User's TOTP passcode (Env: OS_PASSCODE)
  --os-auth-methods <auth-auth-methods>
                        With v3multifactor: Methods to authenticate with. (Env: OS_AUTH_METHODS)
  --os-endpoint <auth-endpoint>
                        With admin_token: The endpoint that will always be used With none: The endpoint that will always be used With noauth: Cinder endpoint (Env: OS_ENDPOINT)
  --os-application-credential-secret <auth-application-credential-secret>
                        With v3applicationcredential: Application credential auth secret (Env: OS_APPLICATION_CREDENTIAL_SECRET)
  --os-application-credential-id <auth-application-credential-id>
                        With v3applicationcredential: Application credential ID (Env: OS_APPLICATION_CREDENTIAL_ID)
  --os-application-credential-name <auth-application-credential-name>
                        With v3applicationcredential: Application credential name (Env: OS_APPLICATION_CREDENTIAL_NAME)
  --os-access-token <auth-access-token>
                        With v3oidcaccesstoken: OAuth 2.0 Access Token (Env: OS_ACCESS_TOKEN)

Commands:
  access rule delete  Delete access rule(s)
  access rule list  List access rules
  access rule show  Display access rule details
  access token create  Create an access token
  acl delete     Delete ACLs for a secret or container as identified by its href. (python-barbicanclient)
  acl get        Retrieve ACLs for a secret or container by providing its href. (python-barbicanclient)
  acl submit     Submit ACL on a secret or container as identified by its href. (python-barbicanclient)
  acl user add   Add ACL users to a secret or container as identified by its href. (python-barbicanclient)
  acl user remove  Remove ACL users from a secret or container as identified by its href. (python-barbicanclient)
  address scope create  Create a new Address Scope
  address scope delete  Delete address scope(s)
  address scope list  List address scopes
  address scope set  Set address scope properties
  address scope show  Display address scope details
  aggregate add host  Add host to aggregate
  aggregate create  Create a new aggregate
  aggregate delete  Delete existing aggregate(s)
  aggregate list  List all aggregates
  aggregate remove host  Remove host from aggregate
  aggregate set  Set aggregate properties
  aggregate show  Display aggregate details
  aggregate unset  Unset aggregate properties
  application credential create  Create new application credential
  application credential delete  Delete application credentials(s)
  application credential list  List application credentials
  application credential show  Display application credential details
  availability zone list  List availability zones and their status
  bgp dragent add speaker  Add a BGP speaker to a dynamic routing agent (python-neutronclient)
  bgp dragent list  List dynamic routing agents (python-neutronclient)
  bgp dragent remove speaker  Removes a BGP speaker from a dynamic routing agent (python-neutronclient)
  bgp peer create  Create a BGP peer (python-neutronclient)
  bgp peer delete  Delete a BGP peer (python-neutronclient)
  bgp peer list  List BGP peers (python-neutronclient)
  bgp peer set   Update a BGP peer (python-neutronclient)
  bgp peer show  Show information for a BGP peer (python-neutronclient)
  bgp speaker add network  Add a network to a BGP speaker (python-neutronclient)
  bgp speaker add peer  Add a peer to a BGP speaker (python-neutronclient)
  bgp speaker create  Create a BGP speaker (python-neutronclient)
  bgp speaker delete  Delete a BGP speaker (python-neutronclient)
  bgp speaker list  List BGP speakers (python-neutronclient)
  bgp speaker list advertised routes  List routes advertised (python-neutronclient)
  bgp speaker remove network  Remove a network from a BGP speaker (python-neutronclient)
  bgp speaker remove peer  Remove a peer from a BGP speaker (python-neutronclient)
  bgp speaker set  Set BGP speaker properties (python-neutronclient)
  bgp speaker show  Show a BGP speaker (python-neutronclient)
  bgp speaker show dragents  (Deprecated) List dynamic routing agents hosting a BGP speaker (python-neutronclient)
  bgpvpn create  Create BGP VPN resource (python-neutronclient)
  bgpvpn delete  Delete BGP VPN resource(s) (python-neutronclient)
  bgpvpn list    List BGP VPN resources (python-neutronclient)
  bgpvpn network association create  Create a BGP VPN network association (python-neutronclient)
  bgpvpn network association delete  Delete a BGP VPN network association(s) for a given BGP VPN (python-neutronclient)
  bgpvpn network association list  List BGP VPN network associations for a given BGP VPN (python-neutronclient)
  bgpvpn network association show  Show information of a given BGP VPN network association (python-neutronclient)
  bgpvpn port association create  Create a BGP VPN port association (python-neutronclient)
  bgpvpn port association delete  Delete a BGP VPN port association(s) for a given BGP VPN (python-neutronclient)
  bgpvpn port association list  List BGP VPN port associations for a given BGP VPN (python-neutronclient)
  bgpvpn port association set  Set BGP VPN port association properties (python-neutronclient)
  bgpvpn port association show  Show information of a given BGP VPN port association (python-neutronclient)
  bgpvpn port association unset  Unset BGP VPN port association properties (python-neutronclient)
  bgpvpn router association create  Create a BGP VPN router association (python-neutronclient)
  bgpvpn router association delete  Delete a BGP VPN router association(s) for a given BGP VPN (python-neutronclient)
  bgpvpn router association list  List BGP VPN router associations for a given BGP VPN (python-neutronclient)
  bgpvpn router association set  Set BGP VPN router association properties (python-neutronclient)
  bgpvpn router association show  Show information of a given BGP VPN router association (python-neutronclient)
  bgpvpn router association unset  Unset BGP VPN router association properties (python-neutronclient)
  bgpvpn set     Set BGP VPN properties (python-neutronclient)
  bgpvpn show    Show information of a given BGP VPN (python-neutronclient)
  bgpvpn unset   Unset BGP VPN properties (python-neutronclient)
  ca get         Retrieve a CA by providing its URI. (python-barbicanclient)
  ca list        List CAs. (python-barbicanclient)
  catalog list   List services in the service catalog
  catalog show   Display service catalog details
  command list   List recognized commands by group
  complete       print bash completion command (cliff)
  compute agent create  Create compute agent
  compute agent delete  Delete compute agent(s)
  compute agent list  List compute agents
  compute agent set  Set compute agent properties
  compute service delete  Delete compute service(s)
  compute service list  List compute services. Using ``--os-compute-api-version`` 2.53 or greater will return the ID as a UUID value which can be used to uniquely identify the service in a multi-cell deployment.
  compute service set  Set compute service properties
  configuration show  Display configuration details
  consistency group add volume  Add volume(s) to consistency group
  consistency group create  Create new consistency group.
  consistency group delete  Delete consistency group(s).
  consistency group list  List consistency groups.
  consistency group remove volume  Remove volume(s) from consistency group
  consistency group set  Set consistency group properties
  consistency group show  Display consistency group details.
  consistency group snapshot create  Create new consistency group snapshot.
  consistency group snapshot delete  Delete consistency group snapshot(s).
  consistency group snapshot list  List consistency group snapshots.
  consistency group snapshot show  Display consistency group snapshot details
  console log show  Show server's console output
  console url show  Show server's remote console URL
  consumer create  Create new consumer
  consumer delete  Delete consumer(s)
  consumer list  List consumers
  consumer set   Set consumer properties
  consumer show  Display consumer details
  container create  Create new container
  container delete  Delete container
  container list  List containers
  container save  Save container contents locally
  container set  Set container properties
  container show  Display container details
  container unset  Unset container properties
  credential create  Create new credential
  credential delete  Delete credential(s)
  credential list  List credentials
  credential set  Set credential properties
  credential show  Display credential details
  dns quota list  List quotas (python-designateclient)
  dns quota reset  Reset quotas (python-designateclient)
  dns quota set  Set quotas (python-designateclient)
  dns service list  List service statuses (python-designateclient)
  dns service show  Show service status details (python-designateclient)
  domain create  Create new domain
  domain delete  Delete domain(s)
  domain list    List domains
  domain set     Set domain properties
  domain show    Display domain details
  ec2 credentials create  Create EC2 credentials
  ec2 credentials delete  Delete EC2 credentials
  ec2 credentials list  List EC2 credentials
  ec2 credentials show  Display EC2 credentials details
  endpoint add project  Associate a project to an endpoint
  endpoint create  Create new endpoint
  endpoint delete  Delete endpoint(s)
  endpoint group add project  Add a project to an endpoint group
  endpoint group create  Create new endpoint group
  endpoint group delete  Delete endpoint group(s)
  endpoint group list  List endpoint groups
  endpoint group remove project  Remove project from endpoint group
  endpoint group set  Set endpoint group properties
  endpoint group show  Display endpoint group details
  endpoint list  List endpoints
  endpoint remove project  Dissociate a project from an endpoint
  endpoint set   Set endpoint properties
  endpoint show  Display endpoint details
  extension list  List API extensions
  extension show  Show API extension
  federation domain list  List accessible domains
  federation project list  List accessible projects
  federation protocol create  Create new federation protocol
  federation protocol delete  Delete federation protocol(s)
  federation protocol list  List federation protocols
  federation protocol set  Set federation protocol properties
  federation protocol show  Display federation protocol details
  firewall group create  Create a new firewall group (python-neutronclient)
  firewall group delete  Delete firewall group(s) (python-neutronclient)
  firewall group list  List firewall groups (python-neutronclient)
  firewall group policy add rule  Insert a rule into a given firewall policy (python-neutronclient)
  firewall group policy create  Create a new firewall policy (python-neutronclient)
  firewall group policy delete  Delete firewall policy(s) (python-neutronclient)
  firewall group policy list  List firewall policies (python-neutronclient)
  firewall group policy remove rule  Remove a rule from a given firewall policy (python-neutronclient)
  firewall group policy set  Set firewall policy properties (python-neutronclient)
  firewall group policy show  Display firewall policy details (python-neutronclient)
  firewall group policy unset  Unset firewall policy properties (python-neutronclient)
  firewall group rule create  Create a new firewall rule (python-neutronclient)
  firewall group rule delete  Delete firewall rule(s) (python-neutronclient)
  firewall group rule list  List firewall rules that belong to a given tenant (python-neutronclient)
  firewall group rule set  Set firewall rule properties (python-neutronclient)
  firewall group rule show  Display firewall rule details (python-neutronclient)
  firewall group rule unset  Unset firewall rule properties (python-neutronclient)
  firewall group set  Set firewall group properties (python-neutronclient)
  firewall group show  Display firewall group details (python-neutronclient)
  firewall group unset  Unset firewall group properties (python-neutronclient)
  flavor create  Create new flavor
  flavor delete  Delete flavor(s)
  flavor list    List flavors
  flavor set     Set flavor properties
  flavor show    Display flavor details
  flavor unset   Unset flavor properties
  floating ip create  Create floating IP
  floating ip delete  Delete floating IP(s)
  floating ip list  List floating IP(s)
  floating ip pool list  List pools of floating IP addresses
  floating ip port forwarding create  Create floating IP port forwarding
  floating ip port forwarding delete  Delete floating IP port forwarding
  floating ip port forwarding list  List floating IP port forwarding
  floating ip port forwarding set  Set floating IP Port Forwarding Properties
  floating ip port forwarding show  Display floating IP Port Forwarding details
  floating ip set  Set floating IP Properties
  floating ip show  Display floating IP details
  floating ip unset  Unset floating IP Properties
  group add user  Add user to group
  group contains user  Check user membership in group
  group create   Create new group
  group delete   Delete group(s)
  group list     List groups
  group remove user  Remove user from group
  group set      Set group properties
  group show     Display group details
  help           print detailed help for another command (cliff)
  host list      List hosts
  host set       Set host properties
  host show      Display host details
  hypervisor list  List hypervisors
  hypervisor show  Display hypervisor details
  hypervisor stats show  Display hypervisor stats details
  identity provider create  Create new identity provider
  identity provider delete  Delete identity provider(s)
  identity provider list  List identity providers
  identity provider set  Set identity provider properties
  identity provider show  Display identity provider details
  image add project  Associate project with image
  image create   Create/upload an image
  image delete   Delete image(s)
  image list     List available images
  image member list  List projects associated with image
  image remove project  Disassociate project with image
  image save     Save an image locally
  image set      Set image properties
  image show     Display image details
  image unset    Unset image tags and properties
  implied role create  Creates an association between prior and implied roles
  implied role delete  Deletes an association between prior and implied roles
  implied role list  List implied roles
  ip availability list  List IP availability for network
  ip availability show  Show network IP availability details
  keypair create  Create new public or private key for server ssh access
  keypair delete  Delete public or private key(s)
  keypair list   List key fingerprints
  keypair show   Display key details
  limit create   Create a limit
  limit delete   Delete a limit
  limit list     List limits
  limit set      Update information about a limit
  limit show     Display limit details
  limits show    Show compute and block storage limits
  mapping create  Create new mapping
  mapping delete  Delete mapping(s)
  mapping list   List mappings
  mapping set    Set mapping properties
  mapping show   Display mapping details
  module list    List module versions
  network agent add network  Add network to an agent
  network agent add router  Add router to an agent
  network agent delete  Delete network agent(s)
  network agent list  List network agents
  network agent remove network  Remove network from an agent.
  network agent remove router  Remove router from an agent
  network agent set  Set network agent properties
  network agent show  Display network agent details
  network auto allocated topology create  Create the  auto allocated topology for project
  network auto allocated topology delete  Delete auto allocated topology for project
  network create  Create new network
  network delete  Delete network(s)
  network flavor add profile  Add a service profile to a network flavor
  network flavor create  Create new network flavor
  network flavor delete  Delete network flavors
  network flavor list  List network flavors
  network flavor profile create  Create new network flavor profile
  network flavor profile delete  Delete network flavor profile
  network flavor profile list  List network flavor profile(s)
  network flavor profile set  Set network flavor profile properties
  network flavor profile show  Display network flavor profile details
  network flavor remove profile  Remove service profile from network flavor
  network flavor set  Set network flavor properties
  network flavor show  Display network flavor details
  network list   List networks
  network log create  Create a new network log (python-neutronclient)
  network log delete  Delete network log(s) (python-neutronclient)
  network log list  List network logs (python-neutronclient)
  network log set  Set network log properties (python-neutronclient)
  network log show  Display network log details (python-neutronclient)
  network loggable resources list  List supported loggable resources (python-neutronclient)
  network meter create  Create network meter
  network meter delete  Delete network meter
  network meter list  List network meters
  network meter rule create  Create a new meter rule
  network meter rule delete  Delete meter rule(s)
  network meter rule list  List meter rules
  network meter rule show  Display meter rules details
  network meter show  Show network meter
  network onboard subnets  Onboard network subnets into a subnet pool (python-neutronclient)
  network qos policy create  Create a QoS policy
  network qos policy delete  Delete Qos Policy(s)
  network qos policy list  List QoS policies
  network qos policy set  Set QoS policy properties
  network qos policy show  Display QoS policy details
  network qos rule create  Create new Network QoS rule
  network qos rule delete  Delete Network QoS rule
  network qos rule list  List Network QoS rules
  network qos rule set  Set Network QoS rule properties
  network qos rule show  Display Network QoS rule details
  network qos rule type list  List QoS rule types
  network qos rule type show  Show details about supported QoS rule type
  network rbac create  Create network RBAC policy
  network rbac delete  Delete network RBAC policy(s)
  network rbac list  List network RBAC policies
  network rbac set  Set network RBAC policy properties
  network rbac show  Display network RBAC policy details
  network segment create  Create new network segment
  network segment delete  Delete network segment(s)
  network segment list  List network segments
  network segment range create  Create new network segment range
  network segment range delete  Delete network segment range(s)
  network segment range list  List network segment ranges
  network segment range set  Set network segment range properties
  network segment range show  Display network segment range details
  network segment set  Set network segment properties
  network segment show  Display network segment details
  network service provider list  List Service Providers
  network set    Set network properties
  network show   Show network details
  network subport list  List all subports for a given network trunk (python-neutronclient)
  network trunk create  Create a network trunk for a given project (python-neutronclient)
  network trunk delete  Delete a given network trunk (python-neutronclient)
  network trunk list  List all network trunks (python-neutronclient)
  network trunk set  Set network trunk properties (python-neutronclient)
  network trunk show  Show information of a given network trunk (python-neutronclient)
  network trunk unset  Unset subports from a given network trunk (python-neutronclient)
  network unset  Unset network properties
  object create  Upload object to container
  object delete  Delete object from container
  object list    List objects
  object save    Save object locally
  object set     Set object properties
  object show    Display object details
  object store account set  Set account properties
  object store account show  Display account details
  object store account unset  Unset account properties
  object unset   Unset object properties
  policy create  Create new policy
  policy delete  Delete policy(s)
  policy list    List policies
  policy set     Set policy properties
  policy show    Display policy details
  port create    Create a new port
  port delete    Delete port(s)
  port list      List ports
  port set       Set port properties
  port show      Display port details
  port unset     Unset port properties
  project create  Create new project
  project delete  Delete project(s)
  project list   List projects
  project purge  Clean resources associated with a project
  project set    Set project properties
  project show   Display project details
  ptr record list  List floatingip ptr records (python-designateclient)
  ptr record set  Set floatingip ptr record (python-designateclient)
  ptr record show  Show floatingip ptr record details (python-designateclient)
  ptr record unset  Unset floatingip ptr record (python-designateclient)
  quota list     List quotas for all projects with non-default quota values or list detailed quota informations for requested project
  quota set      Set quotas for project or class
  quota show     Show quotas for project or class. Specify ``--os-compute-api-version 2.50`` or higher to see ``server-groups`` and ``server-group-members`` output for a given quota class.
  recordset create  Create new recordset (python-designateclient)
  recordset delete  Delete recordset (python-designateclient)
  recordset list  List recordsets (python-designateclient)
  recordset set  Set recordset properties (python-designateclient)
  recordset show  Show recordset details (python-designateclient)
  region create  Create new region
  region delete  Delete region(s)
  region list    List regions
  region set     Set region properties
  region show    Display region details
  registered limit create  Create a registered limit
  registered limit delete  Delete a registered limit
  registered limit list  List registered limits
  registered limit set  Update information about a registered limit
  registered limit show  Display registered limit details
  request token authorize  Authorize a request token
  request token create  Create a request token
  role add       Adds a role assignment to a user or group on the system, a domain, or a project
  role assignment list  List role assignments
  role create    Create new role
  role delete    Delete role(s)
  role list      List roles
  role remove    Removes a role assignment from system/domain/project : user/group
  role set       Set role properties
  role show      Display role details
  router add port  Add a port to a router
  router add subnet  Add a subnet to a router
  router create  Create a new router
  router delete  Delete router(s)
  router list    List routers
  router remove port  Remove a port from a router
  router remove subnet  Remove a subnet from a router
  router set     Set router properties
  router show    Display router details
  router unset   Unset router properties
  secret container create  Store a container in Barbican. (python-barbicanclient)
  secret container delete  Delete a container by providing its href. (python-barbicanclient)
  secret container get  Retrieve a container by providing its URI. (python-barbicanclient)
  secret container list  List containers. (python-barbicanclient)
  secret delete  Delete a secret by providing its URI. (python-barbicanclient)
  secret get     Retrieve a secret by providing its URI. (python-barbicanclient)
  secret list    List secrets. (python-barbicanclient)
  secret order create  Create a new order. (python-barbicanclient)
  secret order delete  Delete an order by providing its href. (python-barbicanclient)
  secret order get  Retrieve an order by providing its URI. (python-barbicanclient)
  secret order list  List orders. (python-barbicanclient)
  secret store   Store a secret in Barbican. (python-barbicanclient)
  secret update  Update a secret with no payload in Barbican. (python-barbicanclient)
  security group create  Create a new security group
  security group delete  Delete security group(s)
  security group list  List security groups
  security group rule create  Create a new security group rule
  security group rule delete  Delete security group rule(s)
  security group rule list  List security group rules
  security group rule show  Display security group rule details
  security group set  Set security group properties
  security group show  Display security group details
  security group unset  Unset security group properties
  server add fixed ip  Add fixed IP address to server
  server add floating ip  Add floating IP address to server
  server add network  Add network to server
  server add port  Add port to server
  server add security group  Add security group to server
  server add volume  Add volume to server. Specify ``--os-compute-api-version 2.20`` or higher to add a volume to a server with status ``SHELVED`` or ``SHELVED_OFFLOADED``.
  server backup create  Create a server backup image
  server create  Create a new server
  server delete  Delete server(s)
  server dump create  Create a dump file in server(s)
  server event list  List recent events of a server. Specify ``--os-compute-api-version 2.21`` or higher to show events for a deleted server.
  server event show  Show server event details. Specify ``--os-compute-api-version 2.21`` or higher to show event details for a deleted server. Specify ``--os-compute-api-version 2.51`` or higher to show event details for non-admin users.
  server group create  Create a new server group.
  server group delete  Delete existing server group(s).
  server group list  List all server groups.
  server group show  Display server group details.
  server image create  Create a new server disk image from an existing server
  server list    List servers
  server lock    Lock server(s). A non-admin user will not be able to execute actions
  server migrate  Migrate server to different host.
  server migrate confirm  Confirm server migrate.
  server migrate revert  Revert server migrate.
  server pause   Pause server(s)
  server reboot  Perform a hard or soft server reboot
  server rebuild  Rebuild server
  server remove fixed ip  Remove fixed IP address from server
  server remove floating ip  Remove floating IP address from server
  server remove network  Remove all ports of a network from server
  server remove port  Remove port from server
  server remove security group  Remove security group from server
  server remove volume  Remove volume from server. Specify ``--os-compute-api-version 2.20`` or higher to remove a volume from a server with status ``SHELVED`` or ``SHELVED_OFFLOADED``.
  server rescue  Put server in rescue mode
  server resize  Scale server to a new flavor.
  server resize confirm  Confirm server resize.
  server resize revert  Revert server resize.
  server restore  Restore server(s)
  server resume  Resume server(s)
  server set     Set server properties
  server shelve  Shelve server(s)
  server show    Show server details. Specify ``--os-compute-api-version 2.47`` or higher to see the embedded flavor information for the server.
  server ssh     SSH to server
  server start   Start server(s).
  server stop    Stop server(s).
  server suspend  Suspend server(s)
  server unlock  Unlock server(s)
  server unpause  Unpause server(s)
  server unrescue  Restore server from rescue mode
  server unset   Unset server properties
  server unshelve  Unshelve server(s)
  service create  Create new service
  service delete  Delete service(s)
  service list   List services
  service provider create  Create new service provider
  service provider delete  Delete service provider(s)
  service provider list  List service providers
  service provider set  Set service provider properties
  service provider show  Display service provider details
  service set    Set service properties
  service show   Display service details
  sfc flow classifier create  Create a flow classifier (python-neutronclient)
  sfc flow classifier delete  Delete a given flow classifier (python-neutronclient)
  sfc flow classifier list  List flow classifiers (python-neutronclient)
  sfc flow classifier set  Set flow classifier properties (python-neutronclient)
  sfc flow classifier show  Display flow classifier details (python-neutronclient)
  sfc port chain create  Create a port chain (python-neutronclient)
  sfc port chain delete  Delete a given port chain (python-neutronclient)
  sfc port chain list  List port chains (python-neutronclient)
  sfc port chain set  Set port chain properties (python-neutronclient)
  sfc port chain show  Display port chain details (python-neutronclient)
  sfc port chain unset  Unset port chain properties (python-neutronclient)
  sfc port pair create  Create a port pair (python-neutronclient)
  sfc port pair delete  Delete a given port pair (python-neutronclient)
  sfc port pair group create  Create a port pair group (python-neutronclient)
  sfc port pair group delete  Delete a given port pair group (python-neutronclient)
  sfc port pair group list  List port pair group (python-neutronclient)
  sfc port pair group set  Set port pair group properties (python-neutronclient)
  sfc port pair group show  Display port pair group details (python-neutronclient)
  sfc port pair group unset  Unset port pairs from port pair group (python-neutronclient)
  sfc port pair list  List port pairs (python-neutronclient)
  sfc port pair set  Set port pair properties (python-neutronclient)
  sfc port pair show  Display port pair details (python-neutronclient)
  sfc service graph create  Create a service graph. (python-neutronclient)
  sfc service graph delete  Delete a given service graph. (python-neutronclient)
  sfc service graph list  List service graphs (python-neutronclient)
  sfc service graph set  Set service graph properties (python-neutronclient)
  sfc service graph show  Show information of a given service graph. (python-neutronclient)
  subnet create  Create a subnet
  subnet delete  Delete subnet(s)
  subnet list    List subnets
  subnet pool create  Create subnet pool
  subnet pool delete  Delete subnet pool(s)
  subnet pool list  List subnet pools
  subnet pool set  Set subnet pool properties
  subnet pool show  Display subnet pool details
  subnet pool unset  Unset subnet pool properties
  subnet set     Set subnet properties
  subnet show    Display subnet details
  subnet unset   Unset subnet properties
  tld create     Create new tld (python-designateclient)
  tld delete     Delete tld (python-designateclient)
  tld list       List tlds (python-designateclient)
  tld set        Set tld properties (python-designateclient)
  tld show       Show tld details (python-designateclient)
  token issue    Issue new token
  token revoke   Revoke existing token
  trust create   Create new trust
  trust delete   Delete trust(s)
  trust list     List trusts
  trust show     Display trust details
  tsigkey create  Create new tsigkey (python-designateclient)
  tsigkey delete  Delete tsigkey (python-designateclient)
  tsigkey list   List tsigkeys (python-designateclient)
  tsigkey set    Set tsigkey properties (python-designateclient)
  tsigkey show   Show tsigkey details (python-designateclient)
  usage list     List resource usage per project
  usage show     Show resource usage for a single project
  user create    Create new user
  user delete    Delete user(s)
  user list      List users
  user password set  Change current user password
  user set       Set user properties
  user show      Display user details
  versions show  Show available versions of services
  volume backup create  Create new volume backup
  volume backup delete  Delete volume backup(s)
  volume backup list  List volume backups
  volume backup restore  Restore volume backup
  volume backup set  Set volume backup properties
  volume backup show  Display volume backup details
  volume create  Create new volume
  volume delete  Delete volume(s)
  volume host set  Set volume host properties
  volume list    List volumes
  volume migrate  Migrate volume to a new host
  volume qos associate  Associate a QoS specification to a volume type
  volume qos create  Create new QoS specification
  volume qos delete  Delete QoS specification
  volume qos disassociate  Disassociate a QoS specification from a volume type
  volume qos list  List QoS specifications
  volume qos set  Set QoS specification properties
  volume qos show  Display QoS specification details
  volume qos unset  Unset QoS specification properties
  volume service list  List service command
  volume service set  Set volume service properties
  volume set     Set volume properties
  volume show    Display volume details
  volume snapshot create  Create new volume snapshot
  volume snapshot delete  Delete volume snapshot(s)
  volume snapshot list  List volume snapshots
  volume snapshot set  Set volume snapshot properties
  volume snapshot show  Display volume snapshot details
  volume snapshot unset  Unset volume snapshot properties
  volume transfer request accept  Accept volume transfer request.
  volume transfer request create  Create volume transfer request.
  volume transfer request delete  Delete volume transfer request(s).
  volume transfer request list  Lists all volume transfer requests.
  volume transfer request show  Show volume transfer request details.
  volume type create  Create new volume type
  volume type delete  Delete volume type(s)
  volume type list  List volume types
  volume type set  Set volume type properties
  volume type show  Display volume type details
  volume type unset  Unset volume type properties
  volume unset   Unset volume properties
  vpn endpoint group create  Create an endpoint group (python-neutronclient)
  vpn endpoint group delete  Delete endpoint group(s) (python-neutronclient)
  vpn endpoint group list  List endpoint groups that belong to a given project (python-neutronclient)
  vpn endpoint group set  Set endpoint group properties (python-neutronclient)
  vpn endpoint group show  Display endpoint group details (python-neutronclient)
  vpn ike policy create  Create an IKE policy (python-neutronclient)
  vpn ike policy delete  Delete IKE policy (policies) (python-neutronclient)
  vpn ike policy list  List IKE policies that belong to a given project (python-neutronclient)
  vpn ike policy set  Set IKE policy properties (python-neutronclient)
  vpn ike policy show  Display IKE policy details (python-neutronclient)
  vpn ipsec policy create  Create an IPsec policy (python-neutronclient)
  vpn ipsec policy delete  Delete IPsec policy(policies) (python-neutronclient)
  vpn ipsec policy list  List IPsec policies that belong to a given project (python-neutronclient)
  vpn ipsec policy set  Set IPsec policy properties (python-neutronclient)
  vpn ipsec policy show  Display IPsec policy details (python-neutronclient)
  vpn ipsec site connection create  Create an IPsec site connection (python-neutronclient)
  vpn ipsec site connection delete  Delete IPsec site connection(s) (python-neutronclient)
  vpn ipsec site connection list  List IPsec site connections that belong to a given project (python-neutronclient)
  vpn ipsec site connection set  Set IPsec site connection properties (python-neutronclient)
  vpn ipsec site connection show  Show information of a given IPsec site connection (python-neutronclient)
  vpn service create  Create an VPN service (python-neutronclient)
  vpn service delete  Delete VPN service(s) (python-neutronclient)
  vpn service list  List VPN services that belong to a given project (python-neutronclient)
  vpn service set  Set VPN service properties (python-neutronclient)
  vpn service show  Display VPN service details (python-neutronclient)
  zone abandon   Abandon a zone (python-designateclient)
  zone axfr      AXFR a zone (python-designateclient)
  zone blacklist create  Create new blacklist (python-designateclient)
  zone blacklist delete  Delete blacklist (python-designateclient)
  zone blacklist list  List blacklists (python-designateclient)
  zone blacklist set  Set blacklist properties (python-designateclient)
  zone blacklist show  Show blacklist details (python-designateclient)
  zone create    Create new zone (python-designateclient)
  zone delete    Delete zone (python-designateclient)
  zone export create  Export a Zone (python-designateclient)
  zone export delete  Delete a Zone Export (python-designateclient)
  zone export list  List Zone Exports (python-designateclient)
  zone export show  Show a Zone Export (python-designateclient)
  zone export showfile  Show the zone file for the Zone Export (python-designateclient)
  zone import create  Import a Zone from a file on the filesystem (python-designateclient)
  zone import delete  Delete a Zone Import (python-designateclient)
  zone import list  List Zone Imports (python-designateclient)
  zone import show  Show a Zone Import (python-designateclient)
  zone list      List zones (python-designateclient)
  zone set       Set zone properties (python-designateclient)
  zone show      Show zone details (python-designateclient)
  zone transfer accept list  List Zone Transfer Accepts (python-designateclient)
  zone transfer accept request  Accept a Zone Transfer Request (python-designateclient)
  zone transfer accept show  Show Zone Transfer Accept (python-designateclient)
  zone transfer request create  Create new zone transfer request (python-designateclient)
  zone transfer request delete  Delete a Zone Transfer Request (python-designateclient)
  zone transfer request list  List Zone Transfer Requests (python-designateclient)
  zone transfer request set  Set a Zone Transfer Request (python-designateclient)
  zone transfer request show  Show Zone Transfer Request Details (python-designateclient)
  
  ```
