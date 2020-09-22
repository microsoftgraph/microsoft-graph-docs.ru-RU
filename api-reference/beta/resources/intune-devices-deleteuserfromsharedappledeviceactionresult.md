---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6d615aa333f184569ec3f1424a4aa154407c1ce8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060603"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="c4238-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="c4238-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="c4238-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4238-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4238-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4238-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4238-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4238-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4238-107">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="c4238-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="c4238-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c4238-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c4238-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4238-109">Properties</span></span>
|<span data-ttu-id="c4238-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4238-110">Property</span></span>|<span data-ttu-id="c4238-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c4238-111">Type</span></span>|<span data-ttu-id="c4238-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c4238-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4238-113">actionName</span><span class="sxs-lookup"><span data-stu-id="c4238-113">actionName</span></span>|<span data-ttu-id="c4238-114">String</span><span class="sxs-lookup"><span data-stu-id="c4238-114">String</span></span>|<span data-ttu-id="c4238-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c4238-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c4238-116">actionState</span><span class="sxs-lookup"><span data-stu-id="c4238-116">actionState</span></span>|[<span data-ttu-id="c4238-117">actionState</span><span class="sxs-lookup"><span data-stu-id="c4238-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c4238-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c4238-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="c4238-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="c4238-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c4238-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c4238-120">startDateTime</span></span>|<span data-ttu-id="c4238-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4238-121">DateTimeOffset</span></span>|<span data-ttu-id="c4238-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="c4238-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c4238-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="c4238-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="c4238-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4238-124">DateTimeOffset</span></span>|<span data-ttu-id="c4238-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="c4238-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="c4238-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c4238-126">userPrincipalName</span></span>|<span data-ttu-id="c4238-127">String</span><span class="sxs-lookup"><span data-stu-id="c4238-127">String</span></span>|<span data-ttu-id="c4238-128">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="c4238-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4238-129">Связи</span><span class="sxs-lookup"><span data-stu-id="c4238-129">Relationships</span></span>
<span data-ttu-id="c4238-130">Нет</span><span class="sxs-lookup"><span data-stu-id="c4238-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4238-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4238-131">JSON Representation</span></span>
<span data-ttu-id="c4238-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4238-132">Here is a JSON representation of the resource.</span></span>
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






