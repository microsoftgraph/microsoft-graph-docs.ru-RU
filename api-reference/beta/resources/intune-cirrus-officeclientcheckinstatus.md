---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: davidmu1
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 66087cd47fa70352f8051fc220820ea355805f19
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797341"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="24df3-103">Тип ресурса Оффицеклиентчеккинстатус</span><span class="sxs-lookup"><span data-stu-id="24df3-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="24df3-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24df3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24df3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24df3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24df3-106">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="24df3-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="24df3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="24df3-107">Properties</span></span>
|<span data-ttu-id="24df3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="24df3-108">Property</span></span>|<span data-ttu-id="24df3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="24df3-109">Type</span></span>|<span data-ttu-id="24df3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24df3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24df3-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="24df3-111">userPrincipalName</span></span>|<span data-ttu-id="24df3-112">Строка</span><span class="sxs-lookup"><span data-stu-id="24df3-112">String</span></span>|<span data-ttu-id="24df3-113">Имя участника пользователя, использующего устройство.</span><span class="sxs-lookup"><span data-stu-id="24df3-113">User principal name using the device.</span></span>|
|<span data-ttu-id="24df3-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="24df3-114">deviceName</span></span>|<span data-ttu-id="24df3-115">String</span><span class="sxs-lookup"><span data-stu-id="24df3-115">String</span></span>|<span data-ttu-id="24df3-116">Имя устройства, пытающееся вернуть.</span><span class="sxs-lookup"><span data-stu-id="24df3-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="24df3-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="24df3-117">devicePlatform</span></span>|<span data-ttu-id="24df3-118">String</span><span class="sxs-lookup"><span data-stu-id="24df3-118">String</span></span>|<span data-ttu-id="24df3-119">Платформа устройства пытается вернуться.</span><span class="sxs-lookup"><span data-stu-id="24df3-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="24df3-120">девицеплатформверсион</span><span class="sxs-lookup"><span data-stu-id="24df3-120">devicePlatformVersion</span></span>|<span data-ttu-id="24df3-121">String</span><span class="sxs-lookup"><span data-stu-id="24df3-121">String</span></span>|<span data-ttu-id="24df3-122">Версия платформы устройства, пытающаяся вернуть значение.</span><span class="sxs-lookup"><span data-stu-id="24df3-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="24df3-123">вассукцессфул</span><span class="sxs-lookup"><span data-stu-id="24df3-123">wasSuccessful</span></span>|<span data-ttu-id="24df3-124">Логический</span><span class="sxs-lookup"><span data-stu-id="24df3-124">Boolean</span></span>|<span data-ttu-id="24df3-125">, Если последний возврат выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="24df3-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="24df3-126">userId</span><span class="sxs-lookup"><span data-stu-id="24df3-126">userId</span></span>|<span data-ttu-id="24df3-127">String</span><span class="sxs-lookup"><span data-stu-id="24df3-127">String</span></span>|<span data-ttu-id="24df3-128">Идентификатор пользователя, использующий устройство.</span><span class="sxs-lookup"><span data-stu-id="24df3-128">User identifier using the device.</span></span>|
|<span data-ttu-id="24df3-129">чеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="24df3-129">checkinDateTime</span></span>|<span data-ttu-id="24df3-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24df3-130">DateTimeOffset</span></span>|<span data-ttu-id="24df3-131">Время последнего возврата устройства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="24df3-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="24df3-132">Ошибк</span><span class="sxs-lookup"><span data-stu-id="24df3-132">errorMessage</span></span>|<span data-ttu-id="24df3-133">String</span><span class="sxs-lookup"><span data-stu-id="24df3-133">String</span></span>|<span data-ttu-id="24df3-134">Сообщение об ошибке, если оно связано с последним возвратом.</span><span class="sxs-lookup"><span data-stu-id="24df3-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="24df3-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="24df3-135">appliedPolicies</span></span>|<span data-ttu-id="24df3-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="24df3-136">String collection</span></span>|<span data-ttu-id="24df3-137">Список политик, доставляемых на устройство при последнем возврате.</span><span class="sxs-lookup"><span data-stu-id="24df3-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24df3-138">Связи</span><span class="sxs-lookup"><span data-stu-id="24df3-138">Relationships</span></span>
<span data-ttu-id="24df3-139">Нет</span><span class="sxs-lookup"><span data-stu-id="24df3-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24df3-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24df3-140">JSON Representation</span></span>
<span data-ttu-id="24df3-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24df3-141">Here is a JSON representation of the resource.</span></span>
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



