---
title: Тип ресурса sharedPCAccountManagerPolicy
description: Политика диспетчера учетных записей SharedPC. Применяется, только если включен диспетчер учетных записей.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef25086d573d084e9a4c2917eaa5f56a70bea244
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992460"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="b2310-104">Тип ресурса sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="b2310-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="b2310-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2310-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2310-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2310-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2310-107">Политика диспетчера учетных записей SharedPC.</span><span class="sxs-lookup"><span data-stu-id="b2310-107">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="b2310-108">Применяется, только если включен диспетчер учетных записей.</span><span class="sxs-lookup"><span data-stu-id="b2310-108">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="b2310-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2310-109">Properties</span></span>
|<span data-ttu-id="b2310-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2310-110">Property</span></span>|<span data-ttu-id="b2310-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b2310-111">Type</span></span>|<span data-ttu-id="b2310-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b2310-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2310-113">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="b2310-113">accountDeletionPolicy</span></span>|[<span data-ttu-id="b2310-114">Шаредпкаккаунтделетионполицитипе</span><span class="sxs-lookup"><span data-stu-id="b2310-114">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="b2310-115">Настраивается при удалении учетных записей.</span><span class="sxs-lookup"><span data-stu-id="b2310-115">Configures when accounts are deleted.</span></span> <span data-ttu-id="b2310-116">Возможные значения: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="b2310-116">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="b2310-117">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="b2310-117">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="b2310-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b2310-118">Int32</span></span>|<span data-ttu-id="b2310-119">Задает доступное место на диске в процентах, которое должно быть на компьютере, прежде чем будет прекращено удаление кэшированных учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="b2310-119">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="b2310-120">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b2310-120">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="b2310-121">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="b2310-121">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b2310-122">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="b2310-122">inactiveThresholdDays</span></span>|<span data-ttu-id="b2310-123">Int32</span><span class="sxs-lookup"><span data-stu-id="b2310-123">Int32</span></span>|<span data-ttu-id="b2310-124">Указывает, будут ли удаляться учетные записи, если в течение указанного периода (в днях) в них не входили пользователи.</span><span class="sxs-lookup"><span data-stu-id="b2310-124">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="b2310-125">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b2310-125">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="b2310-126">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="b2310-126">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="b2310-127">Int32</span><span class="sxs-lookup"><span data-stu-id="b2310-127">Int32</span></span>|<span data-ttu-id="b2310-128">Задает минимальное место на диске в процентах, оставшееся на компьютере, при сокращении которого кэшированные учетные записи будут удаляться для освобождения дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="b2310-128">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="b2310-129">Сначала будут удалены учетные записи, неактивные в течение самого длинного периода.</span><span class="sxs-lookup"><span data-stu-id="b2310-129">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="b2310-130">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="b2310-130">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="b2310-131">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="b2310-131">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2310-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="b2310-132">Relationships</span></span>
<span data-ttu-id="b2310-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b2310-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2310-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2310-134">JSON Representation</span></span>
<span data-ttu-id="b2310-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2310-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```





