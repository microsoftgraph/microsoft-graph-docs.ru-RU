---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df8f1927329a34a51b5f6d8738faec05be01b451
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012004"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="6d652-103">Тип ресурса Оффицеклиентчеккинстатус</span><span class="sxs-lookup"><span data-stu-id="6d652-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="6d652-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d652-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d652-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d652-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d652-106">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="6d652-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="6d652-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d652-107">Properties</span></span>
|<span data-ttu-id="6d652-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d652-108">Property</span></span>|<span data-ttu-id="6d652-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6d652-109">Type</span></span>|<span data-ttu-id="6d652-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6d652-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d652-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="6d652-111">userPrincipalName</span></span>|<span data-ttu-id="6d652-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6d652-112">String</span></span>|<span data-ttu-id="6d652-113">Имя участника пользователя, использующего устройство.</span><span class="sxs-lookup"><span data-stu-id="6d652-113">User principal name using the device.</span></span>|
|<span data-ttu-id="6d652-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="6d652-114">deviceName</span></span>|<span data-ttu-id="6d652-115">String</span><span class="sxs-lookup"><span data-stu-id="6d652-115">String</span></span>|<span data-ttu-id="6d652-116">Имя устройства, пытающееся вернуть.</span><span class="sxs-lookup"><span data-stu-id="6d652-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="6d652-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="6d652-117">devicePlatform</span></span>|<span data-ttu-id="6d652-118">String</span><span class="sxs-lookup"><span data-stu-id="6d652-118">String</span></span>|<span data-ttu-id="6d652-119">Платформа устройства пытается вернуться.</span><span class="sxs-lookup"><span data-stu-id="6d652-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="6d652-120">Девицеплатформверсион</span><span class="sxs-lookup"><span data-stu-id="6d652-120">devicePlatformVersion</span></span>|<span data-ttu-id="6d652-121">String</span><span class="sxs-lookup"><span data-stu-id="6d652-121">String</span></span>|<span data-ttu-id="6d652-122">Версия платформы устройства, пытающаяся вернуть значение.</span><span class="sxs-lookup"><span data-stu-id="6d652-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="6d652-123">Вассукцессфул</span><span class="sxs-lookup"><span data-stu-id="6d652-123">wasSuccessful</span></span>|<span data-ttu-id="6d652-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d652-124">Boolean</span></span>|<span data-ttu-id="6d652-125">, Если последний возврат выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="6d652-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="6d652-126">userId</span><span class="sxs-lookup"><span data-stu-id="6d652-126">userId</span></span>|<span data-ttu-id="6d652-127">String</span><span class="sxs-lookup"><span data-stu-id="6d652-127">String</span></span>|<span data-ttu-id="6d652-128">Идентификатор пользователя, использующий устройство.</span><span class="sxs-lookup"><span data-stu-id="6d652-128">User identifier using the device.</span></span>|
|<span data-ttu-id="6d652-129">Чеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="6d652-129">checkinDateTime</span></span>|<span data-ttu-id="6d652-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d652-130">DateTimeOffset</span></span>|<span data-ttu-id="6d652-131">Время последнего возврата устройства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="6d652-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="6d652-132">Ошибк</span><span class="sxs-lookup"><span data-stu-id="6d652-132">errorMessage</span></span>|<span data-ttu-id="6d652-133">String</span><span class="sxs-lookup"><span data-stu-id="6d652-133">String</span></span>|<span data-ttu-id="6d652-134">Сообщение об ошибке, если оно связано с последним возвратом.</span><span class="sxs-lookup"><span data-stu-id="6d652-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="6d652-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="6d652-135">appliedPolicies</span></span>|<span data-ttu-id="6d652-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="6d652-136">String collection</span></span>|<span data-ttu-id="6d652-137">Список политик, доставляемых на устройство при последнем возврате.</span><span class="sxs-lookup"><span data-stu-id="6d652-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d652-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="6d652-138">Relationships</span></span>
<span data-ttu-id="6d652-139">Нет</span><span class="sxs-lookup"><span data-stu-id="6d652-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d652-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d652-140">JSON Representation</span></span>
<span data-ttu-id="6d652-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d652-141">Here is a JSON representation of the resource.</span></span>
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



