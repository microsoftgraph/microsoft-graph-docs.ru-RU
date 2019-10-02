---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88ed9a813b678381b32f2b054933e9d3ad28683d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357033"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="9fb29-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="9fb29-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="9fb29-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9fb29-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fb29-105">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="9fb29-105">Delete user from shared apple device action result</span></span>


<span data-ttu-id="9fb29-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9fb29-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9fb29-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fb29-107">Properties</span></span>
|<span data-ttu-id="9fb29-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fb29-108">Property</span></span>|<span data-ttu-id="9fb29-109">Тип</span><span class="sxs-lookup"><span data-stu-id="9fb29-109">Type</span></span>|<span data-ttu-id="9fb29-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9fb29-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fb29-111">actionName</span><span class="sxs-lookup"><span data-stu-id="9fb29-111">actionName</span></span>|<span data-ttu-id="9fb29-112">String</span><span class="sxs-lookup"><span data-stu-id="9fb29-112">String</span></span>|<span data-ttu-id="9fb29-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9fb29-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9fb29-114">actionState</span><span class="sxs-lookup"><span data-stu-id="9fb29-114">actionState</span></span>|[<span data-ttu-id="9fb29-115">actionState</span><span class="sxs-lookup"><span data-stu-id="9fb29-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="9fb29-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9fb29-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="9fb29-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="9fb29-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="9fb29-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9fb29-118">startDateTime</span></span>|<span data-ttu-id="9fb29-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fb29-119">DateTimeOffset</span></span>|<span data-ttu-id="9fb29-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="9fb29-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9fb29-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fb29-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="9fb29-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fb29-122">DateTimeOffset</span></span>|<span data-ttu-id="9fb29-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="9fb29-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="9fb29-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9fb29-124">userPrincipalName</span></span>|<span data-ttu-id="9fb29-125">String</span><span class="sxs-lookup"><span data-stu-id="9fb29-125">String</span></span>|<span data-ttu-id="9fb29-126">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="9fb29-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="9fb29-127">Связи</span><span class="sxs-lookup"><span data-stu-id="9fb29-127">Relationships</span></span>
<span data-ttu-id="9fb29-128">Нет</span><span class="sxs-lookup"><span data-stu-id="9fb29-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fb29-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9fb29-129">JSON Representation</span></span>
<span data-ttu-id="9fb29-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fb29-130">Here is a JSON representation of the resource.</span></span>
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




