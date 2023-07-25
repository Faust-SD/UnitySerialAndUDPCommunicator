# UnitySerialAndUDPCommunicator
UnitySerialAndUDPCommunicator 是一个Unity的脚本，它可以通过串行或UDP通讯接口从外部设备接收数据。

## 功能
- 提供了对串行和UDP通讯的支持。
- 通过Unity Inspector设置通讯接口参数和优先级。
- 当通讯发生错误时，脚本会自动重试，直到连接成功。

## 使用场景
如果你的项目需要从一个或多个设备（如Arduino控制器、传感器或其他计算机）接收数据，那么这个脚本可以为你节省时间。它为你处理了连接和数据接收的部分，你只需要处理数据的使用。

## 如何使用
1. 把脚本添加到你的Unity游戏对象上。
2. 在Inspector中设置串行端口名（如`COM3`）、波特率（如`115200`）以及UDP端口（如`8000`）。
3. 设置通讯类型的优先级。脚本会按照这个列表的顺序尝试建立通讯连接。
4. 通过 `dataQueue` 接收数据。这是一个线程安全的队列，你可以从任何线程中安全地读取数据。

## 示例
[Dynamic-Light-Control-with-Hybrid-Communication](https://github.com/Faust-SD/Dynamic-Light-Control-with-Hybrid-Communication)


# UnitySerialAndUDPCommunicator
UnitySerialAndUDPCommunicator is a Unity MonoBehaviour script that enables data reception from external devices through serial or UDP communications.

## Features
- Supports both serial and UDP communications.
- Configure communication interface parameters and priority through Unity Inspector.
- Automatically retries the connection until successful when a communication error occurs.

## Use Cases
If your project needs to receive data from one or more devices, such as Arduino controllers, sensors, or other computers, this script can save you time. It handles the connection and data reception part, you just deal with the use of data.

## How to Use
1. Add the script to your Unity game object.
2. Set the serial port name (like `COM3`), baud rate (like `115200`), and UDP port (like `8000`) in the Inspector.
3. Set the priority of communication types. The script will try to establish a communication connection in the order of this list.
4. Receive data through `dataQueue`. This is a thread-safe queue, and you can safely read data from any thread.

## Examples
[Dynamic-Light-Control-with-Hybrid-Communication](https://github.com/Faust-SD/Dynamic-Light-Control-with-Hybrid-Communication)
