---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 09448e70e80ca07c9f556e698f70a0e17d4eb820
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785030"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="44c9b-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="44c9b-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

> <span data-ttu-id="44c9b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44c9b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44c9b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44c9b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44c9b-106">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="44c9b-106">Delete user from shared apple device action result</span></span>


<span data-ttu-id="44c9b-107">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="44c9b-107">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="44c9b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="44c9b-108">Properties</span></span>
|<span data-ttu-id="44c9b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="44c9b-109">Property</span></span>|<span data-ttu-id="44c9b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="44c9b-110">Type</span></span>|<span data-ttu-id="44c9b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="44c9b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44c9b-112">actionName</span><span class="sxs-lookup"><span data-stu-id="44c9b-112">actionName</span></span>|<span data-ttu-id="44c9b-113">String</span><span class="sxs-lookup"><span data-stu-id="44c9b-113">String</span></span>|<span data-ttu-id="44c9b-114">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="44c9b-114">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="44c9b-115">actionState</span><span class="sxs-lookup"><span data-stu-id="44c9b-115">actionState</span></span>|[<span data-ttu-id="44c9b-116">actionState</span><span class="sxs-lookup"><span data-stu-id="44c9b-116">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="44c9b-117">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="44c9b-117">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="44c9b-118">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="44c9b-118">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="44c9b-119">startDateTime</span><span class="sxs-lookup"><span data-stu-id="44c9b-119">startDateTime</span></span>|<span data-ttu-id="44c9b-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44c9b-120">DateTimeOffset</span></span>|<span data-ttu-id="44c9b-121">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="44c9b-121">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="44c9b-122">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="44c9b-122">lastUpdatedDateTime</span></span>|<span data-ttu-id="44c9b-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44c9b-123">DateTimeOffset</span></span>|<span data-ttu-id="44c9b-124">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="44c9b-124">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="44c9b-125">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="44c9b-125">userPrincipalName</span></span>|<span data-ttu-id="44c9b-126">String</span><span class="sxs-lookup"><span data-stu-id="44c9b-126">String</span></span>|<span data-ttu-id="44c9b-127">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="44c9b-127">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="44c9b-128">Связи</span><span class="sxs-lookup"><span data-stu-id="44c9b-128">Relationships</span></span>
<span data-ttu-id="44c9b-129">Нет</span><span class="sxs-lookup"><span data-stu-id="44c9b-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44c9b-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44c9b-130">JSON Representation</span></span>
<span data-ttu-id="44c9b-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44c9b-131">Here is a JSON representation of the resource.</span></span>
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



