---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c33a17bc2489797bfa8dc0101c128d1e29d58b47
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987827"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="d7ac3-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="d7ac3-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="d7ac3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7ac3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7ac3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7ac3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7ac3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d7ac3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7ac3-107">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="d7ac3-107">Delete user from shared apple device action result</span></span>

<span data-ttu-id="d7ac3-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d7ac3-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7ac3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7ac3-109">Properties</span></span>
|<span data-ttu-id="d7ac3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7ac3-110">Property</span></span>|<span data-ttu-id="d7ac3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d7ac3-111">Type</span></span>|<span data-ttu-id="d7ac3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d7ac3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7ac3-113">actionName</span><span class="sxs-lookup"><span data-stu-id="d7ac3-113">actionName</span></span>|<span data-ttu-id="d7ac3-114">String</span><span class="sxs-lookup"><span data-stu-id="d7ac3-114">String</span></span>|<span data-ttu-id="d7ac3-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d7ac3-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d7ac3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d7ac3-116">actionState</span></span>|[<span data-ttu-id="d7ac3-117">actionState</span><span class="sxs-lookup"><span data-stu-id="d7ac3-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d7ac3-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d7ac3-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d7ac3-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d7ac3-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d7ac3-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ac3-120">startDateTime</span></span>|<span data-ttu-id="d7ac3-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ac3-121">DateTimeOffset</span></span>|<span data-ttu-id="d7ac3-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d7ac3-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d7ac3-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7ac3-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="d7ac3-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7ac3-124">DateTimeOffset</span></span>|<span data-ttu-id="d7ac3-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d7ac3-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d7ac3-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d7ac3-126">userPrincipalName</span></span>|<span data-ttu-id="d7ac3-127">String</span><span class="sxs-lookup"><span data-stu-id="d7ac3-127">String</span></span>|<span data-ttu-id="d7ac3-128">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="d7ac3-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7ac3-129">Связи</span><span class="sxs-lookup"><span data-stu-id="d7ac3-129">Relationships</span></span>
<span data-ttu-id="d7ac3-130">Нет</span><span class="sxs-lookup"><span data-stu-id="d7ac3-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d7ac3-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7ac3-131">JSON Representation</span></span>
<span data-ttu-id="d7ac3-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7ac3-132">Here is a JSON representation of the resource.</span></span>
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





