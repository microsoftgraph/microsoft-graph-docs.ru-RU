---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2ca29d440f5721e16d13bf91dd366fb9e893108d
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610965"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="f32b3-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="f32b3-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="f32b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f32b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f32b3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f32b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f32b3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f32b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f32b3-107">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="f32b3-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="f32b3-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f32b3-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f32b3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="f32b3-109">Properties</span></span>
|<span data-ttu-id="f32b3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="f32b3-110">Property</span></span>|<span data-ttu-id="f32b3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="f32b3-111">Type</span></span>|<span data-ttu-id="f32b3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="f32b3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f32b3-113">actionName</span><span class="sxs-lookup"><span data-stu-id="f32b3-113">actionName</span></span>|<span data-ttu-id="f32b3-114">String</span><span class="sxs-lookup"><span data-stu-id="f32b3-114">String</span></span>|<span data-ttu-id="f32b3-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f32b3-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f32b3-116">actionState</span><span class="sxs-lookup"><span data-stu-id="f32b3-116">actionState</span></span>|[<span data-ttu-id="f32b3-117">actionState</span><span class="sxs-lookup"><span data-stu-id="f32b3-117">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="f32b3-118">Состояние действия, унаследованной от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f32b3-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="f32b3-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="f32b3-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="f32b3-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f32b3-120">startDateTime</span></span>|<span data-ttu-id="f32b3-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f32b3-121">DateTimeOffset</span></span>|<span data-ttu-id="f32b3-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="f32b3-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f32b3-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="f32b3-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="f32b3-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f32b3-124">DateTimeOffset</span></span>|<span data-ttu-id="f32b3-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="f32b3-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="f32b3-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f32b3-126">userPrincipalName</span></span>|<span data-ttu-id="f32b3-127">String</span><span class="sxs-lookup"><span data-stu-id="f32b3-127">String</span></span>|<span data-ttu-id="f32b3-128">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="f32b3-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="f32b3-129">Связи</span><span class="sxs-lookup"><span data-stu-id="f32b3-129">Relationships</span></span>
<span data-ttu-id="f32b3-130">Нет</span><span class="sxs-lookup"><span data-stu-id="f32b3-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f32b3-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f32b3-131">JSON Representation</span></span>
<span data-ttu-id="f32b3-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f32b3-132">Here is a JSON representation of the resource.</span></span>
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




