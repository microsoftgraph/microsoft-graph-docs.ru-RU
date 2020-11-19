---
title: Тип ресурса Оффицеклиентчеккинстатус
description: Сущность, описывающая статистику по возврату клиента.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdd2d4f47244bb2eab1e7c357a9f599909166b6a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295126"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="d7b90-103">Тип ресурса Оффицеклиентчеккинстатус</span><span class="sxs-lookup"><span data-stu-id="d7b90-103">officeClientCheckinStatus resource type</span></span>

<span data-ttu-id="d7b90-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7b90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7b90-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7b90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7b90-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7b90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7b90-107">Сущность, описывающая статистику по возврату клиента.</span><span class="sxs-lookup"><span data-stu-id="d7b90-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="d7b90-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7b90-108">Properties</span></span>
|<span data-ttu-id="d7b90-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7b90-109">Property</span></span>|<span data-ttu-id="d7b90-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d7b90-110">Type</span></span>|<span data-ttu-id="d7b90-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d7b90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7b90-112">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7b90-112">userPrincipalName</span></span>|<span data-ttu-id="d7b90-113">String</span><span class="sxs-lookup"><span data-stu-id="d7b90-113">String</span></span>|<span data-ttu-id="d7b90-114">Имя участника пользователя, использующего устройство.</span><span class="sxs-lookup"><span data-stu-id="d7b90-114">User principal name using the device.</span></span>|
|<span data-ttu-id="d7b90-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="d7b90-115">deviceName</span></span>|<span data-ttu-id="d7b90-116">String</span><span class="sxs-lookup"><span data-stu-id="d7b90-116">String</span></span>|<span data-ttu-id="d7b90-117">Имя устройства, пытающееся вернуть.</span><span class="sxs-lookup"><span data-stu-id="d7b90-117">Device name trying to check-in.</span></span>|
|<span data-ttu-id="d7b90-118">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="d7b90-118">devicePlatform</span></span>|<span data-ttu-id="d7b90-119">String</span><span class="sxs-lookup"><span data-stu-id="d7b90-119">String</span></span>|<span data-ttu-id="d7b90-120">Платформа устройства пытается вернуться.</span><span class="sxs-lookup"><span data-stu-id="d7b90-120">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="d7b90-121">девицеплатформверсион</span><span class="sxs-lookup"><span data-stu-id="d7b90-121">devicePlatformVersion</span></span>|<span data-ttu-id="d7b90-122">String</span><span class="sxs-lookup"><span data-stu-id="d7b90-122">String</span></span>|<span data-ttu-id="d7b90-123">Версия платформы устройства, пытающаяся вернуть значение.</span><span class="sxs-lookup"><span data-stu-id="d7b90-123">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="d7b90-124">вассукцессфул</span><span class="sxs-lookup"><span data-stu-id="d7b90-124">wasSuccessful</span></span>|<span data-ttu-id="d7b90-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7b90-125">Boolean</span></span>|<span data-ttu-id="d7b90-126">, Если последний возврат выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="d7b90-126">If the last checkin was successful.</span></span>|
|<span data-ttu-id="d7b90-127">userId</span><span class="sxs-lookup"><span data-stu-id="d7b90-127">userId</span></span>|<span data-ttu-id="d7b90-128">String</span><span class="sxs-lookup"><span data-stu-id="d7b90-128">String</span></span>|<span data-ttu-id="d7b90-129">Идентификатор пользователя, использующий устройство.</span><span class="sxs-lookup"><span data-stu-id="d7b90-129">User identifier using the device.</span></span>|
|<span data-ttu-id="d7b90-130">чеккиндатетиме</span><span class="sxs-lookup"><span data-stu-id="d7b90-130">checkinDateTime</span></span>|<span data-ttu-id="d7b90-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7b90-131">DateTimeOffset</span></span>|<span data-ttu-id="d7b90-132">Время последнего возврата устройства в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="d7b90-132">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="d7b90-133">Ошибк</span><span class="sxs-lookup"><span data-stu-id="d7b90-133">errorMessage</span></span>|<span data-ttu-id="d7b90-134">String</span><span class="sxs-lookup"><span data-stu-id="d7b90-134">String</span></span>|<span data-ttu-id="d7b90-135">Сообщение об ошибке, если оно связано с последним возвратом.</span><span class="sxs-lookup"><span data-stu-id="d7b90-135">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="d7b90-136">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="d7b90-136">appliedPolicies</span></span>|<span data-ttu-id="d7b90-137">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="d7b90-137">String collection</span></span>|<span data-ttu-id="d7b90-138">Список политик, доставляемых на устройство при последнем возврате.</span><span class="sxs-lookup"><span data-stu-id="d7b90-138">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7b90-139">Связи</span><span class="sxs-lookup"><span data-stu-id="d7b90-139">Relationships</span></span>
<span data-ttu-id="d7b90-140">Нет</span><span class="sxs-lookup"><span data-stu-id="d7b90-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7b90-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7b90-141">JSON Representation</span></span>
<span data-ttu-id="d7b90-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7b90-142">Here is a JSON representation of the resource.</span></span>
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




