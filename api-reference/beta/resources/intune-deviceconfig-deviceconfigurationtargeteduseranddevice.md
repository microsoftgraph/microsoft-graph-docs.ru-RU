---
title: Тип ресурса deviceConfigurationTargetedUserAndDevice
description: Конфликт сводки для набора политик конфигурации устройства.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 46355f78f23060ecc901c3f98f0e3f7d13101d1e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809627"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="89df9-103">Тип ресурса deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="89df9-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="89df9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="89df9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89df9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89df9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89df9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="89df9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89df9-107">Конфликт сводки для набора политик конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="89df9-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="89df9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="89df9-108">Properties</span></span>
|<span data-ttu-id="89df9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="89df9-109">Property</span></span>|<span data-ttu-id="89df9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="89df9-110">Type</span></span>|<span data-ttu-id="89df9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="89df9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89df9-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="89df9-112">deviceId</span></span>|<span data-ttu-id="89df9-113">String</span><span class="sxs-lookup"><span data-stu-id="89df9-113">String</span></span>|<span data-ttu-id="89df9-114">Идентификатор устройства в возврата.</span><span class="sxs-lookup"><span data-stu-id="89df9-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="89df9-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="89df9-115">deviceName</span></span>|<span data-ttu-id="89df9-116">String</span><span class="sxs-lookup"><span data-stu-id="89df9-116">String</span></span>|<span data-ttu-id="89df9-117">Имя устройства в возврата.</span><span class="sxs-lookup"><span data-stu-id="89df9-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="89df9-118">userId</span><span class="sxs-lookup"><span data-stu-id="89df9-118">userId</span></span>|<span data-ttu-id="89df9-119">String</span><span class="sxs-lookup"><span data-stu-id="89df9-119">String</span></span>|<span data-ttu-id="89df9-120">Идентификатор пользователя в записи.</span><span class="sxs-lookup"><span data-stu-id="89df9-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="89df9-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="89df9-121">userDisplayName</span></span>|<span data-ttu-id="89df9-122">String</span><span class="sxs-lookup"><span data-stu-id="89df9-122">String</span></span>|<span data-ttu-id="89df9-123">Отображаемое имя пользователя в репозиторий</span><span class="sxs-lookup"><span data-stu-id="89df9-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="89df9-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="89df9-124">userPrincipalName</span></span>|<span data-ttu-id="89df9-125">Строка</span><span class="sxs-lookup"><span data-stu-id="89df9-125">String</span></span>|<span data-ttu-id="89df9-126">Имя участника-пользователя в репозиторий.</span><span class="sxs-lookup"><span data-stu-id="89df9-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="89df9-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="89df9-127">lastCheckinDateTime</span></span>|<span data-ttu-id="89df9-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89df9-128">DateTimeOffset</span></span>|<span data-ttu-id="89df9-129">Время последнего checkin для этой пары пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="89df9-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89df9-130">Связи</span><span class="sxs-lookup"><span data-stu-id="89df9-130">Relationships</span></span>
<span data-ttu-id="89df9-131">Нет</span><span class="sxs-lookup"><span data-stu-id="89df9-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="89df9-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89df9-132">JSON Representation</span></span>
<span data-ttu-id="89df9-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89df9-133">Here is a JSON representation of the resource.</span></span>
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





