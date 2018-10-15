# <a name="firewallpacketqueueingmethodtype-enum-type"></a><span data-ttu-id="684c8-101">тип перечисления firewallPacketQueueingMethodType</span><span class="sxs-lookup"><span data-stu-id="684c8-101">firewallPacketQueueingMethodType enum type</span></span>

> <span data-ttu-id="684c8-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="684c8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="684c8-103">Возможные значения для firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="684c8-103">Possible values for firewallPacketQueueingMethod</span></span>
## <a name="members"></a><span data-ttu-id="684c8-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="684c8-104">Members</span></span>
|<span data-ttu-id="684c8-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="684c8-105">Member</span></span>|<span data-ttu-id="684c8-106">Значение</span><span class="sxs-lookup"><span data-stu-id="684c8-106">Value</span></span>|<span data-ttu-id="684c8-107">Описание</span><span class="sxs-lookup"><span data-stu-id="684c8-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="684c8-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="684c8-108">deviceDefault</span></span>|<span data-ttu-id="684c8-109">0</span><span class="sxs-lookup"><span data-stu-id="684c8-109">0%</span></span>|<span data-ttu-id="684c8-110">Intune не устанавливает никакого значения, не перезаписывает значение устройства по умолчанию, установленное пользователем</span><span class="sxs-lookup"><span data-stu-id="684c8-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="684c8-111">disabled</span><span class="sxs-lookup"><span data-stu-id="684c8-111">disabled</span></span>|<span data-ttu-id="684c8-112">1</span><span class="sxs-lookup"><span data-stu-id="684c8-112">-1</span></span>|<span data-ttu-id="684c8-113">Отключение очереди пакетов</span><span class="sxs-lookup"><span data-stu-id="684c8-113">Disable packet queuing</span></span>|
|<span data-ttu-id="684c8-114">queueInbound</span><span class="sxs-lookup"><span data-stu-id="684c8-114">queueInbound</span></span>|<span data-ttu-id="684c8-115">2</span><span class="sxs-lookup"><span data-stu-id="684c8-115">2</span></span>|<span data-ttu-id="684c8-116">Установка очереди для входящих зашифрованных пакетов</span><span class="sxs-lookup"><span data-stu-id="684c8-116">Queue inbound encrypted packets</span></span>|
|<span data-ttu-id="684c8-117">queueOutbound</span><span class="sxs-lookup"><span data-stu-id="684c8-117">queueOutbound</span></span>|<span data-ttu-id="684c8-118">3</span><span class="sxs-lookup"><span data-stu-id="684c8-118">3</span></span>|<span data-ttu-id="684c8-119">Установка очереди для исходящих расшифрованных пакетов для пересылки</span><span class="sxs-lookup"><span data-stu-id="684c8-119">Queue decrypted outbound packets for forwarding</span></span>|
|<span data-ttu-id="684c8-120">queueBoth</span><span class="sxs-lookup"><span data-stu-id="684c8-120">queueBoth</span></span>|<span data-ttu-id="684c8-121">4</span><span class="sxs-lookup"><span data-stu-id="684c8-121">4</span></span>|<span data-ttu-id="684c8-122">Установка очереди и для входящих, и для исходящих пакетов</span><span class="sxs-lookup"><span data-stu-id="684c8-122">Queue both inbound and outbound packets</span></span>|








