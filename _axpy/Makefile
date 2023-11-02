#makefile

start:
	#rm bin/*.*

serial:
	echo "serial"
#	${LLVM}/bin/clang -mepi -Wall --target=riscv64-unknown-elf -march=rv64g -O2 -c -o src/axpy_serial.o src/axpy.c
#	${LLVM}/bin/clang -mepi -Wall --target=riscv64-unknown-elf -march=rv64g -O2 -c -o src/main_serial.o src/main.c
#	${LLVM}/bin/clang -mepi -Wall --target=riscv64-unknown-elf -march=rv64g -O2 -c -o src/utils_serial.o src/utils.c
#	${LLVM}/bin/clang -mepi -Wall --target=riscv64-unknown-elf -march=rv64g -O2 -o bin/axpy_serial.exe src/*.o -lm
#	rm src/*.o
#	${LLVM}/bin/llvm-objdump  -mattr=+m,+f,+d,+a,+c,+epi -ds  bin/axpy_serial.exe > bin/axpy_serial.dump

#vector:
#	echo "vector"
#	${LLVM}/bin/clang --target=riscv64-unknown-elf -march=rv64imafdcv -menable-experimental-extensions -v -O2 -c -o src/utils.o src/utils.c 
#	${LLVM}/bin/clang --target=riscv64-unknown-elf -march=rv64imafdcv -menable-experimental-extensions -v -mepi -DUSE_RISCV_VECTOR -fno-vectorize -O2 -c -o src/axpy.o src/axpy.c
#	${LLVM}/bin/clang --target=riscv64-unknown-elf -march=rv64imafdcv -menable-experimental-extensions -v -O2 -c -o src/main.o src/main.c
#	${LLVM}/bin/clang --target=riscv64-unknown-elf -march=rv64imafdcv -menable-experimental-extensions -v -O2 -o bin/axpy_vector.exe src/*.o -lm
#	rm src/*.o
#	${LLVM}/bin/llvm-objdump  --mattr=+m,+f,+d,+a,+c,+experimental-v -ds  bin/axpy_vector.exe > bin/axpy_vector.dump

#clean:
#	rm bin/*.dump; \
#	rm bin/*.exe;



#vector:
#	echo "vector"
#	${LLVM}/bin/clang --target=riscv64-unknown-linux-gnu -march=rv64imafdc -menable-experimental-extensions -O2 -c -o src/utils.o src/utils.c
#	${LLVM}/bin/clang --target=riscv64-unknown-linux-gnu -march=rv64imafdc -menable-experimental-extensions -DUSE_RISCV_VECTOR -fno-vectorize -O2 -c -o src/axpy.o src/axpy.c
#	${LLVM}/bin/clang --target=riscv64-unknown-linux-gnu -march=rv64imafdc -menable-experimental-extensions -O2 -c -o src/main.o src/main.c
#	${LLVM}/bin/clang --target=riscv64-unknown-linux-gnu -march=rv64imafdc -menable-experimental-extensions -O2 -o bin/axpy_vector.exe src/*.o -lm
#	rm src/*.o
#	${LLVM}/bin/llvm-objdump  --mattr=+m,+f,+d,+a,+c,+experimental-v -ds  bin/axpy_vector.exe > bin/axpy_vector.dump

#clean:
#	rm bin/*.dump; \
#	rm bin/*.exe;
	
	
#vector:
#	echo "vector"
#	${LLVM}/bin/clang -target riscv64-unknown-linux-gnu -march=rv64imafdc -O2 -c -g -o src/utils.o src/utils.c 
#	${LLVM}/bin/clang -target riscv64-unknown-linux-gnu -march=rv64imafdc -mepi -g -DUSE_RISCV_VECTOR -fno-vectorize -O2 -c -o src/axpy.o src/axpy.c
#	${LLVM}/bin/clang -target riscv64-unknown-linux-gnu -march=rv64imafdc  -O2 -c -g -o src/main.o src/main.c 
#	${LLVM}/bin/clang -target riscv64-unknown-linux-gnu -march=rv64imafdc  -O2 -g -o bin/axpy_vector.exe src/*.o -lm
#	rm src/*.o
#	${LLVM}/bin/llvm-objdump  --mattr=+m,+f,+d,+a,+c,+experimental-v -ds  bin/axpy_vector.exe > bin/axpy_vector.dump

#clean:
#	rm bin/*.dump; \
#	rm bin/*.exe;





vector:
	echo "vector"
	${LLVM}/bin/clang --target=riscv64-unknown-elf -march=rv64imafdc -O2 -c -o src/utils.o src/utils.c 
	${LLVM}/bin/clang --target=riscv64-unknown-elf -march=rv64imafdc -mepi -DUSE_RISCV_VECTOR -fno-vectorize -O2 -c -o src/axpy.o src/axpy.c
	${LLVM}/bin/clang --target=riscv64-unknown-elf -march=rv64imafdc -O2 -c -o src/main.o src/main.c
	${LLVM}/bin/clang --target=riscv64-unknown-elf -march=rv64imafdc -O2 -g -o bin/axpy_vector.exe src/*.o -lm
	rm src/*.o
	${LLVM}/bin/llvm-objdump  --mattr=+m,+f,+d,+a,+c,+experimental-v -ds  bin/axpy_vector.exe > bin/axpy_vector.dump

clean:
	rm bin/*.dump; \
	rm bin/*.exe;
