add_libc_testsuite(libc_errno_unittests)

add_libc_unittest(
  errno_test
  SUITE
    libc_errno_unittests
  SRCS
    errno_test.cpp
  DEPENDS
    __errno_location
)
