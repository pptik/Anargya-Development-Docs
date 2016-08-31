.. Anargya Development Docs documentation master file, created by
   sphinx-quickstart on Wed Aug 31 00:10:22 2016.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Environment
====================================================


.. toctree::
   :maxdepth: 3
   :numbered:


Arsitektur
********************
Lingkungan Anargya terdiri dari beberapa node, seperti yang dijelaskan pada gambar berikut :

.. figure:: arsitektur.png
    :width: 100%
    :align: center
    :alt: alternate text

    Arsitektur Lingkungan Anargya

Secara garis besar lingkungan Anargya terdiri dari empat node utama :

* Server yang menangani urusan Partner, **Partner Server**

* Server yang menagani Operasional (Log, Report, traffic, dll), **Ops Server**

* Server yang melayani aktifitas transaksi, **Trx Server**

* Database

Partner Server
###############

Partner Server berisi sumber kode yang menangani management partner, ditampilkan dalam antarmuka website. Secara garis besar, partner dibagi menjadi dua role : loket dan agen. Agen adalah end user dari lingkungan Anargya, sedangkan diatasnya terdapat loket. Masing-masing bentuk partnership bisa menggunakan layanan antar muka website untuk mengelola akun dan transaksi dengan melakukan login menggunakan role yang telah ditentukan. Data yang dikelola diambil dan disimpan di database, direct dan menggunakan web service tergantung fitur yang digunakan.
