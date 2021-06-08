---
title: тип ресурса officeClientCheckinStatus
description: Объект, описывая статистику регистрации клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdd2d4f47244bb2eab1e7c357a9f599909166b6a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758622"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="36c26-103">тип ресурса officeClientCheckinStatus</span><span class="sxs-lookup"><span data-stu-id="36c26-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="36c26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36c26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36c26-105">**Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36c26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36c26-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="36c26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36c26-107">Объект, описывая статистику регистрации клиента.</span><span class="sxs-lookup"><span data-stu-id="36c26-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="36c26-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="36c26-108">Properties</span></span>
|<span data-ttu-id="36c26-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="36c26-109">Property</span></span>|<span data-ttu-id="36c26-110">Тип</span><span class="sxs-lookup"><span data-stu-id="36c26-110">Type</span></span>|<span data-ttu-id="36c26-111">Описание</span><span class="sxs-lookup"><span data-stu-id="36c26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="36c26-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="36c26-112">userPrincipalName</span></span>|<span data-ttu-id="36c26-113">String</span><span class="sxs-lookup"><span data-stu-id="36c26-113">String</span></span>|<span data-ttu-id="36c26-114">Имя основного пользователя с помощью устройства.</span><span class="sxs-lookup"><span data-stu-id="36c26-114">User principal name using the device.</span></span>|
|<span data-ttu-id="36c26-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="36c26-115">deviceName</span></span>|<span data-ttu-id="36c26-116">String</span><span class="sxs-lookup"><span data-stu-id="36c26-116">String</span></span>|<span data-ttu-id="36c26-117">Имя устройства при попытке регистрации.</span><span class="sxs-lookup"><span data-stu-id="36c26-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="36c26-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="36c26-118">devicePlatform</span></span>|<span data-ttu-id="36c26-119">String</span><span class="sxs-lookup"><span data-stu-id="36c26-119">String</span></span>|<span data-ttu-id="36c26-120">Платформа устройства, пытаемаяся проверить регистрацию.</span><span class="sxs-lookup"><span data-stu-id="36c26-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="36c26-121">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="36c26-121">devicePlatformVersion</span></span>|<span data-ttu-id="36c26-122">String</span><span class="sxs-lookup"><span data-stu-id="36c26-122">String</span></span>|<span data-ttu-id="36c26-123">Версия платформы устройства при попытке регистрации.</span><span class="sxs-lookup"><span data-stu-id="36c26-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="36c26-124">wasSuccessful</span><span class="sxs-lookup"><span data-stu-id="36c26-124">wasSuccessful</span></span>|<span data-ttu-id="36c26-125">Логический</span><span class="sxs-lookup"><span data-stu-id="36c26-125">Boolean</span></span>|<span data-ttu-id="36c26-126">Если последняя проверка прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="36c26-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="36c26-127">userId</span><span class="sxs-lookup"><span data-stu-id="36c26-127">userId</span></span>|<span data-ttu-id="36c26-128">String</span><span class="sxs-lookup"><span data-stu-id="36c26-128">String</span></span>|<span data-ttu-id="36c26-129">Идентификатор пользователя с помощью устройства.</span><span class="sxs-lookup"><span data-stu-id="36c26-129">User identifier using the device.</span></span>|
|<span data-ttu-id="36c26-130">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="36c26-130">checkinDateTime</span></span>|<span data-ttu-id="36c26-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="36c26-131">DateTimeOffset</span></span>|<span data-ttu-id="36c26-132">Последнее время регистрации устройства в UTC.</span><span class="sxs-lookup"><span data-stu-id="36c26-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="36c26-133">errorMessage</span><span class="sxs-lookup"><span data-stu-id="36c26-133">errorMessage</span></span>|<span data-ttu-id="36c26-134">String</span><span class="sxs-lookup"><span data-stu-id="36c26-134">String</span></span>|<span data-ttu-id="36c26-135">Сообщение об ошибке, связанное с последней проверкой.</span><span class="sxs-lookup"><span data-stu-id="36c26-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="36c26-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="36c26-136">appliedPolicies</span></span>|<span data-ttu-id="36c26-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="36c26-137">String collection</span></span>|<span data-ttu-id="36c26-138">Список политик, доставленных на устройство в качестве последней проверки.</span><span class="sxs-lookup"><span data-stu-id="36c26-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="36c26-139">Связи</span><span class="sxs-lookup"><span data-stu-id="36c26-139">Relationships</span></span>
<span data-ttu-id="36c26-140">Нет</span><span class="sxs-lookup"><span data-stu-id="36c26-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="36c26-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36c26-141">JSON Representation</span></span>
<span data-ttu-id="36c26-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36c26-142">Here is a JSON representation of the resource.</span></span>
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




