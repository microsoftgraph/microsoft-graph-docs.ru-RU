---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e956edd96d752b50f189b951ac686deb78ba026d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968542"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="9f7ed-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="9f7ed-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="9f7ed-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9f7ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9f7ed-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9f7ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f7ed-106">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="9f7ed-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="9f7ed-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9f7ed-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9f7ed-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9f7ed-108">Properties</span></span>
|<span data-ttu-id="9f7ed-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f7ed-109">Property</span></span>|<span data-ttu-id="9f7ed-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9f7ed-110">Type</span></span>|<span data-ttu-id="9f7ed-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9f7ed-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f7ed-112">actionName</span><span class="sxs-lookup"><span data-stu-id="9f7ed-112">actionName</span></span>|<span data-ttu-id="9f7ed-113">String</span><span class="sxs-lookup"><span data-stu-id="9f7ed-113">String</span></span>|<span data-ttu-id="9f7ed-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9f7ed-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9f7ed-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9f7ed-115">actionState</span></span>|[<span data-ttu-id="9f7ed-116">actionState</span><span class="sxs-lookup"><span data-stu-id="9f7ed-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="9f7ed-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9f7ed-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9f7ed-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9f7ed-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9f7ed-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9f7ed-119">startDateTime</span></span>|<span data-ttu-id="9f7ed-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f7ed-120">DateTimeOffset</span></span>|<span data-ttu-id="9f7ed-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9f7ed-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9f7ed-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f7ed-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="9f7ed-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f7ed-123">DateTimeOffset</span></span>|<span data-ttu-id="9f7ed-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9f7ed-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9f7ed-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9f7ed-125">userPrincipalName</span></span>|<span data-ttu-id="9f7ed-126">String</span><span class="sxs-lookup"><span data-stu-id="9f7ed-126">String</span></span>|<span data-ttu-id="9f7ed-127">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="9f7ed-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="9f7ed-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="9f7ed-128">Relationships</span></span>
<span data-ttu-id="9f7ed-129">Нет</span><span class="sxs-lookup"><span data-stu-id="9f7ed-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9f7ed-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9f7ed-130">JSON Representation</span></span>
<span data-ttu-id="9f7ed-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9f7ed-131">Here is a JSON representation of the resource.</span></span>
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





