---
title: Тип ресурса Девицеконфигуратионтаржетедусеранддевице
description: Сводка по конфликтам для набора политик конфигурации устройств.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 012a29a7dc0f5cd9fc6332ff99062b6a295792ee
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995905"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="3668b-103">Тип ресурса Девицеконфигуратионтаржетедусеранддевице</span><span class="sxs-lookup"><span data-stu-id="3668b-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="3668b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3668b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3668b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3668b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3668b-106">Сводка по конфликтам для набора политик конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="3668b-106">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="3668b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3668b-107">Properties</span></span>
|<span data-ttu-id="3668b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3668b-108">Property</span></span>|<span data-ttu-id="3668b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3668b-109">Type</span></span>|<span data-ttu-id="3668b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3668b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3668b-111">deviceId</span><span class="sxs-lookup"><span data-stu-id="3668b-111">deviceId</span></span>|<span data-ttu-id="3668b-112">String</span><span class="sxs-lookup"><span data-stu-id="3668b-112">String</span></span>|<span data-ttu-id="3668b-113">Идентификатор устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="3668b-113">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="3668b-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="3668b-114">deviceName</span></span>|<span data-ttu-id="3668b-115">String</span><span class="sxs-lookup"><span data-stu-id="3668b-115">String</span></span>|<span data-ttu-id="3668b-116">Имя устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="3668b-116">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="3668b-117">userId</span><span class="sxs-lookup"><span data-stu-id="3668b-117">userId</span></span>|<span data-ttu-id="3668b-118">String</span><span class="sxs-lookup"><span data-stu-id="3668b-118">String</span></span>|<span data-ttu-id="3668b-119">Идентификатор пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="3668b-119">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="3668b-120">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="3668b-120">userDisplayName</span></span>|<span data-ttu-id="3668b-121">String</span><span class="sxs-lookup"><span data-stu-id="3668b-121">String</span></span>|<span data-ttu-id="3668b-122">Отображаемое имя пользователя в репозитории</span><span class="sxs-lookup"><span data-stu-id="3668b-122">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="3668b-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3668b-123">userPrincipalName</span></span>|<span data-ttu-id="3668b-124">Строка</span><span class="sxs-lookup"><span data-stu-id="3668b-124">String</span></span>|<span data-ttu-id="3668b-125">Имя участника-пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="3668b-125">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="3668b-126">Ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="3668b-126">lastCheckinDateTime</span></span>|<span data-ttu-id="3668b-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3668b-127">DateTimeOffset</span></span>|<span data-ttu-id="3668b-128">Время последнего возврата для этой связи пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="3668b-128">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3668b-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="3668b-129">Relationships</span></span>
<span data-ttu-id="3668b-130">Нет</span><span class="sxs-lookup"><span data-stu-id="3668b-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3668b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3668b-131">JSON Representation</span></span>
<span data-ttu-id="3668b-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3668b-132">Here is a JSON representation of the resource.</span></span>
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





