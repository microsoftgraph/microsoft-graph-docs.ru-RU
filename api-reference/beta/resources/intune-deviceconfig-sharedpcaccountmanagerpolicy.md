---
title: Тип ресурса sharedPCAccountManagerPolicy
description: Политика диспетчера учетных записей SharedPC. Применяется, только если включен диспетчер учетных записей.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ec508868d09264d633d920aeb22dfbdf328daf6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529398"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="67eaf-104">Тип ресурса sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="67eaf-104">sharedPCAccountManagerPolicy resource type</span></span>

<span data-ttu-id="67eaf-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="67eaf-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67eaf-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67eaf-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67eaf-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="67eaf-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67eaf-108">Политика диспетчера учетных записей SharedPC.</span><span class="sxs-lookup"><span data-stu-id="67eaf-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="67eaf-109">Применяется, только если включен диспетчер учетных записей.</span><span class="sxs-lookup"><span data-stu-id="67eaf-109">Only applies when the account manager is enabled.</span></span>

## <a name="properties"></a><span data-ttu-id="67eaf-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="67eaf-110">Properties</span></span>
|<span data-ttu-id="67eaf-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="67eaf-111">Property</span></span>|<span data-ttu-id="67eaf-112">Тип</span><span class="sxs-lookup"><span data-stu-id="67eaf-112">Type</span></span>|<span data-ttu-id="67eaf-113">Описание</span><span class="sxs-lookup"><span data-stu-id="67eaf-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67eaf-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="67eaf-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="67eaf-115">шаредпкаккаунтделетионполицитипе</span><span class="sxs-lookup"><span data-stu-id="67eaf-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="67eaf-116">Настраивается при удалении учетных записей.</span><span class="sxs-lookup"><span data-stu-id="67eaf-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="67eaf-117">Возможные значения: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="67eaf-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="67eaf-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="67eaf-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="67eaf-119">Int32</span><span class="sxs-lookup"><span data-stu-id="67eaf-119">Int32</span></span>|<span data-ttu-id="67eaf-120">Задает доступное место на диске в процентах, которое должно быть на компьютере, прежде чем будет прекращено удаление кэшированных учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="67eaf-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="67eaf-121">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="67eaf-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="67eaf-122">Допустимые значения: от 0 до 100</span><span class="sxs-lookup"><span data-stu-id="67eaf-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="67eaf-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="67eaf-123">inactiveThresholdDays</span></span>|<span data-ttu-id="67eaf-124">Int32</span><span class="sxs-lookup"><span data-stu-id="67eaf-124">Int32</span></span>|<span data-ttu-id="67eaf-125">Указывает, будут ли удаляться учетные записи, если в течение указанного периода (в днях) в них не входили пользователи.</span><span class="sxs-lookup"><span data-stu-id="67eaf-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="67eaf-126">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="67eaf-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="67eaf-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="67eaf-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="67eaf-128">Int32</span><span class="sxs-lookup"><span data-stu-id="67eaf-128">Int32</span></span>|<span data-ttu-id="67eaf-129">Задает минимальное место на диске в процентах, оставшееся на компьютере, при сокращении которого кэшированные учетные записи будут удаляться для освобождения дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="67eaf-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="67eaf-130">Сначала будут удалены учетные записи, неактивные в течение самого длинного периода.</span><span class="sxs-lookup"><span data-stu-id="67eaf-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="67eaf-131">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="67eaf-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="67eaf-132">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="67eaf-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="67eaf-133">Связи</span><span class="sxs-lookup"><span data-stu-id="67eaf-133">Relationships</span></span>
<span data-ttu-id="67eaf-134">Нет</span><span class="sxs-lookup"><span data-stu-id="67eaf-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67eaf-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="67eaf-135">JSON Representation</span></span>
<span data-ttu-id="67eaf-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67eaf-136">Here is a JSON representation of the resource.</span></span>
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



