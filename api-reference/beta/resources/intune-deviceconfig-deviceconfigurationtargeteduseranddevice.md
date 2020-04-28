---
title: Тип ресурса Девицеконфигуратионтаржетедусеранддевице
description: Сводка по конфликтам для набора политик конфигурации устройств.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a553cf15a82b25d78eb983037d45c1c3c245025
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469369"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="71c0f-103">Тип ресурса Девицеконфигуратионтаржетедусеранддевице</span><span class="sxs-lookup"><span data-stu-id="71c0f-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

<span data-ttu-id="71c0f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71c0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71c0f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71c0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71c0f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71c0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71c0f-107">Сводка по конфликтам для набора политик конфигурации устройств.</span><span class="sxs-lookup"><span data-stu-id="71c0f-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="71c0f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="71c0f-108">Properties</span></span>
|<span data-ttu-id="71c0f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="71c0f-109">Property</span></span>|<span data-ttu-id="71c0f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="71c0f-110">Type</span></span>|<span data-ttu-id="71c0f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="71c0f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71c0f-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="71c0f-112">deviceId</span></span>|<span data-ttu-id="71c0f-113">String</span><span class="sxs-lookup"><span data-stu-id="71c0f-113">String</span></span>|<span data-ttu-id="71c0f-114">Идентификатор устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="71c0f-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="71c0f-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="71c0f-115">deviceName</span></span>|<span data-ttu-id="71c0f-116">String</span><span class="sxs-lookup"><span data-stu-id="71c0f-116">String</span></span>|<span data-ttu-id="71c0f-117">Имя устройства в возврате.</span><span class="sxs-lookup"><span data-stu-id="71c0f-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="71c0f-118">userId</span><span class="sxs-lookup"><span data-stu-id="71c0f-118">userId</span></span>|<span data-ttu-id="71c0f-119">String</span><span class="sxs-lookup"><span data-stu-id="71c0f-119">String</span></span>|<span data-ttu-id="71c0f-120">Идентификатор пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="71c0f-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="71c0f-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="71c0f-121">userDisplayName</span></span>|<span data-ttu-id="71c0f-122">String</span><span class="sxs-lookup"><span data-stu-id="71c0f-122">String</span></span>|<span data-ttu-id="71c0f-123">Отображаемое имя пользователя в репозитории</span><span class="sxs-lookup"><span data-stu-id="71c0f-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="71c0f-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="71c0f-124">userPrincipalName</span></span>|<span data-ttu-id="71c0f-125">Строка</span><span class="sxs-lookup"><span data-stu-id="71c0f-125">String</span></span>|<span data-ttu-id="71c0f-126">Имя участника-пользователя в возврате.</span><span class="sxs-lookup"><span data-stu-id="71c0f-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="71c0f-127">ластчеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="71c0f-127">lastCheckinDateTime</span></span>|<span data-ttu-id="71c0f-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c0f-128">DateTimeOffset</span></span>|<span data-ttu-id="71c0f-129">Время последнего возврата для этой связи пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="71c0f-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71c0f-130">Связи</span><span class="sxs-lookup"><span data-stu-id="71c0f-130">Relationships</span></span>
<span data-ttu-id="71c0f-131">Нет</span><span class="sxs-lookup"><span data-stu-id="71c0f-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71c0f-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71c0f-132">JSON Representation</span></span>
<span data-ttu-id="71c0f-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71c0f-133">Here is a JSON representation of the resource.</span></span>
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



