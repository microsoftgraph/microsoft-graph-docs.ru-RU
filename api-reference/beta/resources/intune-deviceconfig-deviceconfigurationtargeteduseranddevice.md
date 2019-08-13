---
title: Тип ресурса Девицеконфигуратионтаржетедусеранддевице
description: Сводка по конфликтам для набора политик конфигурации устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d994491b86d1590c5765d5771ea52b24d6e42f8b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332934"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="2cc98-103">Тип ресурса Девицеконфигуратионтаржетедусеранддевице</span><span class="sxs-lookup"><span data-stu-id="2cc98-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="2cc98-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cc98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cc98-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cc98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cc98-106">Сводка по конфликтам для набора политик конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="2cc98-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="2cc98-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cc98-107">Properties</span></span>
|<span data-ttu-id="2cc98-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cc98-108">Property</span></span>|<span data-ttu-id="2cc98-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2cc98-109">Type</span></span>|<span data-ttu-id="2cc98-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2cc98-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cc98-111">deviceId</span><span class="sxs-lookup"><span data-stu-id="2cc98-111">deviceId</span></span>|<span data-ttu-id="2cc98-112">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-112">String</span></span>|<span data-ttu-id="2cc98-113">Идентификатор устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="2cc98-113">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="2cc98-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="2cc98-114">deviceName</span></span>|<span data-ttu-id="2cc98-115">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-115">String</span></span>|<span data-ttu-id="2cc98-116">Имя устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="2cc98-116">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="2cc98-117">userId</span><span class="sxs-lookup"><span data-stu-id="2cc98-117">userId</span></span>|<span data-ttu-id="2cc98-118">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-118">String</span></span>|<span data-ttu-id="2cc98-119">Идентификатор пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="2cc98-119">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="2cc98-120">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2cc98-120">userDisplayName</span></span>|<span data-ttu-id="2cc98-121">String</span><span class="sxs-lookup"><span data-stu-id="2cc98-121">String</span></span>|<span data-ttu-id="2cc98-122">Отображаемое имя пользователя в репозитории</span><span class="sxs-lookup"><span data-stu-id="2cc98-122">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="2cc98-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2cc98-123">userPrincipalName</span></span>|<span data-ttu-id="2cc98-124">Строка</span><span class="sxs-lookup"><span data-stu-id="2cc98-124">String</span></span>|<span data-ttu-id="2cc98-125">Имя участника-пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="2cc98-125">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="2cc98-126">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="2cc98-126">lastCheckinDateTime</span></span>|<span data-ttu-id="2cc98-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2cc98-127">DateTimeOffset</span></span>|<span data-ttu-id="2cc98-128">Время последнего возврата для этой связи пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="2cc98-128">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cc98-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="2cc98-129">Relationships</span></span>
<span data-ttu-id="2cc98-130">Нет</span><span class="sxs-lookup"><span data-stu-id="2cc98-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cc98-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2cc98-131">JSON Representation</span></span>
<span data-ttu-id="2cc98-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cc98-132">Here is a JSON representation of the resource.</span></span>
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



