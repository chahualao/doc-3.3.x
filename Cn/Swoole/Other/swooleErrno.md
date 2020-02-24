---
title: swoole错误码
meta:
  - name: description
    content: swoole错误码
  - name: keywords
    content: swoole|swoole 拓展|swoole 框架|EasySwoole|swoole|swoole错误码
---

### 错误码

```php
//获取当前错误码
echo swoole_last_error();
//将错误码转换为文字错误
echo swoole_strerror(swoole_last_error(), 9); 
```

### Linux错误码


- define EPERM            1      /* Operation not permitted */
- define ENOENT           2      /* No such file or directory */
- define ESRCH            3      /* No such process */
- define EINTR            4      /* Interrupted system call */
- define EIO              5      /* I/O error */
- define ENXIO            6      /* No such device or address */
- define E2BIG            7      /* Argument list too long */
- define ENOEXEC          8      /* Exec format error */
- define EBADF            9      /* Bad file number */
- define ECHILD          10      /* No child processes */
- define EAGAIN          11      /* Try again */
- define ENOMEM          12      /* Out of memory */
- define EACCES          13      /* Permission denied */
- define EFAULT          14      /* Bad address */
- define ENOTBLK         15      /* Block device required */
- define EBUSY           16      /* Device or resource busy */
- define EEXIST          17      /* File exists */
- define EXDEV           18      /* Cross-device link */
- define ENODEV          19      /* No such device */
- define ENOTDIR         20      /* Not a directory */
- define EISDIR          21      /* Is a directory */
- define EINVAL          22      /* Invalid argument */
- define ENFILE          23      /* File table overflow */
- define EMFILE          24      /* Too many open files */
- define ENOTTY          25      /* Not a typewriter */
- define ETXTBSY         26      /* Text file busy */
- define EFBIG           27      /* File too large */
- define ENOSPC          28      /* No space left on device */
- define ESPIPE          29      /* Illegal seek */
- define EROFS           30      /* Read-only file system */
- define EMLINK          31      /* Too many links */
- define EPIPE           32      /* Broken pipe */
- define EDOM            33      /* Math argument out of domain of func */
- define ERANGE          34      /* Math result not representable */
- define	EDEADLK			35		/* Resource deadlock would occur */
- define	ENAMETOOLONG	36		/* File name too long */
- define	ENOLCK			37		/* No record locks available */
- define	ENOSYS			38		/* Function not implemented */
- define	ENOTEMPTY		39		/* Directory not empty */
- define	ELOOP			40		/* Too many symbolic links encountered */
- define	EWOULDBLOCK	  EAGAIN	/* Operation would block */
- define	ENOMSG			42		/* No message of desired type */
- define	EIDRM			43		/* Identifier removed */
- define	ECHRNG			44		/* Channel number out of range */
- define	EL2NSYNC		45		/* Level 2 not synchronized */
- define	EL3HLT			46		/* Level 3 halted */
- define	EL3RST			47		/* Level 3 reset */
- define	ELNRNG			48		/* Link number out of range */
- define	EUNATCH			49		/* Protocol driver not attached */
- define	ENOCSI			50		/* No CSI structure available */
- define	EL2HLT			51		/* Level 2 halted */
- define	EBADE			52		/* Invalid exchange */
- define	EBADR			53		/* Invalid request descriptor */
- define	EXFULL			54		/* Exchange full */
- define	ENOANO			55		/* No anode */
- define	EBADRQC			56		/* Invalid request code */
- define	EBADSLT			57		/* Invalid slot */
- define	EBFONT			59		/* Bad font file format */
- define	ENOSTR			60		/* Device not a stream */
- define	ENODATA			61		/* No data available */
- define	ETIME			62		/* Timer expired */
- define	ENOSR			63		/* Out of streams resources */
- define	ENONET			64		/* Machine is not on the network */
- define	ENOPKG			65		/* Package not installed */
- define	EREMOTE			66		/* Object is remote */
- define	ENOLINK			67		/* Link has been severed */
- define	EADV			68		/* Advertise error */
- define	ESRMNT			69		/* Srmount error */
- define	ECOMM			70		/* Communication error on send */
- define	EPROTO			71		/* Protocol error */
- define	EMULTIHOP		72		/* Multihop attempted */
- define	EDOTDOT			73		/* RFS specific error */
- define	EBADMSG			74		/* Not a data message */
- define	EOVERFLOW		75		/* Value too large for defined data type */
- define	ENOTUNIQ		76		/* Name not unique on network */
- define	EBADFD			77		/* File descriptor in bad state */
- define	EREMCHG			78		/* Remote address changed */
- define	ELIBACC			79		/* Can not access a needed shared library */
- define	ELIBBAD			80		/* Accessing a corrupted shared library */
- define	ELIBSCN			81		/* .lib section in a.out corrupted */
- define	ELIBMAX			82		/* Attempting to link in too many shared libraries */
- define	ELIBEXEC		83		/* Cannot exec a shared library directly */
- define	EILSEQ			84		/* Illegal byte sequence */
- define	ERESTART		85		/* Interrupted system call should be restarted */
- define	ESTRPIPE		86		/* Streams pipe error */
- define	EUSERS			87		/* Too many users */
- define	ENOTSOCK		88		/* Socket operation on non-socket */
- define	EDESTADDRREQ	89		/* Destination address required */
- define	EMSGSIZE		90		/* Message too long */
- define	EPROTOTYPE		91		/* Protocol wrong type for socket */
- define	ENOPROTOOPT		92		/* Protocol not available */
- define	EPROTONOSUPPORT	93		/* Protocol not supported */
- define	ESOCKTNOSUPPORT	94		/* Socket type not supported */
- define	EOPNOTSUPP		95		/* Operation not supported on transport endpoint */
- define	EPFNOSUPPORT	96		/* Protocol family not supported */
- define	EAFNOSUPPORT	97		/* Address family not supported by protocol */
- define	EADDRINUSE		98		/* Address already in use */
- define	EADDRNOTAVAIL	99		/* Cannot assign requested address */
- define	ENETDOWN		100		/* Network is down */
- define	ENETUNREACH		101		/* Network is unreachable */
- define	ENETRESET		102		/* Network dropped connection because of reset */
- define	ECONNABORTED	103		/* Software caused connection abort */
- define	ECONNRESET		104		/* Connection reset by peer */
- define	ENOBUFS			105		/* No buffer space available */
- define	EISCONN			106		/* Transport endpoint is already connected */
- define	ENOTCONN		107		/* Transport endpoint is not connected */
- define	ESHUTDOWN		108		/* Cannot send after transport endpoint shutdown */
- define	ETOOMANYREFS	109		/* Too many references: cannot splice */
- define	ETIMEDOUT		110		/* Connection timed out */
- define	ECONNREFUSED	111		/* Connection refused */
- define	EHOSTDOWN		112		/* Host is down */
- define	EHOSTUNREACH	113		/* No route to host */
- define	EALREADY		114		/* Operation already in progress */
- define	EINPROGRESS		115		/* Operation now in progress */
- define	ESTALE			116		/* Stale NFS file handle */
- define	EUCLEAN			117		/* Structure needs cleaning */
- define	ENOTNAM			118		/* Not a XENIX named type file */
- define	ENAVAIL			119		/* No XENIX semaphores available */
- define	EISNAM			120		/* Is a named type file */
- define	EREMOTEIO		121		/* Remote I/O error */
- define	EDQUOT			122		/* Quota exceeded */
- define	ENOMEDIUM		123		/* No medium found */
- define	EMEDIUMTYPE		124		/* Wrong medium type */
- define	ECANCELED		125		/* Operation Canceled */
- define	ENOKEY			126		/* Required key not available */
- define	EKEYEXPIRED		127		/* Key has expired */
- define	EKEYREVOKED		128		/* Key has been revoked */
- define	EKEYREJECTED	129		/* Key was rejected by service */
- define	EOWNERDEAD		130		/* Owner died */
- define	ENOTRECOVERABLE	131		* State not recoverable */
- define ERFKILL			132		/* Operation not possible due to RF-kill */

>注意,以上linux错误代码来源于(https://gist.github.com/greggyNapalm/2413028), 如有问题请自行翻译。如有错误请对本文档进行pr  

### Swoole错误码

   标识                                     数字
- SWOOLE_ERROR_MALLOC_FAIL	                501
- SWOOLE_ERROR_SYSTEM_CALL_FAIL	            502
- SWOOLE_ERROR_PHP_FATAL_ERROR	            503
- SWOOLE_ERROR_NAME_TOO_LONG	            504
- SWOOLE_ERROR_INVALID_PARAMS	            505
- SWOOLE_ERROR_QUEUE_FULL	                506
- SWOOLE_ERROR_FILE_NOT_EXIST	            700
- SWOOLE_ERROR_FILE_TOO_LARGE	            701
- SWOOLE_ERROR_FILE_EMPTY	                702
- SWOOLE_ERROR_DNSLOOKUP_DUPLICATE_REQUEST	703
- SWOOLE_ERROR_DNSLOOKUP_RESOLVE_FAILED	    704
- SWOOLE_ERROR_DNSLOOKUP_RESOLVE_TIMEOUT	705
- SWOOLE_ERROR_BAD_IPV6_ADDRESS	            706
- SWOOLE_ERROR_UNREGISTERED_SIGNAL	        707
- SWOOLE_ERROR_SESSION_CLOSED_BY_SERVER	    1001
- SWOOLE_ERROR_SESSION_CLOSED_BY_CLIENT	    1002
- SWOOLE_ERROR_SESSION_CLOSING	            1003
- SWOOLE_ERROR_SESSION_CLOSED	            1004
- SWOOLE_ERROR_SESSION_NOT_EXIST	        1005
- SWOOLE_ERROR_SESSION_INVALID_ID	        1006
- SWOOLE_ERROR_SESSION_DISCARD_TIMEOUT_DATA	1007
- SWOOLE_ERROR_OUTPUT_BUFFER_OVERFLOW	    1008
- SWOOLE_ERROR_SSL_NOT_READY	            1009
- SWOOLE_ERROR_SSL_CANNOT_USE_SENFILE	    1010
- SWOOLE_ERROR_SSL_EMPTY_PEER_CERTIFICATE	1011
- SWOOLE_ERROR_SSL_VEFIRY_FAILED	        1012
- SWOOLE_ERROR_SSL_BAD_CLIENT	            1013
- SWOOLE_ERROR_SSL_BAD_PROTOCOL	            1014
- SWOOLE_ERROR_PACKAGE_LENGTH_TOO_LARGE	    1201
- SWOOLE_ERROR_DATA_LENGTH_TOO_LARGE	    1202
- SWOOLE_ERROR_TASK_PACKAGE_TOO_BIG	        2001
- SWOOLE_ERROR_TASK_DISPATCH_FAIL	        2002
- SWOOLE_ERROR_HTTP2_STREAM_ID_TOO_BIG	    3001
- SWOOLE_ERROR_HTTP2_STREAM_NO_HEADER	    3002
- SWOOLE_ERROR_HTTP2_STREAM_NOT_FOUND	    3003	
- SWOOLE_ERROR_AIO_BAD_REQUEST	            4001	
- SWOOLE_ERROR_AIO_CANCELED	                4002
- SWOOLE_ERROR_CLIENT_NO_CONNECTION         5001
- SWOOLE_ERROR_SOCKET_CLOSED	            5002
- SWOOLE_ERROR_SOCKS5_UNSUPPORT_VERSION	    7001
- SWOOLE_ERROR_SOCKS5_UNSUPPORT_METHOD	    7002
- SWOOLE_ERROR_SOCKS5_AUTH_FAILED	        7003
- SWOOLE_ERROR_SOCKS5_SERVER_ERROR	        7004
- SWOOLE_ERROR_HTTP_PROXY_HANDSHAKE_ERROR	8001
- SWOOLE_ERROR_HTTP_INVALID_PROTOCOL	    8002
- SWOOLE_ERROR_WEBSOCKET_BAD_CLIENT	        8501
- SWOOLE_ERROR_WEBSOCKET_BAD_OPCODE	        8502
- SWOOLE_ERROR_WEBSOCKET_UNCONNECTED	    8503
- SWOOLE_ERROR_WEBSOCKET_HANDSHAKE_FAILED	8504
- SWOOLE_ERROR_SERVER_MUST_CREATED_BEFORE_CLIENT	9001
- SWOOLE_ERROR_SERVER_TOO_MANY_SOCKET	    9002	
- SWOOLE_ERROR_SERVER_WORKER_TERMINATED	    9003	
- SWOOLE_ERROR_SERVER_INVALID_LISTEN_PORT	9004	
- SWOOLE_ERROR_SERVER_TOO_MANY_LISTEN_PORT	9005	
- SWOOLE_ERROR_SERVER_PIPE_BUFFER_FULL	    9006
- SWOOLE_ERROR_SERVER_NO_IDLE_WORKER	    9007
- SWOOLE_ERROR_SERVER_ONLY_START_ONE	    9008
- SWOOLE_ERROR_SERVER_SEND_IN_MASTER	    9009
- SWOOLE_ERROR_SERVER_INVALID_REQUEST	    9010
- SWOOLE_ERROR_SERVER_WORKER_EXIT_TIMEOUT	9011
- SWOOLE_ERROR_CO_OUT_OF_COROUTINE	        10001
- SWOOLE_ERROR_CO_HAS_BEEN_BOUND	        10002
- SWOOLE_ERROR_CO_MUTEX_DOUBLE_UNLOCK	    10003
- SWOOLE_ERROR_CO_BLOCK_OBJECT_LOCKED	    10004
- SWOOLE_ERROR_CO_BLOCK_OBJECT_WAITING	    10005
- SWOOLE_ERROR_CO_YIELD_FAILED	            10006
- SWOOLE_ERROR_CO_GETCONTEXT_FAILED	        10007
- SWOOLE_ERROR_CO_SWOOLEAPCONTEXT_FAILED	10008
- SWOOLE_ERROR_CO_MAKECONTEXT_FAILED	    10009
- SWOOLE_ERROR_CO_IOCPINIT_FAILED	        10010
- SWOOLE_ERROR_CO_PROTECT_STACK_FAILED	    10011
- SWOOLE_ERROR_CO_STD_THREAD_LINK_ERROR	    10012
- SWOOLE_ERROR_CO_DISABLED_MULTI_THREAD