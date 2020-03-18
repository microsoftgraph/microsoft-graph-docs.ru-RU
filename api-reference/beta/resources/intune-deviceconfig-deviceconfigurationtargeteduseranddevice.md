---
title: Тип ресурса Девицеконфигуратионтаржетедусеранддевице
description: Сводка по конфликтам для набора политик конфигурации устройств.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e373dfd4cae79fad4877195544091d054560873
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42793235"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="7769e-103">Тип ресурса Девицеконфигуратионтаржетедусеранддевице</span><span class="sxs-lookup"><span data-stu-id="7769e-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="7769e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7769e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7769e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7769e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7769e-106">Сводка по конфликтам для набора политик конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="7769e-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="7769e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7769e-107">Properties</span></span>
|<span data-ttu-id="7769e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7769e-108">Property</span></span>|<span data-ttu-id="7769e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7769e-109">Type</span></span>|<span data-ttu-id="7769e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7769e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7769e-111">deviceId</span><span class="sxs-lookup"><span data-stu-id="7769e-111">deviceId</span></span>|<span data-ttu-id="7769e-112">String</span><span class="sxs-lookup"><span data-stu-id="7769e-112">String</span></span>|<span data-ttu-id="7769e-113">Идентификатор устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="7769e-113">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="7769e-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="7769e-114">deviceName</span></span>|<span data-ttu-id="7769e-115">String</span><span class="sxs-lookup"><span data-stu-id="7769e-115">String</span></span>|<span data-ttu-id="7769e-116">Имя устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="7769e-116">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="7769e-117">userId</span><span class="sxs-lookup"><span data-stu-id="7769e-117">userId</span></span>|<span data-ttu-id="7769e-118">String</span><span class="sxs-lookup"><span data-stu-id="7769e-118">String</span></span>|<span data-ttu-id="7769e-119">Идентификатор пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="7769e-119">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="7769e-120">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7769e-120">userDisplayName</span></span>|<span data-ttu-id="7769e-121">String</span><span class="sxs-lookup"><span data-stu-id="7769e-121">String</span></span>|<span data-ttu-id="7769e-122">Отображаемое имя пользователя в репозитории</span><span class="sxs-lookup"><span data-stu-id="7769e-122">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="7769e-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7769e-123">userPrincipalName</span></span>|<span data-ttu-id="7769e-124">Строка</span><span class="sxs-lookup"><span data-stu-id="7769e-124">String</span></span>|<span data-ttu-id="7769e-125">Имя участника-пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="7769e-125">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="7769e-126">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="7769e-126">lastCheckinDateTime</span></span>|<span data-ttu-id="7769e-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7769e-127">DateTimeOffset</span></span>|<span data-ttu-id="7769e-128">Время последнего возврата для этой связи пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="7769e-128">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7769e-129">Связи</span><span class="sxs-lookup"><span data-stu-id="7769e-129">Relationships</span></span>
<span data-ttu-id="7769e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="7769e-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7769e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7769e-131">JSON Representation</span></span>
<span data-ttu-id="7769e-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7769e-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```



