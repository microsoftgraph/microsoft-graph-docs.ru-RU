---
title: Тип ресурса deviceConfigurationTargetedUserAndDevice
description: Конфликт сводки для набора политик конфигурации устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e246d9731f5ed9d2ea888ba2b53d335fcbca19f1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410744"
---
# <a name="deviceconfigurationtargeteduseranddevice-resource-type"></a><span data-ttu-id="288f0-103">Тип ресурса deviceConfigurationTargetedUserAndDevice</span><span class="sxs-lookup"><span data-stu-id="288f0-103">deviceConfigurationTargetedUserAndDevice resource type</span></span>

> <span data-ttu-id="288f0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="288f0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="288f0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="288f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="288f0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="288f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="288f0-107">Конфликт сводки для набора политик конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="288f0-107">Conflict summary for a set of device configuration policies.</span></span>

## <a name="properties"></a><span data-ttu-id="288f0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="288f0-108">Properties</span></span>
|<span data-ttu-id="288f0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="288f0-109">Property</span></span>|<span data-ttu-id="288f0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="288f0-110">Type</span></span>|<span data-ttu-id="288f0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="288f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="288f0-112">deviceId</span><span class="sxs-lookup"><span data-stu-id="288f0-112">deviceId</span></span>|<span data-ttu-id="288f0-113">String</span><span class="sxs-lookup"><span data-stu-id="288f0-113">String</span></span>|<span data-ttu-id="288f0-114">Идентификатор устройства в возврата.</span><span class="sxs-lookup"><span data-stu-id="288f0-114">The id of the device in the checkin.</span></span>|
|<span data-ttu-id="288f0-115">deviceName</span><span class="sxs-lookup"><span data-stu-id="288f0-115">deviceName</span></span>|<span data-ttu-id="288f0-116">String</span><span class="sxs-lookup"><span data-stu-id="288f0-116">String</span></span>|<span data-ttu-id="288f0-117">Имя устройства в возврата.</span><span class="sxs-lookup"><span data-stu-id="288f0-117">The name of the device in the checkin.</span></span>|
|<span data-ttu-id="288f0-118">userId</span><span class="sxs-lookup"><span data-stu-id="288f0-118">userId</span></span>|<span data-ttu-id="288f0-119">String</span><span class="sxs-lookup"><span data-stu-id="288f0-119">String</span></span>|<span data-ttu-id="288f0-120">Идентификатор пользователя в записи.</span><span class="sxs-lookup"><span data-stu-id="288f0-120">The id of the user in the checkin.</span></span>|
|<span data-ttu-id="288f0-121">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="288f0-121">userDisplayName</span></span>|<span data-ttu-id="288f0-122">String</span><span class="sxs-lookup"><span data-stu-id="288f0-122">String</span></span>|<span data-ttu-id="288f0-123">Отображаемое имя пользователя в репозиторий</span><span class="sxs-lookup"><span data-stu-id="288f0-123">The display name of the user in the checkin</span></span>|
|<span data-ttu-id="288f0-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="288f0-124">userPrincipalName</span></span>|<span data-ttu-id="288f0-125">String</span><span class="sxs-lookup"><span data-stu-id="288f0-125">String</span></span>|<span data-ttu-id="288f0-126">Имя участника-пользователя в репозиторий.</span><span class="sxs-lookup"><span data-stu-id="288f0-126">The UPN of the user in the checkin.</span></span>|
|<span data-ttu-id="288f0-127">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="288f0-127">lastCheckinDateTime</span></span>|<span data-ttu-id="288f0-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="288f0-128">DateTimeOffset</span></span>|<span data-ttu-id="288f0-129">Время последнего checkin для этой пары пользователя и устройства.</span><span class="sxs-lookup"><span data-stu-id="288f0-129">Last checkin time for this user/device pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="288f0-130">Отношения</span><span class="sxs-lookup"><span data-stu-id="288f0-130">Relationships</span></span>
<span data-ttu-id="288f0-131">Нет</span><span class="sxs-lookup"><span data-stu-id="288f0-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="288f0-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="288f0-132">JSON Representation</span></span>
<span data-ttu-id="288f0-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="288f0-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationTargetedUserAndDevice",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "lastCheckinDateTime": "String (timestamp)"
}
```




