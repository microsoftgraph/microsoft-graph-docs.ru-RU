---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5071c0c9168cfedbbaa527f82241c80b4ad53705
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261525"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="b0f2e-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="b0f2e-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="b0f2e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0f2e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0f2e-105">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="b0f2e-105">Delete user from shared apple device action result</span></span>


<span data-ttu-id="b0f2e-106">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0f2e-106">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0f2e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0f2e-107">Properties</span></span>
|<span data-ttu-id="b0f2e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0f2e-108">Property</span></span>|<span data-ttu-id="b0f2e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b0f2e-109">Type</span></span>|<span data-ttu-id="b0f2e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b0f2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0f2e-111">actionName</span><span class="sxs-lookup"><span data-stu-id="b0f2e-111">actionName</span></span>|<span data-ttu-id="b0f2e-112">String</span><span class="sxs-lookup"><span data-stu-id="b0f2e-112">String</span></span>|<span data-ttu-id="b0f2e-113">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0f2e-113">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0f2e-114">actionState</span><span class="sxs-lookup"><span data-stu-id="b0f2e-114">actionState</span></span>|[<span data-ttu-id="b0f2e-115">actionState</span><span class="sxs-lookup"><span data-stu-id="b0f2e-115">actionState</span></span>](../resources/intune-devices-actionstate.md)|<span data-ttu-id="b0f2e-116">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="b0f2e-116">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="b0f2e-117">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="b0f2e-117">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="b0f2e-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b0f2e-118">startDateTime</span></span>|<span data-ttu-id="b0f2e-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0f2e-119">DateTimeOffset</span></span>|<span data-ttu-id="b0f2e-120">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0f2e-120">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0f2e-121">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0f2e-121">lastUpdatedDateTime</span></span>|<span data-ttu-id="b0f2e-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0f2e-122">DateTimeOffset</span></span>|<span data-ttu-id="b0f2e-123">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="b0f2e-123">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="b0f2e-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0f2e-124">userPrincipalName</span></span>|<span data-ttu-id="b0f2e-125">String</span><span class="sxs-lookup"><span data-stu-id="b0f2e-125">String</span></span>|<span data-ttu-id="b0f2e-126">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="b0f2e-126">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0f2e-127">Связи</span><span class="sxs-lookup"><span data-stu-id="b0f2e-127">Relationships</span></span>
<span data-ttu-id="b0f2e-128">Нет</span><span class="sxs-lookup"><span data-stu-id="b0f2e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0f2e-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0f2e-129">JSON Representation</span></span>
<span data-ttu-id="b0f2e-130">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0f2e-130">Here is a JSON representation of the resource.</span></span>
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



