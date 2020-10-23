---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 014246b973e9ea94ef79eba45c771110dca6da76
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694013"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="a6570-103">Тип ресурса Оффицеклиентчеккинстатус</span><span class="sxs-lookup"><span data-stu-id="a6570-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="a6570-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6570-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6570-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6570-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6570-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6570-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6570-107">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="a6570-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="a6570-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6570-108">Properties</span></span>
|<span data-ttu-id="a6570-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6570-109">Property</span></span>|<span data-ttu-id="a6570-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a6570-110">Type</span></span>|<span data-ttu-id="a6570-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a6570-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6570-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a6570-112">userPrincipalName</span></span>|<span data-ttu-id="a6570-113">String</span><span class="sxs-lookup"><span data-stu-id="a6570-113">String</span></span>|<span data-ttu-id="a6570-114">Имя участника пользователя, использующего устройство.</span><span class="sxs-lookup"><span data-stu-id="a6570-114">User principal name using the device.</span></span>|
|<span data-ttu-id="a6570-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="a6570-115">deviceName</span></span>|<span data-ttu-id="a6570-116">String</span><span class="sxs-lookup"><span data-stu-id="a6570-116">String</span></span>|<span data-ttu-id="a6570-117">Имя устройства, пытающееся вернуть.</span><span class="sxs-lookup"><span data-stu-id="a6570-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="a6570-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="a6570-118">devicePlatform</span></span>|<span data-ttu-id="a6570-119">Строка</span><span class="sxs-lookup"><span data-stu-id="a6570-119">String</span></span>|<span data-ttu-id="a6570-120">Платформа устройства пытается вернуться.</span><span class="sxs-lookup"><span data-stu-id="a6570-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="a6570-121">девицеплатформверсион</span><span class="sxs-lookup"><span data-stu-id="a6570-121">devicePlatformVersion</span></span>|<span data-ttu-id="a6570-122">Строка</span><span class="sxs-lookup"><span data-stu-id="a6570-122">String</span></span>|<span data-ttu-id="a6570-123">Версия платформы устройства, пытающаяся вернуть значение.</span><span class="sxs-lookup"><span data-stu-id="a6570-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="a6570-124">вассукцессфул</span><span class="sxs-lookup"><span data-stu-id="a6570-124">wasSuccessful</span></span>|<span data-ttu-id="a6570-125">Логический</span><span class="sxs-lookup"><span data-stu-id="a6570-125">Boolean</span></span>|<span data-ttu-id="a6570-126">, Если последний возврат выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="a6570-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="a6570-127">userId</span><span class="sxs-lookup"><span data-stu-id="a6570-127">userId</span></span>|<span data-ttu-id="a6570-128">String</span><span class="sxs-lookup"><span data-stu-id="a6570-128">String</span></span>|<span data-ttu-id="a6570-129">Идентификатор пользователя, использующий устройство.</span><span class="sxs-lookup"><span data-stu-id="a6570-129">User identifier using the device.</span></span>|
|<span data-ttu-id="a6570-130">чеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="a6570-130">checkinDateTime</span></span>|<span data-ttu-id="a6570-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6570-131">DateTimeOffset</span></span>|<span data-ttu-id="a6570-132">Время последнего возврата устройства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="a6570-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="a6570-133">Ошибк</span><span class="sxs-lookup"><span data-stu-id="a6570-133">errorMessage</span></span>|<span data-ttu-id="a6570-134">Строка</span><span class="sxs-lookup"><span data-stu-id="a6570-134">String</span></span>|<span data-ttu-id="a6570-135">Сообщение об ошибке, если оно связано с последним возвратом.</span><span class="sxs-lookup"><span data-stu-id="a6570-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="a6570-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="a6570-136">appliedPolicies</span></span>|<span data-ttu-id="a6570-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a6570-137">String collection</span></span>|<span data-ttu-id="a6570-138">Список политик, доставляемых на устройство при последнем возврате.</span><span class="sxs-lookup"><span data-stu-id="a6570-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6570-139">Связи</span><span class="sxs-lookup"><span data-stu-id="a6570-139">Relationships</span></span>
<span data-ttu-id="a6570-140">Нет</span><span class="sxs-lookup"><span data-stu-id="a6570-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6570-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6570-141">JSON Representation</span></span>
<span data-ttu-id="a6570-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6570-142">Here is a JSON representation of the resource.</span></span>
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





