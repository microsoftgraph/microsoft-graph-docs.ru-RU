---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: dougeby
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a2f8bb8728a43187903016ca3417b8e6655b3ab
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471491"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="101ea-103">Тип ресурса Оффицеклиентчеккинстатус</span><span class="sxs-lookup"><span data-stu-id="101ea-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="101ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="101ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="101ea-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="101ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="101ea-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="101ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="101ea-107">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="101ea-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="101ea-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="101ea-108">Properties</span></span>
|<span data-ttu-id="101ea-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="101ea-109">Property</span></span>|<span data-ttu-id="101ea-110">Тип</span><span class="sxs-lookup"><span data-stu-id="101ea-110">Type</span></span>|<span data-ttu-id="101ea-111">Описание</span><span class="sxs-lookup"><span data-stu-id="101ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="101ea-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="101ea-112">userPrincipalName</span></span>|<span data-ttu-id="101ea-113">Строка</span><span class="sxs-lookup"><span data-stu-id="101ea-113">String</span></span>|<span data-ttu-id="101ea-114">Имя участника пользователя, использующего устройство.</span><span class="sxs-lookup"><span data-stu-id="101ea-114">User principal name using the device.</span></span>|
|<span data-ttu-id="101ea-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="101ea-115">deviceName</span></span>|<span data-ttu-id="101ea-116">String</span><span class="sxs-lookup"><span data-stu-id="101ea-116">String</span></span>|<span data-ttu-id="101ea-117">Имя устройства, пытающееся вернуть.</span><span class="sxs-lookup"><span data-stu-id="101ea-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="101ea-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="101ea-118">devicePlatform</span></span>|<span data-ttu-id="101ea-119">String</span><span class="sxs-lookup"><span data-stu-id="101ea-119">String</span></span>|<span data-ttu-id="101ea-120">Платформа устройства пытается вернуться.</span><span class="sxs-lookup"><span data-stu-id="101ea-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="101ea-121">девицеплатформверсион</span><span class="sxs-lookup"><span data-stu-id="101ea-121">devicePlatformVersion</span></span>|<span data-ttu-id="101ea-122">String</span><span class="sxs-lookup"><span data-stu-id="101ea-122">String</span></span>|<span data-ttu-id="101ea-123">Версия платформы устройства, пытающаяся вернуть значение.</span><span class="sxs-lookup"><span data-stu-id="101ea-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="101ea-124">вассукцессфул</span><span class="sxs-lookup"><span data-stu-id="101ea-124">wasSuccessful</span></span>|<span data-ttu-id="101ea-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="101ea-125">Boolean</span></span>|<span data-ttu-id="101ea-126">, Если последний возврат выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="101ea-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="101ea-127">userId</span><span class="sxs-lookup"><span data-stu-id="101ea-127">userId</span></span>|<span data-ttu-id="101ea-128">String</span><span class="sxs-lookup"><span data-stu-id="101ea-128">String</span></span>|<span data-ttu-id="101ea-129">Идентификатор пользователя, использующий устройство.</span><span class="sxs-lookup"><span data-stu-id="101ea-129">User identifier using the device.</span></span>|
|<span data-ttu-id="101ea-130">чеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="101ea-130">checkinDateTime</span></span>|<span data-ttu-id="101ea-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="101ea-131">DateTimeOffset</span></span>|<span data-ttu-id="101ea-132">Время последнего возврата устройства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="101ea-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="101ea-133">Ошибк</span><span class="sxs-lookup"><span data-stu-id="101ea-133">errorMessage</span></span>|<span data-ttu-id="101ea-134">String</span><span class="sxs-lookup"><span data-stu-id="101ea-134">String</span></span>|<span data-ttu-id="101ea-135">Сообщение об ошибке, если оно связано с последним возвратом.</span><span class="sxs-lookup"><span data-stu-id="101ea-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="101ea-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="101ea-136">appliedPolicies</span></span>|<span data-ttu-id="101ea-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="101ea-137">String collection</span></span>|<span data-ttu-id="101ea-138">Список политик, доставляемых на устройство при последнем возврате.</span><span class="sxs-lookup"><span data-stu-id="101ea-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="101ea-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="101ea-139">Relationships</span></span>
<span data-ttu-id="101ea-140">Нет</span><span class="sxs-lookup"><span data-stu-id="101ea-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="101ea-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="101ea-141">JSON Representation</span></span>
<span data-ttu-id="101ea-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="101ea-142">Here is a JSON representation of the resource.</span></span>
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



