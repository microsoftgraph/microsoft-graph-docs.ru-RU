---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 465b07ba286b9ee3a58132424be2a25b1c7e564e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156058"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="bfa4d-103">Тип ресурса Оффицеклиентчеккинстатус</span><span class="sxs-lookup"><span data-stu-id="bfa4d-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="bfa4d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfa4d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfa4d-106">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="bfa4d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfa4d-107">Properties</span></span>
|<span data-ttu-id="bfa4d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfa4d-108">Property</span></span>|<span data-ttu-id="bfa4d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bfa4d-109">Type</span></span>|<span data-ttu-id="bfa4d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bfa4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfa4d-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bfa4d-111">userPrincipalName</span></span>|<span data-ttu-id="bfa4d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="bfa4d-112">String</span></span>|<span data-ttu-id="bfa4d-113">Имя участника пользователя, использующего устройство.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-113">User principal name using the device.</span></span>|
|<span data-ttu-id="bfa4d-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="bfa4d-114">deviceName</span></span>|<span data-ttu-id="bfa4d-115">String</span><span class="sxs-lookup"><span data-stu-id="bfa4d-115">String</span></span>|<span data-ttu-id="bfa4d-116">Имя устройства, пытающееся вернуть.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="bfa4d-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="bfa4d-117">devicePlatform</span></span>|<span data-ttu-id="bfa4d-118">String</span><span class="sxs-lookup"><span data-stu-id="bfa4d-118">String</span></span>|<span data-ttu-id="bfa4d-119">Платформа устройства пытается вернуться.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="bfa4d-120">Девицеплатформверсион</span><span class="sxs-lookup"><span data-stu-id="bfa4d-120">devicePlatformVersion</span></span>|<span data-ttu-id="bfa4d-121">String</span><span class="sxs-lookup"><span data-stu-id="bfa4d-121">String</span></span>|<span data-ttu-id="bfa4d-122">Версия платформы устройства, пытающаяся вернуть значение.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="bfa4d-123">Вассукцессфул</span><span class="sxs-lookup"><span data-stu-id="bfa4d-123">wasSuccessful</span></span>|<span data-ttu-id="bfa4d-124">Логический</span><span class="sxs-lookup"><span data-stu-id="bfa4d-124">Boolean</span></span>|<span data-ttu-id="bfa4d-125">, Если последний возврат выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="bfa4d-126">userId</span><span class="sxs-lookup"><span data-stu-id="bfa4d-126">userId</span></span>|<span data-ttu-id="bfa4d-127">String</span><span class="sxs-lookup"><span data-stu-id="bfa4d-127">String</span></span>|<span data-ttu-id="bfa4d-128">Идентификатор пользователя, использующий устройство.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-128">User identifier using the device.</span></span>|
|<span data-ttu-id="bfa4d-129">Чеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="bfa4d-129">checkinDateTime</span></span>|<span data-ttu-id="bfa4d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bfa4d-130">DateTimeOffset</span></span>|<span data-ttu-id="bfa4d-131">Время последнего возврата устройства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="bfa4d-132">Ошибк</span><span class="sxs-lookup"><span data-stu-id="bfa4d-132">errorMessage</span></span>|<span data-ttu-id="bfa4d-133">String</span><span class="sxs-lookup"><span data-stu-id="bfa4d-133">String</span></span>|<span data-ttu-id="bfa4d-134">Сообщение об ошибке, если оно связано с последним возвратом.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="bfa4d-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="bfa4d-135">appliedPolicies</span></span>|<span data-ttu-id="bfa4d-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bfa4d-136">String collection</span></span>|<span data-ttu-id="bfa4d-137">Список политик, доставляемых на устройство при последнем возврате.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfa4d-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="bfa4d-138">Relationships</span></span>
<span data-ttu-id="bfa4d-139">Нет</span><span class="sxs-lookup"><span data-stu-id="bfa4d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bfa4d-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfa4d-140">JSON Representation</span></span>
<span data-ttu-id="bfa4d-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bfa4d-141">Here is a JSON representation of the resource.</span></span>
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



