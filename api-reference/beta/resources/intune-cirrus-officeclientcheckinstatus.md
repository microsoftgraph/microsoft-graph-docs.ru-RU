---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9b5509fed7c7dba43a9070695982c120f007f097
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42488546"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="c8e8f-103">Тип ресурса Оффицеклиентчеккинстатус</span><span class="sxs-lookup"><span data-stu-id="c8e8f-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="c8e8f-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c8e8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8e8f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8e8f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8e8f-107">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="c8e8f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8e8f-108">Properties</span></span>
|<span data-ttu-id="c8e8f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8e8f-109">Property</span></span>|<span data-ttu-id="c8e8f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c8e8f-110">Type</span></span>|<span data-ttu-id="c8e8f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c8e8f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8e8f-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c8e8f-112">userPrincipalName</span></span>|<span data-ttu-id="c8e8f-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c8e8f-113">String</span></span>|<span data-ttu-id="c8e8f-114">Имя участника пользователя, использующего устройство.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-114">User principal name using the device.</span></span>|
|<span data-ttu-id="c8e8f-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="c8e8f-115">deviceName</span></span>|<span data-ttu-id="c8e8f-116">String</span><span class="sxs-lookup"><span data-stu-id="c8e8f-116">String</span></span>|<span data-ttu-id="c8e8f-117">Имя устройства, пытающееся вернуть.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="c8e8f-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="c8e8f-118">devicePlatform</span></span>|<span data-ttu-id="c8e8f-119">String</span><span class="sxs-lookup"><span data-stu-id="c8e8f-119">String</span></span>|<span data-ttu-id="c8e8f-120">Платформа устройства пытается вернуться.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="c8e8f-121">девицеплатформверсион</span><span class="sxs-lookup"><span data-stu-id="c8e8f-121">devicePlatformVersion</span></span>|<span data-ttu-id="c8e8f-122">String</span><span class="sxs-lookup"><span data-stu-id="c8e8f-122">String</span></span>|<span data-ttu-id="c8e8f-123">Версия платформы устройства, пытающаяся вернуть значение.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="c8e8f-124">вассукцессфул</span><span class="sxs-lookup"><span data-stu-id="c8e8f-124">wasSuccessful</span></span>|<span data-ttu-id="c8e8f-125">Логический</span><span class="sxs-lookup"><span data-stu-id="c8e8f-125">Boolean</span></span>|<span data-ttu-id="c8e8f-126">, Если последний возврат выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="c8e8f-127">userId</span><span class="sxs-lookup"><span data-stu-id="c8e8f-127">userId</span></span>|<span data-ttu-id="c8e8f-128">String</span><span class="sxs-lookup"><span data-stu-id="c8e8f-128">String</span></span>|<span data-ttu-id="c8e8f-129">Идентификатор пользователя, использующий устройство.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-129">User identifier using the device.</span></span>|
|<span data-ttu-id="c8e8f-130">чеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="c8e8f-130">checkinDateTime</span></span>|<span data-ttu-id="c8e8f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8e8f-131">DateTimeOffset</span></span>|<span data-ttu-id="c8e8f-132">Время последнего возврата устройства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="c8e8f-133">Ошибк</span><span class="sxs-lookup"><span data-stu-id="c8e8f-133">errorMessage</span></span>|<span data-ttu-id="c8e8f-134">String</span><span class="sxs-lookup"><span data-stu-id="c8e8f-134">String</span></span>|<span data-ttu-id="c8e8f-135">Сообщение об ошибке, если оно связано с последним возвратом.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="c8e8f-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c8e8f-136">appliedPolicies</span></span>|<span data-ttu-id="c8e8f-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c8e8f-137">String collection</span></span>|<span data-ttu-id="c8e8f-138">Список политик, доставляемых на устройство при последнем возврате.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8e8f-139">Связи</span><span class="sxs-lookup"><span data-stu-id="c8e8f-139">Relationships</span></span>
<span data-ttu-id="c8e8f-140">Нет</span><span class="sxs-lookup"><span data-stu-id="c8e8f-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8e8f-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8e8f-141">JSON Representation</span></span>
<span data-ttu-id="c8e8f-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8e8f-142">Here is a JSON representation of the resource.</span></span>
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



