---
title: Тип ресурса officeClientCheckinStatus
description: Сущности, которая описывает клиента возврат stats.
ms.openlocfilehash: a87a085d42ce0754e046b319b270ddf90a3bdba7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077425"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="c3e80-103">Тип ресурса officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="c3e80-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="c3e80-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c3e80-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3e80-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e80-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3e80-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c3e80-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3e80-107">Сущности, которая описывает клиента возврат stats.</span><span class="sxs-lookup"><span data-stu-id="c3e80-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="c3e80-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3e80-108">Properties</span></span>
|<span data-ttu-id="c3e80-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3e80-109">Property</span></span>|<span data-ttu-id="c3e80-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c3e80-110">Type</span></span>|<span data-ttu-id="c3e80-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c3e80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3e80-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c3e80-112">userPrincipalName</span></span>|<span data-ttu-id="c3e80-113">String</span><span class="sxs-lookup"><span data-stu-id="c3e80-113">String</span></span>|<span data-ttu-id="c3e80-114">Имя участника-пользователя с помощью устройства.</span><span class="sxs-lookup"><span data-stu-id="c3e80-114">User principal name using the device.</span></span>|
|<span data-ttu-id="c3e80-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="c3e80-115">deviceName</span></span>|<span data-ttu-id="c3e80-116">String</span><span class="sxs-lookup"><span data-stu-id="c3e80-116">String</span></span>|<span data-ttu-id="c3e80-117">Имя устройства для возврата.</span><span class="sxs-lookup"><span data-stu-id="c3e80-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="c3e80-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="c3e80-118">devicePlatform</span></span>|<span data-ttu-id="c3e80-119">String</span><span class="sxs-lookup"><span data-stu-id="c3e80-119">String</span></span>|<span data-ttu-id="c3e80-120">Устройство платформы для возврата.</span><span class="sxs-lookup"><span data-stu-id="c3e80-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="c3e80-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="c3e80-121">devicePlatformVersion</span></span>|<span data-ttu-id="c3e80-122">String</span><span class="sxs-lookup"><span data-stu-id="c3e80-122">String</span></span>|<span data-ttu-id="c3e80-123">Для возврата версии платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="c3e80-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="c3e80-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="c3e80-124">wasSuccessful</span></span>|<span data-ttu-id="c3e80-125">Логический</span><span class="sxs-lookup"><span data-stu-id="c3e80-125">Boolean</span></span>|<span data-ttu-id="c3e80-126">Если последний checkin прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="c3e80-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="c3e80-127">userId</span><span class="sxs-lookup"><span data-stu-id="c3e80-127">userId</span></span>|<span data-ttu-id="c3e80-128">String</span><span class="sxs-lookup"><span data-stu-id="c3e80-128">String</span></span>|<span data-ttu-id="c3e80-129">Идентификатор пользователя, с помощью устройства.</span><span class="sxs-lookup"><span data-stu-id="c3e80-129">User identifier using the device.</span></span>|
|<span data-ttu-id="c3e80-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="c3e80-130">checkinDateTime</span></span>|<span data-ttu-id="c3e80-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3e80-131">DateTimeOffset</span></span>|<span data-ttu-id="c3e80-132">Последний устройства возврат времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c3e80-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="c3e80-133">сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="c3e80-133">errorMessage</span></span>|<span data-ttu-id="c3e80-134">String</span><span class="sxs-lookup"><span data-stu-id="c3e80-134">String</span></span>|<span data-ttu-id="c3e80-135">Сообщение об ошибке, если какие-либо связанные для последнего checkin.</span><span class="sxs-lookup"><span data-stu-id="c3e80-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="c3e80-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c3e80-136">appliedPolicies</span></span>|<span data-ttu-id="c3e80-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c3e80-137">String collection</span></span>|<span data-ttu-id="c3e80-138">Список политик доставки на устройство как последний checkin.</span><span class="sxs-lookup"><span data-stu-id="c3e80-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3e80-139">Связи</span><span class="sxs-lookup"><span data-stu-id="c3e80-139">Relationships</span></span>
<span data-ttu-id="c3e80-140">Нет</span><span class="sxs-lookup"><span data-stu-id="c3e80-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c3e80-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c3e80-141">JSON Representation</span></span>
<span data-ttu-id="c3e80-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3e80-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



