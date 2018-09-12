# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="757af-101">тип перечисления automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="757af-101">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="757af-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="757af-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="757af-103">Возможные значения для режима автоматического обновления.</span><span class="sxs-lookup"><span data-stu-id="757af-103">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="757af-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="757af-104">Members</span></span>
|<span data-ttu-id="757af-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="757af-105">Member</span></span>|<span data-ttu-id="757af-106">Значение</span><span class="sxs-lookup"><span data-stu-id="757af-106">Value</span></span>|<span data-ttu-id="757af-107">Описание</span><span class="sxs-lookup"><span data-stu-id="757af-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="757af-108">userDefined</span><span class="sxs-lookup"><span data-stu-id="757af-108">userDefined</span></span>|<span data-ttu-id="757af-109">0</span><span class="sxs-lookup"><span data-stu-id="757af-109">0%</span></span>|<span data-ttu-id="757af-110">Определено пользователем, значение по умолчанию, без назначения.</span><span class="sxs-lookup"><span data-stu-id="757af-110">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="757af-111">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="757af-111">notifyDownload</span></span>|<span data-ttu-id="757af-112">1</span><span class="sxs-lookup"><span data-stu-id="757af-112">-1</span></span>|<span data-ttu-id="757af-113">Уведомление при загрузке.</span><span class="sxs-lookup"><span data-stu-id="757af-113">Notify on download.</span></span>|
|<span data-ttu-id="757af-114">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="757af-114">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="757af-115">2</span><span class="sxs-lookup"><span data-stu-id="757af-115">2</span></span>|<span data-ttu-id="757af-116">Автоматическая установка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="757af-116">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="757af-117">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="757af-117">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="757af-118">3</span><span class="sxs-lookup"><span data-stu-id="757af-118">3</span></span>|<span data-ttu-id="757af-119">Автоматическая установка и перезагрузка во время обслуживания.</span><span class="sxs-lookup"><span data-stu-id="757af-119">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="757af-120">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="757af-120">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="757af-121">4</span><span class="sxs-lookup"><span data-stu-id="757af-121">4</span></span>|<span data-ttu-id="757af-122">Автоматическая установка и перезагрузка в запланированное время.</span><span class="sxs-lookup"><span data-stu-id="757af-122">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="757af-123">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="757af-123">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="757af-124">5</span><span class="sxs-lookup"><span data-stu-id="757af-124">5</span></span>|<span data-ttu-id="757af-125">Автоматическая установка и перезагрузка без управления со стороны конечных пользователей</span><span class="sxs-lookup"><span data-stu-id="757af-125">Auto-install and restart without end-user control</span></span>|








