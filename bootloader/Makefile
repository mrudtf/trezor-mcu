NAME  = bootloader

OBJS += bootloader.o
OBJS += signatures.o
OBJS += usb.o

OBJS += ../vendor/trezor-crypto/bignum.o
OBJS += ../vendor/trezor-crypto/ecdsa.small.o
OBJS += ../vendor/trezor-crypto/hmac.o
OBJS += ../vendor/trezor-crypto/ripemd160.o
OBJS += ../vendor/trezor-crypto/secp256k1.small.o
OBJS += ../vendor/trezor-crypto/sha2.o

CFLAGS += -DUSE_PRECOMPUTED_IV=0
CFLAGS += -DUSE_PRECOMPUTED_CP=0

include ../Makefile.include

align:
	./firmware_align.py $(NAME).bin
