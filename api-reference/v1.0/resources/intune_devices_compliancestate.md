# <a name="compliancestate-enum-type"></a><span data-ttu-id="ed70c-101">тип перечисления complianceState</span><span class="sxs-lookup"><span data-stu-id="ed70c-101">complianceState enum type</span></span>

> <span data-ttu-id="ed70c-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ed70c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed70c-103">Состояние соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="ed70c-103">Compliance state.</span></span>
## <a name="members"></a><span data-ttu-id="ed70c-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="ed70c-104">Members</span></span>
|<span data-ttu-id="ed70c-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="ed70c-105">Member</span></span>|<span data-ttu-id="ed70c-106">Значение</span><span class="sxs-lookup"><span data-stu-id="ed70c-106">Value</span></span>|<span data-ttu-id="ed70c-107">Описание</span><span class="sxs-lookup"><span data-stu-id="ed70c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed70c-108">unknown</span><span class="sxs-lookup"><span data-stu-id="ed70c-108">unknown</span></span>|<span data-ttu-id="ed70c-109">0</span><span class="sxs-lookup"><span data-stu-id="ed70c-109">0%</span></span>|<span data-ttu-id="ed70c-110">Неизвестно.</span><span class="sxs-lookup"><span data-stu-id="ed70c-110">Unknown</span></span>|
|<span data-ttu-id="ed70c-111">compliant</span><span class="sxs-lookup"><span data-stu-id="ed70c-111">compliant</span></span>|<span data-ttu-id="ed70c-112">1</span><span class="sxs-lookup"><span data-stu-id="ed70c-112">-1</span></span>|<span data-ttu-id="ed70c-113">Соответствует требованиям.</span><span class="sxs-lookup"><span data-stu-id="ed70c-113">compliant</span></span>|
|<span data-ttu-id="ed70c-114">nonCompliant</span><span class="sxs-lookup"><span data-stu-id="ed70c-114">noncompliant</span></span>|<span data-ttu-id="ed70c-115">2</span><span class="sxs-lookup"><span data-stu-id="ed70c-115">2</span></span>|<span data-ttu-id="ed70c-116">Устройство не соответствует требованиям и заблокировано корпоративными ресурсами.</span><span class="sxs-lookup"><span data-stu-id="ed70c-116">Device is non-compliant and is blocked from corporate resources.</span></span>|
|<span data-ttu-id="ed70c-117">conflict</span><span class="sxs-lookup"><span data-stu-id="ed70c-117">Conflict</span></span>|<span data-ttu-id="ed70c-118">3</span><span class="sxs-lookup"><span data-stu-id="ed70c-118">3</span></span>|<span data-ttu-id="ed70c-119">Конфликт с другими правилами.</span><span class="sxs-lookup"><span data-stu-id="ed70c-119">Conflict with other rules.</span></span>|
|<span data-ttu-id="ed70c-120">error</span><span class="sxs-lookup"><span data-stu-id="ed70c-120">error</span></span>|<span data-ttu-id="ed70c-121">4</span><span class="sxs-lookup"><span data-stu-id="ed70c-121">4</span></span>|<span data-ttu-id="ed70c-122">Ошибка.</span><span class="sxs-lookup"><span data-stu-id="ed70c-122">Error.</span></span>|
|<span data-ttu-id="ed70c-123">inGracePeriod</span><span class="sxs-lookup"><span data-stu-id="ed70c-123">inGracePeriod</span></span>|<span data-ttu-id="ed70c-124">254</span><span class="sxs-lookup"><span data-stu-id="ed70c-124">254</span></span>|<span data-ttu-id="ed70c-125">Устройство не соответствует требованиям, но всё равно имеет доступ к корпоративным ресурсам</span><span class="sxs-lookup"><span data-stu-id="ed70c-125">Device is non-compliant but still has access to corporate resources</span></span>|
|<span data-ttu-id="ed70c-126">configManager</span><span class="sxs-lookup"><span data-stu-id="ed70c-126">configManager</span></span>|<span data-ttu-id="ed70c-127">255</span><span class="sxs-lookup"><span data-stu-id="ed70c-127">255 characters</span></span>|<span data-ttu-id="ed70c-128">Управляется диспетчером конфигурации</span><span class="sxs-lookup"><span data-stu-id="ed70c-128">Managed by Config Manager</span></span>|








