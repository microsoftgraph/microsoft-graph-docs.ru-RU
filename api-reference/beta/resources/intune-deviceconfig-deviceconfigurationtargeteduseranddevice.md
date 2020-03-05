---
title: Тип ресурса Девицеконфигуратионтаржетедусеранддевице
description: Сводка по конфликтам для набора политик конфигурации устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d202c50c22cb287f91c18ab6b779d48e971f672c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530149"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="c79c5-103">Тип ресурса Девицеконфигуратионтаржетедусеранддевице</span><span class="sxs-lookup"><span data-stu-id="c79c5-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

<span data-ttu-id="c79c5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c79c5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c79c5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c79c5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c79c5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c79c5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c79c5-107">Сводка по конфликтам для набора политик конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="c79c5-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="c79c5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c79c5-108">Properties</span></span>
|<span data-ttu-id="c79c5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c79c5-109">Property</span></span>|<span data-ttu-id="c79c5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c79c5-110">Type</span></span>|<span data-ttu-id="c79c5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c79c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c79c5-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="c79c5-112">deviceId</span></span>|<span data-ttu-id="c79c5-113">String</span><span class="sxs-lookup"><span data-stu-id="c79c5-113">String</span></span>|<span data-ttu-id="c79c5-114">Идентификатор устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="c79c5-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="c79c5-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="c79c5-115">deviceName</span></span>|<span data-ttu-id="c79c5-116">String</span><span class="sxs-lookup"><span data-stu-id="c79c5-116">String</span></span>|<span data-ttu-id="c79c5-117">Имя устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="c79c5-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="c79c5-118">userId</span><span class="sxs-lookup"><span data-stu-id="c79c5-118">userId</span></span>|<span data-ttu-id="c79c5-119">String</span><span class="sxs-lookup"><span data-stu-id="c79c5-119">String</span></span>|<span data-ttu-id="c79c5-120">Идентификатор пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="c79c5-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="c79c5-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="c79c5-121">userDisplayName</span></span>|<span data-ttu-id="c79c5-122">String</span><span class="sxs-lookup"><span data-stu-id="c79c5-122">String</span></span>|<span data-ttu-id="c79c5-123">Отображаемое имя пользователя в репозитории</span><span class="sxs-lookup"><span data-stu-id="c79c5-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="c79c5-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c79c5-124">userPrincipalName</span></span>|<span data-ttu-id="c79c5-125">Строка</span><span class="sxs-lookup"><span data-stu-id="c79c5-125">String</span></span>|<span data-ttu-id="c79c5-126">Имя участника-пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="c79c5-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="c79c5-127">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="c79c5-127">lastCheckinDateTime</span></span>|<span data-ttu-id="c79c5-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c79c5-128">DateTimeOffset</span></span>|<span data-ttu-id="c79c5-129">Время последнего возврата для этой связи пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="c79c5-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c79c5-130">Связи</span><span class="sxs-lookup"><span data-stu-id="c79c5-130">Relationships</span></span>
<span data-ttu-id="c79c5-131">Нет</span><span class="sxs-lookup"><span data-stu-id="c79c5-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c79c5-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c79c5-132">JSON Representation</span></span>
<span data-ttu-id="c79c5-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c79c5-133">Here is a JSON representation of the resource.</span></span>
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



