Bottle Daemon
=============

A simple tool to help make bottle appliations run in the background a unix/linux daemon.

Usage is pretty straighforward:

.. sourcecode:: python

  from bottledaemon import daemon_run
  from bottle import route

  @route("/hello")
  def hello():
    return "Hello World"

  if __name__ == "__main__":
    daemon_run()

The above application will launch in the background. This top-level script can be used to start/stop the background process.
