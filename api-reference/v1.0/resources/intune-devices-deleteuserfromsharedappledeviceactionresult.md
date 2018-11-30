---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
ms.openlocfilehash: dc21e22ca2e819835178a7cb2ed3aa824cd40004
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024460"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="7f997-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="7f997-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="7f997-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7f997-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f997-105">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="7f997-105">Delete user from shared apple device action result</span></span>

<span data-ttu-id="7f997-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7f997-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f997-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7f997-107">Properties</span></span>
|<span data-ttu-id="7f997-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f997-108">Property</span></span>|<span data-ttu-id="7f997-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7f997-109">Type</span></span>|<span data-ttu-id="7f997-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7f997-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f997-111">actionName</span><span class="sxs-lookup"><span data-stu-id="7f997-111">actionName</span></span>|<span data-ttu-id="7f997-112">String</span><span class="sxs-lookup"><span data-stu-id="7f997-112">String</span></span>|<span data-ttu-id="7f997-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7f997-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7f997-114">actionState</span><span class="sxs-lookup"><span data-stu-id="7f997-114">actionState</span></span>|[<span data-ttu-id="7f997-115">actionState</span><span class="sxs-lookup"><span data-stu-id="7f997-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="7f997-116">Состояние действие унаследованные от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="7f997-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="7f997-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="7f997-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="7f997-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7f997-118">startDateTime</span></span>|<span data-ttu-id="7f997-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f997-119">DateTimeOffset</span></span>|<span data-ttu-id="7f997-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7f997-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7f997-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f997-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="7f997-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f997-122">DateTimeOffset</span></span>|<span data-ttu-id="7f997-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="7f997-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="7f997-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7f997-124">userPrincipalName</span></span>|<span data-ttu-id="7f997-125">String</span><span class="sxs-lookup"><span data-stu-id="7f997-125">String</span></span>|<span data-ttu-id="7f997-126">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="7f997-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f997-127">Связи</span><span class="sxs-lookup"><span data-stu-id="7f997-127">Relationships</span></span>
<span data-ttu-id="7f997-128">Нет</span><span class="sxs-lookup"><span data-stu-id="7f997-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f997-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7f997-129">JSON Representation</span></span>
<span data-ttu-id="7f997-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f997-130">Here is a JSON representation of the resource.</span></span>
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



