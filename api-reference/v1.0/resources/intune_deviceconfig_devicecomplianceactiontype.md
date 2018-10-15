# <a name="devicecomplianceactiontype-enum-type"></a><span data-ttu-id="08269-101">Тип перечисления deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="08269-101">deviceComplianceActionType enum type</span></span>

> <span data-ttu-id="08269-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08269-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08269-103">Тип перечисления для типа запланированного действия</span><span class="sxs-lookup"><span data-stu-id="08269-103">Scheduled Action Type Enum</span></span>
## <a name="members"></a><span data-ttu-id="08269-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="08269-104">Members</span></span>
|<span data-ttu-id="08269-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="08269-105">Member</span></span>|<span data-ttu-id="08269-106">Значение</span><span class="sxs-lookup"><span data-stu-id="08269-106">Value</span></span>|<span data-ttu-id="08269-107">Описание</span><span class="sxs-lookup"><span data-stu-id="08269-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08269-108">noAction</span><span class="sxs-lookup"><span data-stu-id="08269-108">noAction</span></span>|<span data-ttu-id="08269-109">0</span><span class="sxs-lookup"><span data-stu-id="08269-109">0%</span></span>|<span data-ttu-id="08269-110">Без действия</span><span class="sxs-lookup"><span data-stu-id="08269-110">No Action</span></span>|
|<span data-ttu-id="08269-111">notification</span><span class="sxs-lookup"><span data-stu-id="08269-111">notification</span></span>|<span data-ttu-id="08269-112">1</span><span class="sxs-lookup"><span data-stu-id="08269-112">-1</span></span>|<span data-ttu-id="08269-113">Отправить уведомление</span><span class="sxs-lookup"><span data-stu-id="08269-113">Send Notification</span></span>|
|<span data-ttu-id="08269-114">block</span><span class="sxs-lookup"><span data-stu-id="08269-114">Block</span></span>|<span data-ttu-id="08269-115">2</span><span class="sxs-lookup"><span data-stu-id="08269-115">2</span></span>|<span data-ttu-id="08269-116">Блокировать устройство в AAD</span><span class="sxs-lookup"><span data-stu-id="08269-116">Block the device in AAD</span></span>|
|<span data-ttu-id="08269-117">retire</span><span class="sxs-lookup"><span data-stu-id="08269-117">retire action</span></span>|<span data-ttu-id="08269-118">3</span><span class="sxs-lookup"><span data-stu-id="08269-118">3</span></span>|<span data-ttu-id="08269-119">Снять устройство с учета</span><span class="sxs-lookup"><span data-stu-id="08269-119">Retire the device</span></span>|
|<span data-ttu-id="08269-120">wipe</span><span class="sxs-lookup"><span data-stu-id="08269-120">wipe action</span></span>|<span data-ttu-id="08269-121">4</span><span class="sxs-lookup"><span data-stu-id="08269-121">4</span></span>|<span data-ttu-id="08269-122">Очистить устройство</span><span class="sxs-lookup"><span data-stu-id="08269-122">Wipe the device</span></span>|
|<span data-ttu-id="08269-123">removeResourceAccessProfiles</span><span class="sxs-lookup"><span data-stu-id="08269-123">removeResourceAccessProfiles</span></span>|<span data-ttu-id="08269-124">5</span><span class="sxs-lookup"><span data-stu-id="08269-124">5</span></span>|<span data-ttu-id="08269-125">Удалить с устройства профили доступа ресурсов</span><span class="sxs-lookup"><span data-stu-id="08269-125">Remove Resource Access Profiles from the device</span></span>|
|<span data-ttu-id="08269-126">pushNotification</span><span class="sxs-lookup"><span data-stu-id="08269-126">pushNotification</span></span>|<span data-ttu-id="08269-127">9</span><span class="sxs-lookup"><span data-stu-id="08269-127"> :=9</span></span>|<span data-ttu-id="08269-128">Отправить push-уведомление устройству</span><span class="sxs-lookup"><span data-stu-id="08269-128">Send push notification to device</span></span>|








