Import('rtconfig')
from building import *

cwd = GetCurrentDir()
src = []
path = [cwd + '/inc']
libs = []
libpath = [cwd + '/libs']

if rtconfig.CROSS_TOOL == 'gcc':
    libs += ['FTP_gcc']

group = DefineGroup('FTP', src, depend = [''], CPPPATH = path, LIBS = libs, LIBPATH = libpath)

Return('group')
