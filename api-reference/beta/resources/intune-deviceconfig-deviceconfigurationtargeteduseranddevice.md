---
title: Тип ресурса deviceConfigurationTargetedUserAndDevice
description: Конфликт сводки для набора политик конфигурации устройства.
ms.openlocfilehash: 6f79a8fe24e06d2bdafa81c30cabf8158b4e5773
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075648"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="51902-103">Тип ресурса deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="51902-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="51902-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51902-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51902-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51902-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51902-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51902-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51902-107">Конфликт сводки для набора политик конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="51902-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="51902-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="51902-108">Properties</span></span>
|<span data-ttu-id="51902-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="51902-109">Property</span></span>|<span data-ttu-id="51902-110">Тип</span><span class="sxs-lookup"><span data-stu-id="51902-110">Type</span></span>|<span data-ttu-id="51902-111">Description</span><span class="sxs-lookup"><span data-stu-id="51902-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51902-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="51902-112">deviceId</span></span>|<span data-ttu-id="51902-113">String</span><span class="sxs-lookup"><span data-stu-id="51902-113">String</span></span>|<span data-ttu-id="51902-114">Идентификатор устройства в возврата.</span><span class="sxs-lookup"><span data-stu-id="51902-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="51902-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="51902-115">deviceName</span></span>|<span data-ttu-id="51902-116">String</span><span class="sxs-lookup"><span data-stu-id="51902-116">String</span></span>|<span data-ttu-id="51902-117">Имя устройства в возврата.</span><span class="sxs-lookup"><span data-stu-id="51902-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="51902-118">userId</span><span class="sxs-lookup"><span data-stu-id="51902-118">userId</span></span>|<span data-ttu-id="51902-119">String</span><span class="sxs-lookup"><span data-stu-id="51902-119">String</span></span>|<span data-ttu-id="51902-120">Идентификатор пользователя в записи.</span><span class="sxs-lookup"><span data-stu-id="51902-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="51902-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="51902-121">userDisplayName</span></span>|<span data-ttu-id="51902-122">String</span><span class="sxs-lookup"><span data-stu-id="51902-122">String</span></span>|<span data-ttu-id="51902-123">Отображаемое имя пользователя в репозиторий</span><span class="sxs-lookup"><span data-stu-id="51902-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="51902-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51902-124">userPrincipalName</span></span>|<span data-ttu-id="51902-125">String</span><span class="sxs-lookup"><span data-stu-id="51902-125">String</span></span>|<span data-ttu-id="51902-126">Имя участника-пользователя в репозиторий.</span><span class="sxs-lookup"><span data-stu-id="51902-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="51902-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="51902-127">lastCheckinDateTime</span></span>|<span data-ttu-id="51902-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51902-128">DateTimeOffset</span></span>|<span data-ttu-id="51902-129">Время последнего checkin для этой пары пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="51902-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51902-130">Связи</span><span class="sxs-lookup"><span data-stu-id="51902-130">Relationships</span></span>
<span data-ttu-id="51902-131">Нет</span><span class="sxs-lookup"><span data-stu-id="51902-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51902-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51902-132">JSON Representation</span></span>
<span data-ttu-id="51902-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51902-133">Here is a JSON representation of the resource.</span></span>
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





