# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="a7d47-101">Тип ресурса sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a7d47-101">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="a7d47-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a7d47-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7d47-103">Политика диспетчера учетных записей SharedPC.</span><span class="sxs-lookup"><span data-stu-id="a7d47-103">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="a7d47-104">Применяется, только если включен диспетчер учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a7d47-104">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="a7d47-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7d47-105">Properties</span></span>
|<span data-ttu-id="a7d47-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7d47-106">Property</span></span>|<span data-ttu-id="a7d47-107">Тип</span><span class="sxs-lookup"><span data-stu-id="a7d47-107">Type</span></span>|<span data-ttu-id="a7d47-108">Описание</span><span class="sxs-lookup"><span data-stu-id="a7d47-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7d47-109">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="a7d47-109">accountDeletionPolicy</span></span>|[<span data-ttu-id="a7d47-110">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a7d47-110">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune_deviceconfig_sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="a7d47-p102">Настраивает, когда учетные записи удаляются. Возможные значения: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="a7d47-p102">Configures when accounts are deleted. The possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="a7d47-113">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="a7d47-113">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="a7d47-114">Int32</span><span class="sxs-lookup"><span data-stu-id="a7d47-114">Int32</span></span>|<span data-ttu-id="a7d47-115">Задает доступное место на диске в процентах, которое должно быть на компьютере, прежде чем будет прекращено удаление кэшированных учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="a7d47-115">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="a7d47-116">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="a7d47-116">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="a7d47-117">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="a7d47-117">Valid values 0 to 100</span></span>|
|<span data-ttu-id="a7d47-118">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="a7d47-118">inactiveThresholdDays</span></span>|<span data-ttu-id="a7d47-119">Int32</span><span class="sxs-lookup"><span data-stu-id="a7d47-119">Int32</span></span>|<span data-ttu-id="a7d47-120">Указывает, будут ли удаляться учетные записи, если в течение указанного периода (в днях) в них не входили пользователи.</span><span class="sxs-lookup"><span data-stu-id="a7d47-120">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="a7d47-121">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="a7d47-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="a7d47-122">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="a7d47-122">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="a7d47-123">Int32</span><span class="sxs-lookup"><span data-stu-id="a7d47-123">Int32</span></span>|<span data-ttu-id="a7d47-124">Задает минимальное место на диске в процентах, оставшееся на компьютере, при сокращении которого кэшированные учетные записи будут удаляться для освобождения дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="a7d47-124">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="a7d47-125">Сначала будут удалены учетные записи, неактивные в течение самого длинного периода.</span><span class="sxs-lookup"><span data-stu-id="a7d47-125">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="a7d47-126">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="a7d47-126">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="a7d47-127">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="a7d47-127">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7d47-128">Связи</span><span class="sxs-lookup"><span data-stu-id="a7d47-128">Relationships</span></span>
<span data-ttu-id="a7d47-129">Нет</span><span class="sxs-lookup"><span data-stu-id="a7d47-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a7d47-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7d47-130">JSON Representation</span></span>
<span data-ttu-id="a7d47-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7d47-131">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```








