## Install the Intersight Python SDK and import modules

The Python Intersight SDK is available in the [Python Packaging Index](https://pypi.org/)  and installable using the command `pip install intersight`.

> Be sure to running Python >= 3.6 as earlier versions of Python are not supported. Also, uninstall any conflicting versions of the SDK installed on your machine. You can check installed versions with the `pip list` command prior to running `pip install intersight`.

```python
pip install intersight
```

Running the command `pip list` all packages installed by `pip`. Run the command and scroll down to verify the `intersight` pack is installed.

```python
pip list
```

<details><summary>Click here to see output</summary>
<pre><code>
Package                            Version
---------------------------------- -------------------
alabaster                          0.7.12
anaconda-client                    1.7.2
anaconda-navigator                 1.10.0
anaconda-project                   0.8.3
appdirs                            1.4.4
applaunchservices                  0.2.1
appnope                            0.1.0
appscript                          1.1.1
argh                               0.26.2
argon2-cffi                        20.1.0
arrow                              1.1.1
asn1crypto                         1.4.0
astroid                            2.4.2
astropy                            4.0.2
async-generator                    1.10
atomicwrites                       1.4.0
attrs                              20.3.0
autoflake                          1.4
autopep8                           1.5.4
Babel                              2.8.1
backcall                           0.2.0
backports.functools-lru-cache      1.6.1
backports.shutil-get-terminal-size 1.0.0
backports.tempfile                 1.0
backports.weakref                  1.0.post1
bcrypt                             3.2.0
beautifulsoup4                     4.9.3
binaryornot                        0.4.4
bitarray                           1.6.1
bkcharts                           0.2
black                              20.8b1
bleach                             3.2.1
bokeh                              2.2.3
boto                               2.49.0
Bottleneck                         1.3.2
brotlipy                           0.7.0
certifi                            2020.6.20
cffi                               1.14.3
chardet                            3.0.4
click                              7.1.2
cloudpickle                        1.6.0
clyent                             1.2.2
colorama                           0.4.4
conda                              4.9.2
conda-build                        3.20.5
conda-package-handling             1.7.2
conda-verify                       3.4.2
contextlib2                        0.6.0.post1
cookiecutter                       1.7.3
cryptography                       3.1.1
cycler                             0.10.0
Cython                             0.29.21
cytoolz                            0.11.0
dask                               2.30.0
decorator                          4.4.2
defusedxml                         0.6.0
Deprecated                         1.2.12
diff-match-patch                   20200713
distributed                        2.30.1
docutils                           0.16
entrypoints                        0.3
et-xmlfile                         1.0.1
fastcache                          1.1.0
filelock                           3.0.12
flake8                             3.8.4
Flask                              1.1.2
fsspec                             0.8.3
future                             0.18.2
gevent                             20.9.0
glob2                              0.7
gmpy2                              2.0.8
greenlet                           0.4.17
h11                                0.11.0
h5py                               2.10.0
HeapDict                           1.0.1
html5lib                           1.1
httpcore                           0.12.2
httpx                              0.16.1
idna                               2.10
imageio                            2.9.0
imagesize                          1.2.0
importlib-metadata                 2.0.0
iniconfig                          1.1.1
intersight                         1.0.9.4437
intervaltree                       3.1.0
ipykernel                          5.3.4
ipython                            7.19.0
ipython-genutils                   0.2.0
ipywidgets                         7.5.1
isort                              5.6.4
itsdangerous                       1.1.0
jdcal                              1.4.1
jedi                               0.17.1
Jinja2                             2.11.2
jinja2-time                        0.2.0
joblib                             0.17.0
json5                              0.9.5
jsonschema                         3.2.0
jupyter                            1.0.0
jupyter-client                     6.1.7
jupyter-console                    6.2.0
jupyter-core                       4.6.3
jupyterlab                         2.2.6
jupyterlab-pygments                0.1.2
jupyterlab-server                  1.2.0
keyring                            21.4.0
kiwisolver                         1.3.0
lazy-object-proxy                  1.4.3
libarchive-c                       2.9
llvmlite                           0.34.0
locket                             0.2.0
lxml                               4.6.1
MarkupSafe                         1.1.1
matplotlib                         3.3.2
mccabe                             0.6.1
mistune                            0.8.4
mkl-fft                            1.2.0
mkl-random                         1.1.1
mkl-service                        2.3.0
mock                               4.0.2
more-itertools                     8.6.0
mpmath                             1.1.0
msgpack                            1.0.0
multipledispatch                   0.6.0
mypy-extensions                    0.4.3
navigator-updater                  0.2.1
nbclient                           0.5.1
nbconvert                          6.0.7
nbformat                           5.0.8
nest-asyncio                       1.4.2
networkx                           2.5
nltk                               3.5
nose                               1.3.7
notebook                           6.1.4
numba                              0.51.2
numexpr                            2.7.1
numpy                              1.19.2
numpydoc                           1.1.0
olefile                            0.46
openapi-python-client              0.7.3
openpyxl                           3.0.5
packaging                          20.4
pandas                             1.1.3
pandocfilters                      1.4.3
paramiko                           2.7.2
parso                              0.7.0
partd                              1.1.0
path                               15.0.0
pathlib2                           2.3.5
pathspec                           0.8.1
pathtools                          0.1.2
patsy                              0.5.1
pem                                21.2.0
pep8                               1.7.1
pexpect                            4.8.0
pickleshare                        0.7.5
Pillow                             8.0.1
pip                                20.2.4
pkginfo                            1.6.1
pluggy                             0.13.1
ply                                3.11
poyo                               0.5.0
prometheus-client                  0.8.0
prompt-toolkit                     3.0.8
psutil                             5.7.2
ptyprocess                         0.6.0
py                                 1.9.0
pycodestyle                        2.6.0
pycosat                            0.6.3
pycparser                          2.20
pycryptodome                       3.10.1
pycurl                             7.43.0.6
pydantic                           1.7.3
pydocstyle                         5.1.1
pyflakes                           2.2.0
PyGithub                           1.55
Pygments                           2.7.2
PyJWT                              2.1.0
pylint                             2.6.0
PyNaCl                             1.4.0
pyodbc                             4.0.0-unsupported
pyOpenSSL                          19.1.0
pyparsing                          2.4.7
pyrsistent                         0.17.3
PySocks                            1.7.1
pytest                             0.0.0
python-dateutil                    2.8.1
python-jsonrpc-server              0.4.0
python-language-server             0.35.1
python-slugify                     5.0.2
pytz                               2020.1
PyWavelets                         1.1.1
PyYAML                             5.3.1
pyzmq                              19.0.2
QDarkStyle                         2.8.1
QtAwesome                          1.0.1
qtconsole                          4.7.7
QtPy                               1.9.0
regex                              2020.10.15
requests                           2.24.0
rfc3986                            1.4.0
rope                               0.18.0
Rtree                              0.9.4
ruamel-yaml                        0.15.87
scikit-image                       0.17.2
scikit-learn                       0.23.2
scipy                              1.5.2
seaborn                            0.11.0
Send2Trash                         1.5.0
setuptools                         50.3.1.post20201107
shellingham                        1.3.2
simplegeneric                      0.8.1
singledispatch                     3.4.0.3
six                                1.15.0
sniffio                            1.2.0
snowballstemmer                    2.0.0
sortedcollections                  1.2.1
sortedcontainers                   2.2.2
soupsieve                          2.0.1
Sphinx                             3.2.1
sphinxcontrib-applehelp            1.0.2
sphinxcontrib-devhelp              1.0.2
sphinxcontrib-htmlhelp             1.0.3
sphinxcontrib-jsmath               1.0.1
sphinxcontrib-qthelp               1.0.3
sphinxcontrib-serializinghtml      1.1.4
sphinxcontrib-websupport           1.2.4
spyder                             4.1.5
spyder-kernels                     1.9.4
SQLAlchemy                         1.3.20
statsmodels                        0.12.0
stringcase                         1.2.0
sympy                              1.6.2
tables                             3.6.1
tblib                              1.7.0
terminado                          0.9.1
testpath                           0.4.4
text-unidecode                     1.3
threadpoolctl                      2.1.0
tifffile                           2020.10.1
toml                               0.10.1
toolz                              0.11.1
tornado                            6.0.4
tqdm                               4.50.2
traitlets                          5.0.5
typed-ast                          1.4.1
typer                              0.3.2
typing-extensions                  3.7.4.3
ucsmsdk                            0.9.10
ujson                              4.0.1
unicodecsv                         0.14.1
urllib3                            1.25.11
watchdog                           0.10.3
wcwidth                            0.2.5
webencodings                       0.5.1
Werkzeug                           1.0.1
wheel                              0.35.1
widgetsnbextension                 3.5.1
wrapt                              1.11.2
wurlitzer                          2.0.1
xlrd                               1.2.0
XlsxWriter                         1.3.7
xlwings                            0.20.8
xlwt                               1.3.0
xmltodict                          0.12.0
yapf                               0.30.0
zict                               2.0.0
zipp                               3.4.0
zope.event                         4.5.0
zope.interface                     5.1.2
Note: you may need to restart the kernel to use updated packages.
</code></pre>
</details> 

Now that the `intersight` package is installed using `pip` you are ready to import modules needed putting this example together. Start by importing `intersight`, `datetime`, and `timedelta`.

```python
import intersight
import intersight.api.compute_api
```
> Interested in learning more about the `intersight` module? If so, use the command `help(intersight)` to see a description of the module as shown below.

```python
help(intersight)
```
<details><summary>Click here to see output</summary>
<pre><code>
Help on package intersight:

NAME
    intersight - Cisco Intersight

DESCRIPTION
    Cisco Intersight is a management platform delivered as a service with embedded analytics for your Cisco and 3rd party IT infrastructure. This platform offers an intelligent level of management that enables IT organizations to analyze, simplify, and automate their environments in more advanced ways than the prior generations of tools. Cisco Intersight provides an integrated and intuitive management experience for resources in the traditional data center as well as at the edge. With flexible deployment options to address complex security needs, getting started with Intersight is quick and easy. Cisco Intersight has deep integration with Cisco UCS and HyperFlex systems allowing for remote deployment, configuration, and ongoing maintenance. The model-based deployment works for a single system in a remote location or hundreds of systems in a data center and enables rapid, standardized configuration and deployment. It also streamlines maintaining those systems whether you are working with small or very large configurations. The Intersight OpenAPI document defines the complete set of properties that are returned in the HTTP response. From that perspective, a client can expect that no additional properties are returned, unless these properties are explicitly defined in the OpenAPI document. However, when a client uses an older version of the Intersight OpenAPI document, the server may send additional properties because the software is more recent than the client. In that case, the client may receive properties that it does not know about. Some generated SDKs perform a strict validation of the HTTP response body against the OpenAPI document. This document was created on 2021-08-16T17:23:52Z.  # noqa: E501
    
    The version of the OpenAPI document: 1.0.9-4437
    Contact: intersight@cisco.com
    Generated by: https://openapi-generator.tech

PACKAGE CONTENTS
    api (package)
    api_client
    apis (package)
    configuration
    exceptions
    model (package)
    model_utils
    models (package)
    rest
    signing

VERSION
    1.0.9.4437

FILE
    /Users/delgadm/anaconda3/lib/python3.8/site-packages/intersight/__init__.py
</code></pre>
</details> 


## Configuring and Creating the API Client

In step 1, you retrieved your API key and secret key and in this step you apply those values while configuring a newly created API client. The command `help(intersight.Configuration)` displays information about the `Configuration` Python class and its usage.

```python
help(intersight.Configuration)
```

<details><summary>Click here to see output</summary>
<pre><code>
Help on class Configuration in module intersight.configuration:

class Configuration(builtins.object)
 |  Configuration(host=None, api_key=None, api_key_prefix=None, access_token=None, username=None, password=None, discard_unknown_keys=False, disabled_client_side_validations='', signing_info=None, server_index=None, server_variables=None, server_operation_index=None, server_operation_variables=None, ssl_ca_cert=None)
 |  
 |  NOTE: This class is auto generated by OpenAPI Generator
 |  
 |      Ref: https://openapi-generator.tech
 |      Do not edit the class manually.
 |  
 |      :param host: Base url
 |      :param api_key: Dict to store API key(s).
 |        Each entry in the dict specifies an API key.
 |        The dict key is the name of the security scheme in the OAS specification.
 |        The dict value is the API key secret.
 |      :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
 |        The dict key is the name of the security scheme in the OAS specification.
 |        The dict value is an API key prefix when generating the auth data.
 |      :param username: Username for HTTP basic authentication
 |      :param password: Password for HTTP basic authentication
 |      :param discard_unknown_keys: Boolean value indicating whether to discard
 |        unknown properties. A server may send a response that includes additional
 |        properties that are not known by the client in the following scenarios:
 |        1. The OpenAPI document is incomplete, i.e. it does not match the server
 |           implementation.
 |        2. The client was generated using an older version of the OpenAPI document
 |           and the server has been upgraded since then.
 |        If a schema in the OpenAPI document defines the additionalProperties attribute,
 |        then all undeclared properties received by the server are injected into the
 |        additional properties map. In that case, there are undeclared properties, and
 |        nothing to discard.
 |      :param disabled_client_side_validations (string): Comma-separated list of
 |        JSON schema validation keywords to disable JSON schema structural validation
 |        rules. The following keywords may be specified: multipleOf, maximum,
 |        exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
 |        maxItems, minItems.
 |        By default, the validation is performed for data generated locally by the client
 |        and data received from the server, independent of any validation performed by
 |        the server side. If the input data does not satisfy the JSON schema validation
 |        rules specified in the OpenAPI document, an exception is raised.
 |        If disabled_client_side_validations is set, structural validation is
 |        disabled. This can be useful to troubleshoot data validation problem, such as
 |        when the OpenAPI document validation rules do not match the actual API data
 |        received by the server.
 |      :param signing_info: Configuration parameters for the HTTP signature security scheme.
 |          Must be an instance of intersight.signing.HttpSigningConfiguration
 |      :param server_index: Index to servers configuration.
 |      :param server_variables: Mapping with string values to replace variables in
 |        templated server configuration. The validation of enums is performed for
 |        variables with defined enum values before.
 |      :param server_operation_index: Mapping from operation ID to an index to server
 |        configuration.
 |      :param server_operation_variables: Mapping from operation ID to a mapping with
 |        string values to replace variables in templated server configuration.
 |        The validation of enums is performed for variables with defined enum values before.
 |      :param ssl_ca_cert: str - the path to a file of concatenated CA certificates 
 |        in PEM format
 |  
 |      :Example:
 |  
 |      API Key Authentication Example.
 |      Given the following security scheme in the OpenAPI specification:
 |        components:
 |          securitySchemes:
 |            cookieAuth:         # name for the security scheme
 |              type: apiKey
 |              in: cookie
 |              name: JSESSIONID  # cookie name
 |  
 |      You can programmatically set the cookie:
 |  
 |  conf = intersight.Configuration(
 |      api_key={'cookieAuth': 'abc123'}
 |      api_key_prefix={'cookieAuth': 'JSESSIONID'}
 |  )
 |  
 |      The following cookie will be added to the HTTP request:
 |         Cookie: JSESSIONID abc123
 |  
 |      HTTP Signature Authentication Example.
 |      Given the following security scheme in the OpenAPI specification:
 |        components:
 |          securitySchemes:
 |            http_basic_auth:
 |              type: http
 |              scheme: signature
 |  
 |      Configure API client with HTTP signature authentication. Use the 'hs2019' signature scheme,
 |      sign the HTTP requests with the RSA-SSA-PSS signature algorithm, and set the expiration time
 |      of the signature to 5 minutes after the signature has been created.
 |      Note you can use the constants defined in the intersight.signing module, and you can
 |      also specify arbitrary HTTP headers to be included in the HTTP signature, except for the
 |      'Authorization' header, which is used to carry the signature.
 |  
 |      One may be tempted to sign all headers by default, but in practice it rarely works.
 |      This is beccause explicit proxies, transparent proxies, TLS termination endpoints or
 |      load balancers may add/modify/remove headers. Include the HTTP headers that you know
 |      are not going to be modified in transit.
 |  
 |  conf = intersight.Configuration(
 |      signing_info = intersight.signing.HttpSigningConfiguration(
 |          key_id =                 'my-key-id',
 |          private_key_path =       'rsa.pem',
 |          signing_scheme =         intersight.signing.SCHEME_HS2019,
 |          signing_algorithm =      intersight.signing.ALGORITHM_RSASSA_PSS,
 |          signed_headers =         [intersight.signing.HEADER_REQUEST_TARGET,
 |                                      intersight.signing.HEADER_CREATED,
 |                                      intersight.signing.HEADER_EXPIRES,
 |                                      intersight.signing.HEADER_HOST,
 |                                      intersight.signing.HEADER_DATE,
 |                                      intersight.signing.HEADER_DIGEST,
 |                                      'Content-Type',
 |                                      'User-Agent'
 |                                      ],
 |          signature_max_validity = datetime.timedelta(minutes=5)
 |      )
 |  )
 |  
 |  Methods defined here:
 |  
 |  __deepcopy__(self, memo)
 |  
 |  __init__(self, host=None, api_key=None, api_key_prefix=None, access_token=None, username=None, password=None, discard_unknown_keys=False, disabled_client_side_validations='', signing_info=None, server_index=None, server_variables=None, server_operation_index=None, server_operation_variables=None, ssl_ca_cert=None)
 |      Constructor
 |  
 |  __setattr__(self, name, value)
 |      Implement setattr(self, name, value).
 |  
 |  auth_settings(self)
 |      Gets Auth Settings dict for api client.
 |      
 |      :return: The Auth Settings information dict.
 |  
 |  get_api_key_with_prefix(self, identifier, alias=None)
 |      Gets API key (with prefix if set).
 |      
 |      :param identifier: The identifier of apiKey.
 |      :param alias: The alternative identifier of apiKey.
 |      :return: The token for api key authentication.
 |  
 |  get_basic_auth_token(self)
 |      Gets HTTP basic authentication header (string).
 |      
 |      :return: The token for basic HTTP authentication.
 |  
 |  get_host_from_settings(self, index, variables=None, servers=None)
 |      Gets host URL based on the index and variables
 |      :param index: array index of the host settings
 |      :param variables: hash of variable and the corresponding value
 |      :param servers: an array of host settings or None
 |      :return: URL based on host settings
 |  
 |  get_host_settings(self)
 |      Gets an array of host settings
 |      
 |      :return: An array of host settings
 |  
 |  to_debug_report(self)
 |      Gets the essential information for debugging.
 |      
 |      :return: The report for debugging.
 |  
 |  ----------------------------------------------------------------------
 |  Class methods defined here:
 |  
 |  get_default_copy() from builtins.type
 |      Return new instance of configuration.
 |      
 |      This method returns newly created, based on default constructor,
 |      object of Configuration class or returns a copy of default
 |      configuration passed by the set_default method.
 |      
 |      :return: The configuration object.
 |  
 |  set_default(default) from builtins.type
 |      Set default instance of configuration.
 |      
 |      It stores default configuration, which can be
 |      returned by get_default_copy method.
 |      
 |      :param default: object of Configuration
 |  
 |  ----------------------------------------------------------------------
 |  Data descriptors defined here:
 |  
 |  __dict__
 |      dictionary for instance variables (if defined)
 |  
 |  __weakref__
 |      list of weak references to the object (if defined)
 |  
 |  debug
 |      Debug status
 |      
 |      :param value: The debug status, True or False.
 |      :type: bool
 |  
 |  host
 |      Return generated host.
 |  
 |  logger_file
 |      The logger file.
 |      
 |      If the logger_file is None, then add stream handler and remove file
 |      handler. Otherwise, add file handler and remove stream handler.
 |      
 |      :param value: The logger_file path.
 |      :type: str
 |  
 |  logger_format
 |      The logger format.
 |      
 |      The logger_formatter will be updated when sets logger_format.
 |      
 |      :param value: The format string.
 |      :type: str
</code></pre>
</details> 

#### Configure the API Client

Now that `help` provided you with, albeit a lot of background information, you are ready to configurate and create the API client as shown in the example below.

> Keep in mind that the values below are for demonstration purposes only and the values of the variables will not work in your environment or the example below. You use the values of the secret key and API key derived in Step 1. `API Key ID` maps to `key_id` and `Secret Key` maps to `private_key_path` in the example below.

```python
configuration = intersight.Configuration(
    signing_info=intersight.HttpSigningConfiguration(
        key_id='insert-your-api-key-value-here',
        private_key_path='/Users/delgadm/Documents/intersight/intersight-jupyter-notebooks/key/some-secret-key.txt',
        signing_scheme=intersight.signing.SCHEME_HS2019,
        signed_headers=[intersight.signing.HEADER_HOST,
                        intersight.signing.HEADER_DATE,
                        intersight.signing.HEADER_DIGEST,
                        intersight.signing.HEADER_REQUEST_TARGET
                        ]
    )
)
```
#### Create the API Client

Next, create the client and store the resulting handle in the a variable named `api_client` by calling the `Api.Client` class and passing the values stores in `configuration` to it as shown below.
`api_client = intersight.ApiClient(configuration)`

**Next Step: Query the API for Physical Compute Inventory**