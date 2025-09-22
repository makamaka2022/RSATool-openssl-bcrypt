## English Version

### Overview
cryptTest.cpp is an encryption testing tool developed based on the Qt framework, providing key management, format conversion, and encryption/decryption testing functionalities for both OpenSSL and Windows BCrypt cryptographic libraries.

### Main Functional Pages

#### 1. OpenSSL Key Test Page (OpenSSLKeyTestPage)
**Function Description:**
- Generate OpenSSL RSA key pairs (supporting 2048-bit and 4096-bit)
- Import/export private and public keys in PEM format
- Display detailed key information (modulus, exponent, etc.)
- Save keys to file system
- Validate key validity and integrity

**Main Controls:**
- Key bit length selection (2048/4096-bit)
- Generate key button
- Import PEM key button
- Export PEM key button
- Key information display area
- Status label showing operation results

#### 2. BCrypt Key Test Page (BCryptKeyTestPage)
**Function Description:**
- Generate Windows BCrypt RSA key pairs
- Import/export keys in BCrypt BLOB format
- Display detailed BLOB header information (Magic value, bit length, modulus bytes, etc.)
- Support key persistence storage
- Provide key validation functionality

**Main Controls:**
- Generate BCrypt key button
- Import BLOB key button
- Export BLOB key button
- BLOB header information display area
- Operation status feedback

#### 3. Encryption/Decryption Test Page (EncryptionTestPage)
**Function Description:**
- Encrypt data using OpenSSL or BCrypt keys
- Support corresponding key decryption operations
- Test chunked encryption/decryption for long data
- Verify encryption/decryption correctness and consistency
- Display data comparison before and after encryption

**Main Controls:**
- Plaintext input text box
- Encryption algorithm selection
- Encrypt/Decrypt buttons
- Result display area
- Performance statistics information

#### 4. Key Format Conversion Page (KeyConversionPage)
**Function Description:**
- Mutual conversion between OpenSSL PEM format and BCrypt BLOB format
- DER format key parsing and conversion
- Display detailed header information during conversion
- Support separate conversion of public and private keys
- Provide conversion result validation

**Main Controls:**
- OpenSSL to BCrypt conversion button
- BCrypt to OpenSSL conversion button
- Conversion result display area
- Header information parsing display
- File save functionality

### Auxiliary Functions

#### Key File Operations
- Support multiple format file saving (PEM, DER, BLOB)
- Automatic file extension handling
- File read/write error handling

#### Information Display
- Detailed BLOB header information parsing
- DER file structure analysis
- Hexadecimal data viewing
- Real-time status feedback

#### Error Handling
- Comprehensive error detection and prompts
- Key validation failure handling
- File operation exception handling
- Memory allocation error handling

### Technical Features
- Developed based on Qt 5 framework
- Integrated OpenSSL cryptographic library
- Uses Windows BCrypt API
- Multi-thread safe design
- Cross-platform compatibility considerations

### Usage Notes
- Requires OpenSSL library installation
- BCrypt functionality is Windows-specific
- Ensure proper file permissions for key storage
- Recommended for testing and development purposes

---


## 中文版本

### 概述
cryptTest.cpp 是一个基于Qt框架开发的加密测试工具，提供OpenSSL和Windows BCrypt加密库的密钥管理、格式转换和加解密测试功能。

### 主要功能页面

#### 1. OpenSSL密钥测试页面 (OpenSSLKeyTestPage)
**功能描述：**
- 生成OpenSSL RSA密钥对（支持2048位和4096位）
- 导入/导出PEM格式的私钥和公钥
- 显示密钥详细信息（模数、指数等）
- 保存密钥到文件系统
- 验证密钥的有效性和完整性

**主要控件：**
- 密钥位数选择（2048/4096位）
- 生成密钥按钮
- 导入PEM密钥按钮
- 导出PEM密钥按钮
- 密钥信息显示区域
- 状态标签显示操作结果

#### 2. BCrypt密钥测试页面 (BCryptKeyTestPage)
**功能描述：**
- 生成Windows BCrypt RSA密钥对
- 导入/导出BCrypt BLOB格式的密钥
- 显示BLOB头部详细信息（Magic值、位长度、模数字节数等）
- 支持密钥持久化存储
- 提供密钥验证功能

**主要控件：**
- 生成BCrypt密钥按钮
- 导入BLOB密钥按钮
- 导出BLOB密钥按钮
- BLOB头部信息显示区域
- 操作状态反馈

#### 3. 加密解密测试页面 (EncryptionTestPage)
**功能描述：**
- 使用OpenSSL或BCrypt密钥进行数据加密
- 支持对应密钥的解密操作
- 测试长数据的分块加密解密
- 验证加解密的正确性和一致性
- 显示加密前后的数据对比

**主要控件：**
- 明文输入文本框
- 加密算法选择
- 加密/解密按钮
- 结果显示区域
- 性能统计信息

#### 4. 密钥格式转换页面 (KeyConversionPage)
**功能描述：**
- OpenSSL PEM格式与BCrypt BLOB格式相互转换
- DER格式密钥解析和转换
- 显示转换过程中的详细头部信息
- 支持公私钥的单独转换
- 提供转换结果验证

**主要控件：**
- OpenSSL转BCrypt转换按钮
- BCrypt转OpenSSL转换按钮
- 转换结果显示区域
- 头部信息解析显示
- 文件保存功能

### 辅助功能

#### 密钥文件操作
- 支持PEM、DER、BLOB等多种格式的文件保存
- 自动处理文件扩展名
- 文件读写错误处理

#### 信息显示
- 详细的BLOB头部信息解析
- DER文件结构分析
- 十六进制数据查看
- 实时状态反馈

#### 错误处理
- 全面的错误检测和提示
- 密钥验证失败处理
- 文件操作异常处理
- 内存分配错误处理

### 技术特性
- 基于Qt 5框架开发
- 集成OpenSSL加密库
- 使用Windows BCrypt API
- 多线程安全设计
- 跨平台兼容性考虑

---


*Document generated based on cryptTest.cpp analysis*
*Last Updated: 2024*