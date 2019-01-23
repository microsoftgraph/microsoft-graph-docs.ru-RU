---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c65a1c60a77ba196448dd626b345c69c71f16de6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399278"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="94dd5-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="94dd5-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="94dd5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="94dd5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="94dd5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94dd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94dd5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="94dd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94dd5-107">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="94dd5-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="94dd5-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="94dd5-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="94dd5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="94dd5-109">Properties</span></span>
|<span data-ttu-id="94dd5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="94dd5-110">Property</span></span>|<span data-ttu-id="94dd5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="94dd5-111">Type</span></span>|<span data-ttu-id="94dd5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="94dd5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94dd5-113">actionName</span><span class="sxs-lookup"><span data-stu-id="94dd5-113">actionName</span></span>|<span data-ttu-id="94dd5-114">String</span><span class="sxs-lookup"><span data-stu-id="94dd5-114">String</span></span>|<span data-ttu-id="94dd5-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="94dd5-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="94dd5-116">actionState</span><span class="sxs-lookup"><span data-stu-id="94dd5-116">actionState</span></span>|[<span data-ttu-id="94dd5-117">actionState</span><span class="sxs-lookup"><span data-stu-id="94dd5-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="94dd5-118">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="94dd5-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="94dd5-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="94dd5-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="94dd5-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="94dd5-120">startDateTime</span></span>|<span data-ttu-id="94dd5-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94dd5-121">DateTimeOffset</span></span>|<span data-ttu-id="94dd5-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="94dd5-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="94dd5-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="94dd5-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="94dd5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94dd5-124">DateTimeOffset</span></span>|<span data-ttu-id="94dd5-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="94dd5-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="94dd5-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="94dd5-126">userPrincipalName</span></span>|<span data-ttu-id="94dd5-127">String</span><span class="sxs-lookup"><span data-stu-id="94dd5-127">String</span></span>|<span data-ttu-id="94dd5-128">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="94dd5-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="94dd5-129">Связи</span><span class="sxs-lookup"><span data-stu-id="94dd5-129">Relationships</span></span>
<span data-ttu-id="94dd5-130">Нет</span><span class="sxs-lookup"><span data-stu-id="94dd5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94dd5-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94dd5-131">JSON Representation</span></span>
<span data-ttu-id="94dd5-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94dd5-132">Here is a JSON representation of the resource.</span></span>
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




