#---------------------------------------------
#添加规则
include ../../Rules.mk

#---------------------------------------------
#~~~~~~引用头文件路径
INC_DIRS += -I../../HawkUtil -I../../HawkProfiler

#---------------------------------------------
#~~~~~~链接库路径,链接库设置
LIB_DIRS += -L../../$(BIN_DIR)
LNK_LIBS += -lhawkutil -lhawkprofiler
GEN_EXE  =  ../../$(BIN_DIR)/profilermonitor
 
#---------------------------------------------
#~~~~~~编译标签设置
all: $(OBJ_FILES)
	$(CPP) $(CPPFLAGS) $(GEN_OBJS) $(LIB_DIRS) $(LNK_LIBS) -o $(GEN_EXE)
	
clean: force
	$(RM) $(OUT_DIR)

force:
