---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: a7cbc54ac2e276932273130f194f484f3ee23b7c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949292"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="02538-103">Тип ресурса Оффицеклиентчеккинстатус</span><span class="sxs-lookup"><span data-stu-id="02538-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="02538-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02538-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02538-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02538-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02538-106">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="02538-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="02538-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="02538-107">Properties</span></span>
|<span data-ttu-id="02538-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="02538-108">Property</span></span>|<span data-ttu-id="02538-109">Тип</span><span class="sxs-lookup"><span data-stu-id="02538-109">Type</span></span>|<span data-ttu-id="02538-110">Описание</span><span class="sxs-lookup"><span data-stu-id="02538-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02538-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="02538-111">userPrincipalName</span></span>|<span data-ttu-id="02538-112">Строка</span><span class="sxs-lookup"><span data-stu-id="02538-112">String</span></span>|<span data-ttu-id="02538-113">Имя участника пользователя, использующего устройство.</span><span class="sxs-lookup"><span data-stu-id="02538-113">User principal name using the device.</span></span>|
|<span data-ttu-id="02538-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="02538-114">deviceName</span></span>|<span data-ttu-id="02538-115">String</span><span class="sxs-lookup"><span data-stu-id="02538-115">String</span></span>|<span data-ttu-id="02538-116">Имя устройства, пытающееся вернуть.</span><span class="sxs-lookup"><span data-stu-id="02538-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="02538-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="02538-117">devicePlatform</span></span>|<span data-ttu-id="02538-118">Строка</span><span class="sxs-lookup"><span data-stu-id="02538-118">String</span></span>|<span data-ttu-id="02538-119">Платформа устройства пытается вернуться.</span><span class="sxs-lookup"><span data-stu-id="02538-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="02538-120">Девицеплатформверсион</span><span class="sxs-lookup"><span data-stu-id="02538-120">devicePlatformVersion</span></span>|<span data-ttu-id="02538-121">Строка</span><span class="sxs-lookup"><span data-stu-id="02538-121">String</span></span>|<span data-ttu-id="02538-122">Версия платформы устройства, пытающаяся вернуть значение.</span><span class="sxs-lookup"><span data-stu-id="02538-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="02538-123">Вассукцессфул</span><span class="sxs-lookup"><span data-stu-id="02538-123">wasSuccessful</span></span>|<span data-ttu-id="02538-124">Логический</span><span class="sxs-lookup"><span data-stu-id="02538-124">Boolean</span></span>|<span data-ttu-id="02538-125">, Если последний возврат выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="02538-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="02538-126">userId</span><span class="sxs-lookup"><span data-stu-id="02538-126">userId</span></span>|<span data-ttu-id="02538-127">String</span><span class="sxs-lookup"><span data-stu-id="02538-127">String</span></span>|<span data-ttu-id="02538-128">Идентификатор пользователя, использующий устройство.</span><span class="sxs-lookup"><span data-stu-id="02538-128">User identifier using the device.</span></span>|
|<span data-ttu-id="02538-129">Чеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="02538-129">checkinDateTime</span></span>|<span data-ttu-id="02538-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02538-130">DateTimeOffset</span></span>|<span data-ttu-id="02538-131">Время последнего возврата устройства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="02538-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="02538-132">Ошибк</span><span class="sxs-lookup"><span data-stu-id="02538-132">errorMessage</span></span>|<span data-ttu-id="02538-133">Строка</span><span class="sxs-lookup"><span data-stu-id="02538-133">String</span></span>|<span data-ttu-id="02538-134">Сообщение об ошибке, если оно связано с последним возвратом.</span><span class="sxs-lookup"><span data-stu-id="02538-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="02538-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="02538-135">appliedPolicies</span></span>|<span data-ttu-id="02538-136">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="02538-136">String collection</span></span>|<span data-ttu-id="02538-137">Список политик, доставляемых на устройство при последнем возврате.</span><span class="sxs-lookup"><span data-stu-id="02538-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02538-138">Связи</span><span class="sxs-lookup"><span data-stu-id="02538-138">Relationships</span></span>
<span data-ttu-id="02538-139">Нет</span><span class="sxs-lookup"><span data-stu-id="02538-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02538-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02538-140">JSON Representation</span></span>
<span data-ttu-id="02538-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02538-141">Here is a JSON representation of the resource.</span></span>
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



