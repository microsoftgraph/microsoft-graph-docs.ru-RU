# <a name="defenderthreataction-enum-type"></a><span data-ttu-id="e389a-101">Тип перечисления defenderThreatAction</span><span class="sxs-lookup"><span data-stu-id="e389a-101">defenderThreatAction enum type</span></span>

> <span data-ttu-id="e389a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e389a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e389a-103">Действие по умолчанию Защитника для обнаружения угроз вредоносных программ.</span><span class="sxs-lookup"><span data-stu-id="e389a-103">Defender’s default action to take on detected Malware threats.</span></span>
## <a name="members"></a><span data-ttu-id="e389a-104">Члены</span><span class="sxs-lookup"><span data-stu-id="e389a-104">Members</span></span>
|<span data-ttu-id="e389a-105">Член</span><span class="sxs-lookup"><span data-stu-id="e389a-105">Member</span></span>|<span data-ttu-id="e389a-106">Значение</span><span class="sxs-lookup"><span data-stu-id="e389a-106">Value</span></span>|<span data-ttu-id="e389a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="e389a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e389a-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e389a-108">deviceDefault</span></span>|<span data-ttu-id="e389a-109">0</span><span class="sxs-lookup"><span data-stu-id="e389a-109">0%</span></span>|<span data-ttu-id="e389a-110">Применить действие на основе определения обновления.</span><span class="sxs-lookup"><span data-stu-id="e389a-110">Apply action based on the update definition.</span></span>|
|<span data-ttu-id="e389a-111">clean</span><span class="sxs-lookup"><span data-stu-id="e389a-111">clean</span></span>|<span data-ttu-id="e389a-112">1</span><span class="sxs-lookup"><span data-stu-id="e389a-112">-1</span></span>|<span data-ttu-id="e389a-113">Очистить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="e389a-113">Clean the detected threat.</span></span>|
|<span data-ttu-id="e389a-114">quarantine</span><span class="sxs-lookup"><span data-stu-id="e389a-114">Quarantine</span></span>|<span data-ttu-id="e389a-115">2</span><span class="sxs-lookup"><span data-stu-id="e389a-115">2</span></span>|<span data-ttu-id="e389a-116">Карантин обнаруженной угрозы.</span><span class="sxs-lookup"><span data-stu-id="e389a-116">Quarantine the detected threat.</span></span>|
|<span data-ttu-id="e389a-117">remove</span><span class="sxs-lookup"><span data-stu-id="e389a-117">remove</span></span>|<span data-ttu-id="e389a-118">3</span><span class="sxs-lookup"><span data-stu-id="e389a-118">3</span></span>|<span data-ttu-id="e389a-119">Удалить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="e389a-119">Remove the detected threat.</span></span>|
|<span data-ttu-id="e389a-120">allow</span><span class="sxs-lookup"><span data-stu-id="e389a-120">Allow</span></span>|<span data-ttu-id="e389a-121">4</span><span class="sxs-lookup"><span data-stu-id="e389a-121">4</span></span>|<span data-ttu-id="e389a-122">Разрешить обнаруженную угрозу.</span><span class="sxs-lookup"><span data-stu-id="e389a-122">Allow the detected threat.</span></span>|
|<span data-ttu-id="e389a-123">userDefined</span><span class="sxs-lookup"><span data-stu-id="e389a-123">userDefined</span></span>|<span data-ttu-id="e389a-124">5</span><span class="sxs-lookup"><span data-stu-id="e389a-124">5</span></span>|<span data-ttu-id="e389a-125">Разрешает пользователю определить действие, которое нужно предпринять с обнаруженной угрозой.</span><span class="sxs-lookup"><span data-stu-id="e389a-125">Allow the user to determine the action to take with the detected threat.</span></span>|
|<span data-ttu-id="e389a-126">block</span><span class="sxs-lookup"><span data-stu-id="e389a-126">Block</span></span>|<span data-ttu-id="e389a-127">6</span><span class="sxs-lookup"><span data-stu-id="e389a-127">6</span></span>|<span data-ttu-id="e389a-128">Блокировать обнаруженных угроз.</span><span class="sxs-lookup"><span data-stu-id="e389a-128">Block the detected threat.</span></span>|








