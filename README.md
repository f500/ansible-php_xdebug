php_xdebug
========

Install xdebug extension for PHP

Requirements
------------

Debian Wheezy with the package python-pycurl and python-software-properties installed.

Role Variables
--------------

    php_xdebug_auto_trace: 0
    php_xdebug_cli_color: 0
    php_xdebug_collect_assignments: 0
    php_xdebug_collect_includes: 1
    php_xdebug_collect_params: 0
    php_xdebug_collect_return: 0
    php_xdebug_collect_vars: 0
    php_xdebug_coverage_enable: 1
    php_xdebug_default_enable: 1
    php_xdebug_dump_globals: 1
    php_xdebug_dump_once: 1
    php_xdebug_dump_undefined: 0
    php_xdebug_extended_info: 1
    php_xdebug_file_link_format: ~
    php_xdebug_force_display_errors: 0
    php_xdebug_force_error_reporting: 0
    php_xdebug_halt_level: 0
    php_xdebug_idekey: ~
    php_xdebug_manual_url: 'http://www.php.net'
    php_xdebug_max_nesting_level: 100
    php_xdebug_overload_var_dump: 1
    php_xdebug_profiler_append: 0
    php_xdebug_profiler_enable: 0
    php_xdebug_profiler_enable_trigger: 0
    php_xdebug_profiler_output_dir: '/tmp'
    php_xdebug_profiler_output_name: 'cachegrind.out.%p'
    php_xdebug_remote_autostart: 0
    php_xdebug_remote_connect_back: 0
    php_xdebug_remote_cookie_expire_time: 3600
    php_xdebug_remote_enable: 0
    php_xdebug_remote_handler: dbgp
    php_xdebug_remote_host: localhost
    php_xdebug_remote_log: ~
    php_xdebug_remote_mode: req
    php_xdebug_remote_port: 9000
    php_xdebug_scream: 0
    php_xdebug_show_exception_trace: 0
    php_xdebug_show_local_vars: 0
    php_xdebug_show_mem_delta: 0
    php_xdebug_trace_enable_trigger: 0
    php_xdebug_trace_format: 0
    php_xdebug_trace_options: 0
    php_xdebug_trace_output_dir: '/tmp'
    php_xdebug_trace_output_name: 'trace.%c'
    php_xdebug_var_display_max_children: 128
    php_xdebug_var_display_max_data: 512
    php_xdebug_var_display_max_depth: 3

    # available: apache2, apache2filter, cgi, cli, fpm
    php_xdebug_versions: []

Dependencies
------------

Depends on f500.repo_dotdeb.

Example Playbook
-------------------------

    - hosts: servers
      roles:
         - { role: f500.php_xdebug }

License
-------

LGPL

Author Information
------------------

Jasper N. Brouwer, jasper@nerdsweide.nl

Ramon de la Fuente, ramon@delafuente.nl
