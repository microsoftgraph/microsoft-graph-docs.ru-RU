---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4bd7815b396f6a8ad79e9369eed72bbb9be23cfb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459709"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="83bec-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="83bec-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="83bec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83bec-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83bec-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="83bec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83bec-106">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="83bec-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="83bec-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="83bec-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="83bec-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="83bec-108">Properties</span></span>
|<span data-ttu-id="83bec-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="83bec-109">Property</span></span>|<span data-ttu-id="83bec-110">Тип</span><span class="sxs-lookup"><span data-stu-id="83bec-110">Type</span></span>|<span data-ttu-id="83bec-111">Описание</span><span class="sxs-lookup"><span data-stu-id="83bec-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83bec-112">actionName</span><span class="sxs-lookup"><span data-stu-id="83bec-112">actionName</span></span>|<span data-ttu-id="83bec-113">String</span><span class="sxs-lookup"><span data-stu-id="83bec-113">String</span></span>|<span data-ttu-id="83bec-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="83bec-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="83bec-115">actionState</span><span class="sxs-lookup"><span data-stu-id="83bec-115">actionState</span></span>|[<span data-ttu-id="83bec-116">actionState</span><span class="sxs-lookup"><span data-stu-id="83bec-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="83bec-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="83bec-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="83bec-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="83bec-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="83bec-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="83bec-119">startDateTime</span></span>|<span data-ttu-id="83bec-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83bec-120">DateTimeOffset</span></span>|<span data-ttu-id="83bec-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="83bec-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="83bec-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="83bec-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="83bec-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83bec-123">DateTimeOffset</span></span>|<span data-ttu-id="83bec-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="83bec-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="83bec-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="83bec-125">userPrincipalName</span></span>|<span data-ttu-id="83bec-126">String</span><span class="sxs-lookup"><span data-stu-id="83bec-126">String</span></span>|<span data-ttu-id="83bec-127">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="83bec-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="83bec-128">Связи</span><span class="sxs-lookup"><span data-stu-id="83bec-128">Relationships</span></span>
<span data-ttu-id="83bec-129">Нет</span><span class="sxs-lookup"><span data-stu-id="83bec-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83bec-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="83bec-130">JSON Representation</span></span>
<span data-ttu-id="83bec-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83bec-131">Here is a JSON representation of the resource.</span></span>
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







