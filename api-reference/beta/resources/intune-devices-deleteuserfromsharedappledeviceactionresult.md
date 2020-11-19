---
title: Тип ресурса deleteUserFromSharedAppleDeviceActionResult
description: Результат удаления пользователя с общего устройства Apple
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8193551aed2a3604f79978d3907c9af6728b6eb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267834"
---
# <a name="deleteuserfromsharedappledeviceactionresult-resource-type"></a><span data-ttu-id="d0f37-103">Тип ресурса deleteUserFromSharedAppleDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="d0f37-103">deleteUserFromSharedAppleDeviceActionResult resource type</span></span>

<span data-ttu-id="d0f37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0f37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0f37-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0f37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0f37-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d0f37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0f37-107">Результат удаления пользователя с общего устройства Apple</span><span class="sxs-lookup"><span data-stu-id="d0f37-107">Delete user from shared apple device action result</span></span>


<span data-ttu-id="d0f37-108">Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0f37-108">Inherits from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d0f37-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="d0f37-109">Properties</span></span>
|<span data-ttu-id="d0f37-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="d0f37-110">Property</span></span>|<span data-ttu-id="d0f37-111">Тип</span><span class="sxs-lookup"><span data-stu-id="d0f37-111">Type</span></span>|<span data-ttu-id="d0f37-112">Описание</span><span class="sxs-lookup"><span data-stu-id="d0f37-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0f37-113">actionName</span><span class="sxs-lookup"><span data-stu-id="d0f37-113">actionName</span></span>|<span data-ttu-id="d0f37-114">String</span><span class="sxs-lookup"><span data-stu-id="d0f37-114">String</span></span>|<span data-ttu-id="d0f37-115">Название действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d0f37-115">Action name Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0f37-116">actionState</span><span class="sxs-lookup"><span data-stu-id="d0f37-116">actionState</span></span>|[<span data-ttu-id="d0f37-117">actionState</span><span class="sxs-lookup"><span data-stu-id="d0f37-117">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="d0f37-118">Состояние действия, унаследованного от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d0f37-118">State of the action Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span></span> <span data-ttu-id="d0f37-119">Возможные значения: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span><span class="sxs-lookup"><span data-stu-id="d0f37-119">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="d0f37-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f37-120">startDateTime</span></span>|<span data-ttu-id="d0f37-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f37-121">DateTimeOffset</span></span>|<span data-ttu-id="d0f37-122">Время начала действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md).</span><span class="sxs-lookup"><span data-stu-id="d0f37-122">Time the action was initiated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0f37-123">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0f37-123">lastUpdatedDateTime</span></span>|<span data-ttu-id="d0f37-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0f37-124">DateTimeOffset</span></span>|<span data-ttu-id="d0f37-125">Время последнего обновления действия. Наследуется от [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span><span class="sxs-lookup"><span data-stu-id="d0f37-125">Time the action state was last updated Inherited from [deviceActionResult](../resources/intune-devices-deviceactionresult.md)</span></span>|
|<span data-ttu-id="d0f37-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0f37-126">userPrincipalName</span></span>|<span data-ttu-id="d0f37-127">String</span><span class="sxs-lookup"><span data-stu-id="d0f37-127">String</span></span>|<span data-ttu-id="d0f37-128">Имя участника-пользователя для удаляемого пользователя</span><span class="sxs-lookup"><span data-stu-id="d0f37-128">User principal name of the user to be deleted</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0f37-129">Связи</span><span class="sxs-lookup"><span data-stu-id="d0f37-129">Relationships</span></span>
<span data-ttu-id="d0f37-130">Нет</span><span class="sxs-lookup"><span data-stu-id="d0f37-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0f37-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d0f37-131">JSON Representation</span></span>
<span data-ttu-id="d0f37-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d0f37-132">Here is a JSON representation of the resource.</span></span>
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




