# <a name="actionstate-enum-type"></a><span data-ttu-id="c660b-101">Тип перечисления actionState</span><span class="sxs-lookup"><span data-stu-id="c660b-101">actionState enum type</span></span>

> <span data-ttu-id="c660b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c660b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c660b-103">Состояние действие на устройстве</span><span class="sxs-lookup"><span data-stu-id="c660b-103">State of the action on the device</span></span>
## <a name="members"></a><span data-ttu-id="c660b-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="c660b-104">Members</span></span>
|<span data-ttu-id="c660b-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="c660b-105">Member</span></span>|<span data-ttu-id="c660b-106">Значение</span><span class="sxs-lookup"><span data-stu-id="c660b-106">Value</span></span>|<span data-ttu-id="c660b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="c660b-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c660b-108">none</span><span class="sxs-lookup"><span data-stu-id="c660b-108">none</span></span>|<span data-ttu-id="c660b-109">0</span><span class="sxs-lookup"><span data-stu-id="c660b-109">0%</span></span>|<span data-ttu-id="c660b-110">Состояние действия недопустимо</span><span class="sxs-lookup"><span data-stu-id="c660b-110">Not a valid action state</span></span>|
|<span data-ttu-id="c660b-111">pending</span><span class="sxs-lookup"><span data-stu-id="c660b-111">Pending</span></span>|<span data-ttu-id="c660b-112">1</span><span class="sxs-lookup"><span data-stu-id="c660b-112">-1</span></span>|<span data-ttu-id="c660b-113">Действие находится в состоянии ожидания</span><span class="sxs-lookup"><span data-stu-id="c660b-113">Action is pending</span></span>|
|<span data-ttu-id="c660b-114">canceled</span><span class="sxs-lookup"><span data-stu-id="c660b-114">Canceled</span></span>|<span data-ttu-id="c660b-115">2</span><span class="sxs-lookup"><span data-stu-id="c660b-115">2</span></span>|<span data-ttu-id="c660b-116">Действие было отменено.</span><span class="sxs-lookup"><span data-stu-id="c660b-116">Action has been cancelled.</span></span>|
|<span data-ttu-id="c660b-117">active</span><span class="sxs-lookup"><span data-stu-id="c660b-117">Active</span></span>|<span data-ttu-id="c660b-118">3</span><span class="sxs-lookup"><span data-stu-id="c660b-118">3</span></span>|<span data-ttu-id="c660b-119">Действие активно.</span><span class="sxs-lookup"><span data-stu-id="c660b-119">Action is active.</span></span>|
|<span data-ttu-id="c660b-120">done</span><span class="sxs-lookup"><span data-stu-id="c660b-120">done</span></span>|<span data-ttu-id="c660b-121">4</span><span class="sxs-lookup"><span data-stu-id="c660b-121">4</span></span>|<span data-ttu-id="c660b-122">Действие завершено без ошибок.</span><span class="sxs-lookup"><span data-stu-id="c660b-122">Action completed without errors.</span></span>|
|<span data-ttu-id="c660b-123">failed</span><span class="sxs-lookup"><span data-stu-id="c660b-123">failed</span></span>|<span data-ttu-id="c660b-124">5</span><span class="sxs-lookup"><span data-stu-id="c660b-124">5</span></span>|<span data-ttu-id="c660b-125">Действие не удалось</span><span class="sxs-lookup"><span data-stu-id="c660b-125">Action failed</span></span>|
|<span data-ttu-id="c660b-126">notSupported</span><span class="sxs-lookup"><span data-stu-id="c660b-126">notSupported</span></span>|<span data-ttu-id="c660b-127">6</span><span class="sxs-lookup"><span data-stu-id="c660b-127">6</span></span>|<span data-ttu-id="c660b-128">Действие не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c660b-128"> is not supported.</span></span>|








