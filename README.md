# character-device-driver

API used in programs are--

 static int __init et_driver_init():- The my_init function is the driver initialization entry point and is called during system startup or when the module is                                                 inserted into the kernel. 
 
 static void __exit et_driver_exit():- The my_exit function is the driver exit point. It’s called when unloading a module from the Linux kernel.
 
 alloc_chrdev_region():- This api is used to allocate the major number dynamically.
 
 dev_t :- is used to hold the device number both major and minor and it is defined in <linux/types.h> library. 

 cdev_init():- The kernel uses cdev structure to represent char devices internally and if we want to read,write,open or close we need to register this structure                       to the driver.It is defined in <linux/cdev.h>.

 cdev_add():- This function is used to register or adding the character driver with the kernel.It is defined in <linux/cdev.h>.

 cdev_del():- This function is used to unregister  the character driver from the kernel.It is defined in <linux/cdev.h>.
 
 copy_to_user():- It copies specific data from the kernel buffer to the buffer allocated in the user space. It is defined in <linux/uaccess.h> 
 
 copy_from_user():-  It copies specific data from the user space to the kernel buffer. It is defined in <linux/uaccess.h>
 
 static int et_open():- This function performs the initialization of a device and filling the specific data.
 
 static int et_release():- The release function is about releasing device specific resources and closing the device.
 
 static ssize_t et_read():- This function reads the data form the device and transfers it to the user space.
 
 static ssize_t et_read():- This function writes the data form the user space and transfers it to the device.
 
 kmalloc():- used to allocate the memory in kernel space.
 
 kfree():- used to free the previously allocated memory in kernel space.
 
 
 
 
 
 
