SimpleSMTP
==========

A very simple class to send e-mails using the Python SMTP standard lib.

Usage
-----

.. code:: python

    from simplesmtp import SimpleSMTP

    mail = SimpleSMTP(
        host='mail.host',
        username='user@mail.host',
        passw='password',
        from_email='You <youremail@mail.host>'
    )
    mail.send(to_email='email@example.com', subject='Hello', email_message='World')

**Using SSL**

.. code:: python

    from simplesmtp import SimpleSMTP

    mail = SimpleSMTP(
        host='mail.host',
        username='user@mail.host',
        passw='password',
        from_email='You <youremail@mail.host>',
        port=465,
        use_ssl=True
    )
    mail.send(to_email='email@example.com', subject='Hello', email_message='World')