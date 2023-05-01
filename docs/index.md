# Welcome to BrazilCEP

<p align="center">
  <a href="https://pypi.org/project/brazilcep/">
    <img src="static/logo.png" width="20%">
  </a>
</p>

<p align="center">
  <a href="https://coveralls.io/github/mstuttgart/pycep-correios">
    <img alt="Status" src="https://img.shields.io/pypi/status/pycep-correios?style=flat-square">
  </a>
  <a href="https://pypi.org/project/pycep-correios">
      <img src="https://img.shields.io/pypi/dm/pycep-correios?style=flat-square" alt="Downloads">
  </a>
  <a href="https://pypi.org/project/pycep-correios">
      <img src="https://img.shields.io/pypi/v/pycep-correios.svg?style=flat-square" alt="Ratings">
  </a>
  <a href="https://pypi.org/project/pycep-correios/">
      <img src="https://img.shields.io/pypi/pyversions/pycep-correios.svg?style=flat-square" alt="Version">
  </a>
  <a href="https://coveralls.io/github/mstuttgart/pycep-correios">
   <img alt="PyPI - License" src="https://img.shields.io/pypi/l/pycep-correios?color=yellow&style=flat-square">
  </a>
</p>

**BrazilCEP** is a minimalist and easy-to-use python library designed to query CEP (brazilian zip codes) data.

Its objective is to provide a common query interface to all these search services, facilitating the integration of Python applications with these services.

```python
>>> get_address_from_cep('37503-130')
{
    'bairro': 'str',
    'cep': 'str',
    'cidade': 'str',
    'logradouro': 'str',
    'uf': 'str',
    'complemento': 'str',
}
```

## Features

* Cross-platform: Windows, Mac, and Linux are officially supported.
* Works with Python 3.8, 3.9, 3.10 and 3.11.
* Currently supports several CEP API's:
  * [ViaCEP](https://viacep.com.br)
  * [ApiCEP (WideNet)](https://apicep.com)
  * [Correios (SIGEPWeb)](http://www.corporativo.correios.com.br/encomendas/sigepweb/doc/Manual_de_Implementacao_do_Web_Service_SIGEP_WEB.pdf)

BrazilCEP started as a personal study project and evolved into a serious and open source project that is used by many developers on a daily basis.

!!! info
    BrazilCEP is not responsible for the functioning, availability and support of any of these query API's. All of them are provided by third parties, and
    this library just provides a handy way to centralize the CEP search on these services.