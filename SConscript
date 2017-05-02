Import('*')

targetEnv.RegisterModule('lwip_contrib', depend=['kernel'])

sources = Split("""
	""")


if targetEnv.has_key('SIMULATION'):
	sources.append('ports/win32/pcapif.c')
	sources.append('ports/win32/pcapif_helper.c')

program_sources.extend(File(sources))
program_objects.extend(targetEnv.StaticObject(sources))

