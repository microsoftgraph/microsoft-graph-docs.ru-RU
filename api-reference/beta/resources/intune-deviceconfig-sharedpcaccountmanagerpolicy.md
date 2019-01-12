---
title: Тип ресурса sharedPCAccountManagerPolicy
description: Политика диспетчера учетных записей SharedPC. Применяется, только если включен диспетчер учетных записей.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42b8824f3f9b18722f69db4f3d0d116b2f46dfd2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914887"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a><span data-ttu-id="13820-104">Тип ресурса sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="13820-104">sharedPCAccountManagerPolicy resource type</span></span>

> <span data-ttu-id="13820-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="13820-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13820-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="13820-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13820-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="13820-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13820-108">Политика диспетчера учетных записей SharedPC.</span><span class="sxs-lookup"><span data-stu-id="13820-108">SharedPC Account Manager Policy.</span></span> <span data-ttu-id="13820-109">Применяется, только если включен диспетчер учетных записей.</span><span class="sxs-lookup"><span data-stu-id="13820-109">Only applies when the account manager is enabled.</span></span>
## <a name="properties"></a><span data-ttu-id="13820-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="13820-110">Properties</span></span>
|<span data-ttu-id="13820-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="13820-111">Property</span></span>|<span data-ttu-id="13820-112">Тип</span><span class="sxs-lookup"><span data-stu-id="13820-112">Type</span></span>|<span data-ttu-id="13820-113">Описание</span><span class="sxs-lookup"><span data-stu-id="13820-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13820-114">accountDeletionPolicy</span><span class="sxs-lookup"><span data-stu-id="13820-114">accountDeletionPolicy</span></span>|[<span data-ttu-id="13820-115">sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="13820-115">sharedPCAccountDeletionPolicyType</span></span>](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|<span data-ttu-id="13820-116">Настраивается при удалении учетных записей.</span><span class="sxs-lookup"><span data-stu-id="13820-116">Configures when accounts are deleted.</span></span> <span data-ttu-id="13820-117">Возможные значения: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span><span class="sxs-lookup"><span data-stu-id="13820-117">Possible values are: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.</span></span>|
|<span data-ttu-id="13820-118">cacheAccountsAboveDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="13820-118">cacheAccountsAboveDiskFreePercentage</span></span>|<span data-ttu-id="13820-119">Int32</span><span class="sxs-lookup"><span data-stu-id="13820-119">Int32</span></span>|<span data-ttu-id="13820-120">Задает доступное место на диске в процентах, которое должно быть на компьютере, прежде чем будет прекращено удаление кэшированных учетных записей на общем компьютере.</span><span class="sxs-lookup"><span data-stu-id="13820-120">Sets the percentage of available disk space a PC should have before it stops deleting cached shared PC accounts.</span></span> <span data-ttu-id="13820-121">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="13820-121">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="13820-122">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="13820-122">Valid values 0 to 100</span></span>|
|<span data-ttu-id="13820-123">inactiveThresholdDays</span><span class="sxs-lookup"><span data-stu-id="13820-123">inactiveThresholdDays</span></span>|<span data-ttu-id="13820-124">Int32</span><span class="sxs-lookup"><span data-stu-id="13820-124">Int32</span></span>|<span data-ttu-id="13820-125">Указывает, будут ли удаляться учетные записи, если в течение указанного периода (в днях) в них не входили пользователи.</span><span class="sxs-lookup"><span data-stu-id="13820-125">Specifies when the accounts will start being deleted when they have not been logged on during the specified period, given as number of days.</span></span> <span data-ttu-id="13820-126">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThreshold или DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="13820-126">Only applies when AccountDeletionPolicy is DiskSpaceThreshold or DiskSpaceThresholdOrInactiveThreshold.</span></span>|
|<span data-ttu-id="13820-127">removeAccountsBelowDiskFreePercentage</span><span class="sxs-lookup"><span data-stu-id="13820-127">removeAccountsBelowDiskFreePercentage</span></span>|<span data-ttu-id="13820-128">Int32</span><span class="sxs-lookup"><span data-stu-id="13820-128">Int32</span></span>|<span data-ttu-id="13820-129">Задает минимальное место на диске в процентах, оставшееся на компьютере, при сокращении которого кэшированные учетные записи будут удаляться для освобождения дискового пространства.</span><span class="sxs-lookup"><span data-stu-id="13820-129">Sets the percentage of disk space remaining on a PC before cached accounts will be deleted to free disk space.</span></span> <span data-ttu-id="13820-130">Сначала будут удалены учетные записи, неактивные в течение самого длинного периода.</span><span class="sxs-lookup"><span data-stu-id="13820-130">Accounts that have been inactive the longest will be deleted first.</span></span> <span data-ttu-id="13820-131">Применяется, только если для свойства AccountDeletionPolicy задано значение DiskSpaceThresholdOrInactiveThreshold.</span><span class="sxs-lookup"><span data-stu-id="13820-131">Only applies when AccountDeletionPolicy is DiskSpaceThresholdOrInactiveThreshold.</span></span> <span data-ttu-id="13820-132">Допустимые значения: от 0 до 100.</span><span class="sxs-lookup"><span data-stu-id="13820-132">Valid values 0 to 100</span></span>|

## <a name="relationships"></a><span data-ttu-id="13820-133">Связи</span><span class="sxs-lookup"><span data-stu-id="13820-133">Relationships</span></span>
<span data-ttu-id="13820-134">Нет</span><span class="sxs-lookup"><span data-stu-id="13820-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13820-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="13820-135">JSON Representation</span></span>
<span data-ttu-id="13820-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="13820-136">Here is a JSON representation of the resource.</span></span>
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





