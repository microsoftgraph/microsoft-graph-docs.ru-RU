---
title: Тип ресурса sharedPCAccountManagerPolicy
description: Политика диспетчера учетных записей SharedPC. Применяется, только если включен диспетчер учетных записей.
author: tfitzmac
ms.openlocfilehash: 7eafffbfac115c95cbf2c62be630cf7958965ce9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306568"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="a113e-104">Тип ресурса sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a113e-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="a113e-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a113e-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a113e-106">Политика диспетчера учетных записей SharedPC.</span><span class="sxs-lookup"><span data-stu-id="a113e-106">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="a113e-107">Применяется, только если включен диспетчер учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a113e-107">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="a113e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a113e-108">Properties</span></span>
|<span data-ttu-id="a113e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a113e-109">Property</span></span>|<span data-ttu-id="a113e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a113e-110">Type</span></span>|<span data-ttu-id="a113e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a113e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a113e-112">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="a113e-112">accountDeletionPolicy</span></span>|[<span data-ttu-id="a113e-113">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a113e-113">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="a113e-114">Настраивается при удалении учетных записей.</span><span class="sxs-lookup"><span data-stu-id="a113e-114">Configures when accounts are deleted.</span></span> <span data-ttu-id="a113e-115">Возможные значения: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="a113e-115">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="a113e-116">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="a113e-116">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="a113e-117">Int32</span><span class="sxs-lookup"><span data-stu-id="a113e-117">Int32</span></span>|<span data-ttu-id="a113e-118">Задает доступное место на диске в процентах, которое должно быть на компьютере, прежде чем будет прекращено удаление кэшированных учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="a113e-118">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="a113e-119">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="a113e-119">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="a113e-120">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="a113e-120">Valid values 0 to 100</span></span>|
|<span data-ttu-id="a113e-121">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="a113e-121">inactiveThresholdDays</span></span>|<span data-ttu-id="a113e-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a113e-122">Int32</span></span>|<span data-ttu-id="a113e-123">Указывает, будут ли удаляться учетные записи, если в течение указанного периода (в днях) в них не входили пользователи.</span><span class="sxs-lookup"><span data-stu-id="a113e-123">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="a113e-124">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="a113e-124">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="a113e-125">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="a113e-125">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="a113e-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a113e-126">Int32</span></span>|<span data-ttu-id="a113e-127">Задает минимальное место на диске в процентах, оставшееся на компьютере, при сокращении которого кэшированные учетные записи будут удаляться для освобождения дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="a113e-127">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="a113e-128">Сначала будут удалены учетные записи, неактивные в течение самого длинного периода.</span><span class="sxs-lookup"><span data-stu-id="a113e-128">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="a113e-129">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="a113e-129">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="a113e-130">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="a113e-130">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="a113e-131">Связи</span><span class="sxs-lookup"><span data-stu-id="a113e-131">Relationships</span></span>
<span data-ttu-id="a113e-132">Нет</span><span class="sxs-lookup"><span data-stu-id="a113e-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a113e-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a113e-133">JSON Representation</span></span>
<span data-ttu-id="a113e-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a113e-134">Here is a JSON representation of the resource.</span></span>
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



