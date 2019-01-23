---
title: Тип ресурса officeClientCheckinStatus
description: Сущности, которая описывает клиента возврат stats.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebc534a6c424a9dac4316d0029e2fd35839f0a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403261"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="8b289-103">Тип ресурса officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="8b289-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="8b289-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8b289-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8b289-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b289-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b289-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b289-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b289-107">Сущности, которая описывает клиента возврат stats.</span><span class="sxs-lookup"><span data-stu-id="8b289-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="8b289-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b289-108">Properties</span></span>
|<span data-ttu-id="8b289-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b289-109">Property</span></span>|<span data-ttu-id="8b289-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8b289-110">Type</span></span>|<span data-ttu-id="8b289-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8b289-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b289-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b289-112">userPrincipalName</span></span>|<span data-ttu-id="8b289-113">String</span><span class="sxs-lookup"><span data-stu-id="8b289-113">String</span></span>|<span data-ttu-id="8b289-114">Имя участника-пользователя с помощью устройства.</span><span class="sxs-lookup"><span data-stu-id="8b289-114">User principal name using the device.</span></span>|
|<span data-ttu-id="8b289-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="8b289-115">deviceName</span></span>|<span data-ttu-id="8b289-116">String</span><span class="sxs-lookup"><span data-stu-id="8b289-116">String</span></span>|<span data-ttu-id="8b289-117">Имя устройства для возврата.</span><span class="sxs-lookup"><span data-stu-id="8b289-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="8b289-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="8b289-118">devicePlatform</span></span>|<span data-ttu-id="8b289-119">String</span><span class="sxs-lookup"><span data-stu-id="8b289-119">String</span></span>|<span data-ttu-id="8b289-120">Устройство платформы для возврата.</span><span class="sxs-lookup"><span data-stu-id="8b289-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="8b289-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="8b289-121">devicePlatformVersion</span></span>|<span data-ttu-id="8b289-122">String</span><span class="sxs-lookup"><span data-stu-id="8b289-122">String</span></span>|<span data-ttu-id="8b289-123">Для возврата версии платформы устройства.</span><span class="sxs-lookup"><span data-stu-id="8b289-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="8b289-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="8b289-124">wasSuccessful</span></span>|<span data-ttu-id="8b289-125">Логический</span><span class="sxs-lookup"><span data-stu-id="8b289-125">Boolean</span></span>|<span data-ttu-id="8b289-126">Если последний checkin прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="8b289-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="8b289-127">userId</span><span class="sxs-lookup"><span data-stu-id="8b289-127">userId</span></span>|<span data-ttu-id="8b289-128">String</span><span class="sxs-lookup"><span data-stu-id="8b289-128">String</span></span>|<span data-ttu-id="8b289-129">Идентификатор пользователя, с помощью устройства.</span><span class="sxs-lookup"><span data-stu-id="8b289-129">User identifier using the device.</span></span>|
|<span data-ttu-id="8b289-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="8b289-130">checkinDateTime</span></span>|<span data-ttu-id="8b289-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b289-131">DateTimeOffset</span></span>|<span data-ttu-id="8b289-132">Последний устройства возврат времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="8b289-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="8b289-133">сообщение об ошибке</span><span class="sxs-lookup"><span data-stu-id="8b289-133">errorMessage</span></span>|<span data-ttu-id="8b289-134">String</span><span class="sxs-lookup"><span data-stu-id="8b289-134">String</span></span>|<span data-ttu-id="8b289-135">Сообщение об ошибке, если какие-либо связанные для последнего checkin.</span><span class="sxs-lookup"><span data-stu-id="8b289-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="8b289-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="8b289-136">appliedPolicies</span></span>|<span data-ttu-id="8b289-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="8b289-137">String collection</span></span>|<span data-ttu-id="8b289-138">Список политик доставки на устройство как последний checkin.</span><span class="sxs-lookup"><span data-stu-id="8b289-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b289-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="8b289-139">Relationships</span></span>
<span data-ttu-id="8b289-140">Нет</span><span class="sxs-lookup"><span data-stu-id="8b289-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b289-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b289-141">JSON Representation</span></span>
<span data-ttu-id="8b289-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b289-142">Here is a JSON representation of the resource.</span></span>
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



