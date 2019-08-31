# imad-
Traceback (most recent call last):
  File "C:\Python27\lib\site-packages\werkzeug\serving.py", line 303, in run_wsgi
    execute(self.server.app)
  File "C:\Python27\lib\site-packages\werkzeug\serving.py", line 291, in execute
    application_iter = app(environ, start_response)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\service\server.py", line 319, in app
    return self.app(e, s)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\service\wsgi_server.py", line 166, in application
    return application_unproxied(environ, start_response)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\service\wsgi_server.py", line 154, in application_unproxied
    result = handler(environ, start_response)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 1321, in __call__
    return self.dispatch(environ, start_response)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 1295, in __call__
    return self.app(environ, start_wrapped)
  File "C:\Python27\lib\site-packages\werkzeug\middleware\shared_data.py", line 220, in __call__
    return self.app(environ, start_response)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 1493, in dispatch
    result = ir_http._dispatch()
  File "d:\openerp_dev\oe_servers\v11\odoo-11.0.post20190829\odoo\addons\base\ir\ir_http.py", line 212, in _dispatch
    return cls._handle_exception(e)
  File "d:\openerp_dev\oe_servers\v11\odoo-11.0.post20190829\odoo\addons\base\ir\ir_http.py", line 182, in _handle_exception
    return request._handle_exception(exception)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 773, in _handle_exception
    return super(HttpRequest, self)._handle_exception(exception)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 312, in _handle_exception
    raise pycompat.reraise(type(exception), exception, sys.exc_info()[2])
  File "d:\openerp_dev\oe_servers\v11\odoo-11.0.post20190829\odoo\addons\base\ir\ir_http.py", line 208, in _dispatch
    result = request.dispatch()
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 832, in dispatch
    r = self._call_function(**self.params)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 344, in _call_function
    return checked_call(self.db, *args, **kwargs)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\service\model.py", line 97, in wrapper
    return f(dbname, *args, **kwargs)
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 340, in checked_call
    result.flatten()
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 1272, in flatten
    self.response.append(self.render())
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\http.py", line 1265, in render
    return env["ir.ui.view"].render_template(self.template, self.qcontext)
  File "d:\openerp_dev\oe_servers\v11\odoo-11.0.post20190829\odoo\addons\base\ir\ir_ui_view.py", line 1211, in render_template
    return self.browse(self.get_view_id(template)).render(values, engine)
  File "d:\openerp_dev\oe_servers\v11\odoo-11.0.post20190829\odoo\addons\base\ir\ir_ui_view.py", line 1118, in get_view_id
    return self.env['ir.model.data'].xmlid_to_res_id(template, raise_if_not_found=True)
  File "d:\openerp_dev\oe_servers\v11\odoo-11.0.post20190829\odoo\addons\base\ir\ir_model.py", line 1360, in xmlid_to_res_id
    return self.xmlid_to_res_model_res_id(xmlid, raise_if_not_found)[1]
  File "d:\openerp_dev\oe_servers\v11\odoo-11.0.post20190829\odoo\addons\base\ir\ir_model.py", line 1351, in xmlid_to_res_model_res_id
    return self.xmlid_lookup(xmlid)[1:3]
  File "<C:\Python27\lib\site-packages\decorator.pyc:decorator-gen-21>", line 2, in xmlid_lookup
    
  File "D:\OpenERP_DEV\OE_Servers\v11\odoo-11.0.post20190829\odoo\tools\cache.py", line 89, in lookup
    value = d[key] = self.method(*args, **kwargs)
  File "d:\openerp_dev\oe_servers\v11\odoo-11.0.post20190829\odoo\addons\base\ir\ir_model.py", line 1340, in xmlid_lookup
    raise ValueError('External ID not found in the system: %s' % xmlid)
ValueError: External ID not found in the system: web.login
