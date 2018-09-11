# <a name="applockerapplicationcontroltype-enum-type"></a><span data-ttu-id="1e27d-101">Тип перечисления appLockerApplicationControlType</span><span class="sxs-lookup"><span data-stu-id="1e27d-101">appLockerApplicationControlType enum type</span></span>

> <span data-ttu-id="1e27d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1e27d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e27d-103">Возможные значения типов управления приложением AppLocker</span><span class="sxs-lookup"><span data-stu-id="1e27d-103">Possible values of AppLocker Application Control Types</span></span>
## <a name="members"></a><span data-ttu-id="1e27d-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="1e27d-104">Members</span></span>
|<span data-ttu-id="1e27d-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="1e27d-105">Member</span></span>|<span data-ttu-id="1e27d-106">Значение</span><span class="sxs-lookup"><span data-stu-id="1e27d-106">Value</span></span>|<span data-ttu-id="1e27d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="1e27d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e27d-108">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1e27d-108">notConfigured</span></span>|<span data-ttu-id="1e27d-109">0</span><span class="sxs-lookup"><span data-stu-id="1e27d-109">0%</span></span>|<span data-ttu-id="1e27d-110">Значение устройства по умолчанию, тип управления приложением не выбран.</span><span class="sxs-lookup"><span data-stu-id="1e27d-110">Device default value, no Application Control type selected.</span></span>|
|<span data-ttu-id="1e27d-111">enforceComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1e27d-111">enforceComponentsAndStoreApps</span></span>|<span data-ttu-id="1e27d-112">1</span><span class="sxs-lookup"><span data-stu-id="1e27d-112">-1</span></span>|<span data-ttu-id="1e27d-113">Принудительное использование компонента и приложений магазина Windows.</span><span class="sxs-lookup"><span data-stu-id="1e27d-113">Enforce Windows component and store apps.</span></span>|
|<span data-ttu-id="1e27d-114">auditComponentsAndStoreApps</span><span class="sxs-lookup"><span data-stu-id="1e27d-114">auditComponentsAndStoreApps</span></span>|<span data-ttu-id="1e27d-115">2</span><span class="sxs-lookup"><span data-stu-id="1e27d-115">2</span></span>|<span data-ttu-id="1e27d-116">Аудит компонента и приложений магазина Windows.</span><span class="sxs-lookup"><span data-stu-id="1e27d-116">Audit Windows component and store apps.</span></span>|
|<span data-ttu-id="1e27d-117">enforceComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1e27d-117">enforceComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1e27d-118">3</span><span class="sxs-lookup"><span data-stu-id="1e27d-118">3</span></span>|<span data-ttu-id="1e27d-119">Принудительное применение компонентов, приложений магазина Windows и smart locker.</span><span class="sxs-lookup"><span data-stu-id="1e27d-119">Enforce Windows components, store apps and smart locker.</span></span>|
|<span data-ttu-id="1e27d-120">auditComponentsStoreAppsAndSmartlocker</span><span class="sxs-lookup"><span data-stu-id="1e27d-120">auditComponentsStoreAppsAndSmartlocker</span></span>|<span data-ttu-id="1e27d-121">4</span><span class="sxs-lookup"><span data-stu-id="1e27d-121">4</span></span>|<span data-ttu-id="1e27d-122">Аудит компонентов, приложений магазина Windows и smart locker.</span><span class="sxs-lookup"><span data-stu-id="1e27d-122">Audit Windows components, store apps and smart locker.</span></span>|








