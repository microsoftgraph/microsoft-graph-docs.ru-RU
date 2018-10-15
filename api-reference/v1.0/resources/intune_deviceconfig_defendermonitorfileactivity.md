# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="2d5f6-101">Тип перечисления defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="2d5f6-101">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="2d5f6-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2d5f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d5f6-103">Возможные значения для наблюдение за действиями над файлом.</span><span class="sxs-lookup"><span data-stu-id="2d5f6-103">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="2d5f6-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="2d5f6-104">Members</span></span>
|<span data-ttu-id="2d5f6-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="2d5f6-105">Member</span></span>|<span data-ttu-id="2d5f6-106">Значение</span><span class="sxs-lookup"><span data-stu-id="2d5f6-106">Value</span></span>|<span data-ttu-id="2d5f6-107">Описание</span><span class="sxs-lookup"><span data-stu-id="2d5f6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d5f6-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="2d5f6-108">userDefined</span></span>|<span data-ttu-id="2d5f6-109">0</span><span class="sxs-lookup"><span data-stu-id="2d5f6-109">0%</span></span>|<span data-ttu-id="2d5f6-110">Определено пользователем, значение по умолчанию, без назначения.</span><span class="sxs-lookup"><span data-stu-id="2d5f6-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="2d5f6-111">disable</span><span class="sxs-lookup"><span data-stu-id="2d5f6-111">disable</span></span>|<span data-ttu-id="2d5f6-112">1</span><span class="sxs-lookup"><span data-stu-id="2d5f6-112">-1</span></span>|<span data-ttu-id="2d5f6-113">Отключение наблюдения за действиями над файлом.</span><span class="sxs-lookup"><span data-stu-id="2d5f6-113">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="2d5f6-114">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="2d5f6-114">monitorAllFiles</span></span>|<span data-ttu-id="2d5f6-115">2</span><span class="sxs-lookup"><span data-stu-id="2d5f6-115">2</span></span>|<span data-ttu-id="2d5f6-116">Наблюдение за всеми файлами.</span><span class="sxs-lookup"><span data-stu-id="2d5f6-116">Monitor all files.</span></span>|
|<span data-ttu-id="2d5f6-117">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="2d5f6-117">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="2d5f6-118">3</span><span class="sxs-lookup"><span data-stu-id="2d5f6-118">3</span></span>| <span data-ttu-id="2d5f6-119">Наблюдение только за входящими файлами.</span><span class="sxs-lookup"><span data-stu-id="2d5f6-119">Monitor incoming files only.</span></span>|
|<span data-ttu-id="2d5f6-120">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="2d5f6-120">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="2d5f6-121">4</span><span class="sxs-lookup"><span data-stu-id="2d5f6-121">4</span></span>|<span data-ttu-id="2d5f6-122">Наблюдение только за исходящими файлами.</span><span class="sxs-lookup"><span data-stu-id="2d5f6-122">Monitor outgoing files only.</span></span>|








