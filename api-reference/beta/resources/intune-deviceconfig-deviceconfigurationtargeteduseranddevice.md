---
title: Тип ресурса deviceConfigurationTargetedUserAndDevice
description: Конфликт сводки для набора политик конфигурации устройства.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 234cc9c909875d835ba54709f30f1ca306eb0954
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947969"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="22a4a-103">Тип ресурса deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="22a4a-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="22a4a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22a4a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22a4a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22a4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22a4a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="22a4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22a4a-107">Конфликт сводки для набора политик конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="22a4a-107">Conflict summary for a set of device configuration policies.</span></span>
## <a name="properties"></a><span data-ttu-id="22a4a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="22a4a-108">Properties</span></span>
|<span data-ttu-id="22a4a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="22a4a-109">Property</span></span>|<span data-ttu-id="22a4a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="22a4a-110">Type</span></span>|<span data-ttu-id="22a4a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="22a4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22a4a-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="22a4a-112">deviceId</span></span>|<span data-ttu-id="22a4a-113">String</span><span class="sxs-lookup"><span data-stu-id="22a4a-113">String</span></span>|<span data-ttu-id="22a4a-114">Идентификатор устройства в возврата.</span><span class="sxs-lookup"><span data-stu-id="22a4a-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="22a4a-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="22a4a-115">deviceName</span></span>|<span data-ttu-id="22a4a-116">String</span><span class="sxs-lookup"><span data-stu-id="22a4a-116">String</span></span>|<span data-ttu-id="22a4a-117">Имя устройства в возврата.</span><span class="sxs-lookup"><span data-stu-id="22a4a-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="22a4a-118">userId</span><span class="sxs-lookup"><span data-stu-id="22a4a-118">userId</span></span>|<span data-ttu-id="22a4a-119">String</span><span class="sxs-lookup"><span data-stu-id="22a4a-119">String</span></span>|<span data-ttu-id="22a4a-120">Идентификатор пользователя в записи.</span><span class="sxs-lookup"><span data-stu-id="22a4a-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="22a4a-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="22a4a-121">userDisplayName</span></span>|<span data-ttu-id="22a4a-122">String</span><span class="sxs-lookup"><span data-stu-id="22a4a-122">String</span></span>|<span data-ttu-id="22a4a-123">Отображаемое имя пользователя в репозиторий</span><span class="sxs-lookup"><span data-stu-id="22a4a-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="22a4a-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="22a4a-124">userPrincipalName</span></span>|<span data-ttu-id="22a4a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="22a4a-125">String</span></span>|<span data-ttu-id="22a4a-126">Имя участника-пользователя в репозиторий.</span><span class="sxs-lookup"><span data-stu-id="22a4a-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="22a4a-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="22a4a-127">lastCheckinDateTime</span></span>|<span data-ttu-id="22a4a-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22a4a-128">DateTimeOffset</span></span>|<span data-ttu-id="22a4a-129">Время последнего checkin для этой пары пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="22a4a-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22a4a-130">Связи</span><span class="sxs-lookup"><span data-stu-id="22a4a-130">Relationships</span></span>
<span data-ttu-id="22a4a-131">Нет</span><span class="sxs-lookup"><span data-stu-id="22a4a-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="22a4a-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22a4a-132">JSON Representation</span></span>
<span data-ttu-id="22a4a-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22a4a-133">Here is a JSON representation of the resource.</span></span>
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





