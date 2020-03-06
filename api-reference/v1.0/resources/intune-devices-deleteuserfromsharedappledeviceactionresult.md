---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 921efba76fa290c104c33544c6801f40aa941dde
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532208"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="08475-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="08475-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="08475-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08475-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08475-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08475-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08475-106">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="08475-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="08475-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="08475-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08475-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="08475-108">Properties</span></span>
|<span data-ttu-id="08475-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="08475-109">Property</span></span>|<span data-ttu-id="08475-110">Тип</span><span class="sxs-lookup"><span data-stu-id="08475-110">Type</span></span>|<span data-ttu-id="08475-111">Описание</span><span class="sxs-lookup"><span data-stu-id="08475-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08475-112">actionName</span><span class="sxs-lookup"><span data-stu-id="08475-112">actionName</span></span>|<span data-ttu-id="08475-113">String</span><span class="sxs-lookup"><span data-stu-id="08475-113">String</span></span>|<span data-ttu-id="08475-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="08475-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="08475-115">actionState</span><span class="sxs-lookup"><span data-stu-id="08475-115">actionState</span></span>|[<span data-ttu-id="08475-116">actionState</span><span class="sxs-lookup"><span data-stu-id="08475-116">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="08475-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="08475-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="08475-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="08475-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="08475-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="08475-119">startDateTime</span></span>|<span data-ttu-id="08475-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08475-120">DateTimeOffset</span></span>|<span data-ttu-id="08475-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="08475-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="08475-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="08475-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="08475-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08475-123">DateTimeOffset</span></span>|<span data-ttu-id="08475-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="08475-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="08475-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="08475-125">userPrincipalName</span></span>|<span data-ttu-id="08475-126">String</span><span class="sxs-lookup"><span data-stu-id="08475-126">String</span></span>|<span data-ttu-id="08475-127">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="08475-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="08475-128">Связи</span><span class="sxs-lookup"><span data-stu-id="08475-128">Relationships</span></span>
<span data-ttu-id="08475-129">Нет</span><span class="sxs-lookup"><span data-stu-id="08475-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08475-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08475-130">JSON Representation</span></span>
<span data-ttu-id="08475-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08475-131">Here is a JSON representation of the resource.</span></span>
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




