---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ed004ad8c02d18c19df7be0f819658603fb4fc0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861910"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="d6b08-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="d6b08-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="d6b08-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6b08-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6b08-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6b08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6b08-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6b08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6b08-107">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="d6b08-107">Delete user from shared apple device action result</span></span>

<span data-ttu-id="d6b08-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d6b08-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6b08-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6b08-109">Properties</span></span>
|<span data-ttu-id="d6b08-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6b08-110">Property</span></span>|<span data-ttu-id="d6b08-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d6b08-111">Type</span></span>|<span data-ttu-id="d6b08-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d6b08-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6b08-113">actionName</span><span class="sxs-lookup"><span data-stu-id="d6b08-113">actionName</span></span>|<span data-ttu-id="d6b08-114">String</span><span class="sxs-lookup"><span data-stu-id="d6b08-114">String</span></span>|<span data-ttu-id="d6b08-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d6b08-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d6b08-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d6b08-116">actionState</span></span>|[<span data-ttu-id="d6b08-117">actionState</span><span class="sxs-lookup"><span data-stu-id="d6b08-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d6b08-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d6b08-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d6b08-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d6b08-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d6b08-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d6b08-120">startDateTime</span></span>|<span data-ttu-id="d6b08-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6b08-121">DateTimeOffset</span></span>|<span data-ttu-id="d6b08-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d6b08-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d6b08-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6b08-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="d6b08-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6b08-124">DateTimeOffset</span></span>|<span data-ttu-id="d6b08-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d6b08-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d6b08-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d6b08-126">userPrincipalName</span></span>|<span data-ttu-id="d6b08-127">String</span><span class="sxs-lookup"><span data-stu-id="d6b08-127">String</span></span>|<span data-ttu-id="d6b08-128">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="d6b08-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6b08-129">Связи</span><span class="sxs-lookup"><span data-stu-id="d6b08-129">Relationships</span></span>
<span data-ttu-id="d6b08-130">Нет</span><span class="sxs-lookup"><span data-stu-id="d6b08-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6b08-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6b08-131">JSON Representation</span></span>
<span data-ttu-id="d6b08-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6b08-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





