---
title: Тип ресурса win32LobAppRegistryRequirement
description: Содержит свойства реестра для обнаружения приложения Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 032300f73b249603c36d846db54b39ef050d6e69
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797572"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="b2bfa-103">Тип ресурса win32LobAppRegistryRequirement</span><span class="sxs-lookup"><span data-stu-id="b2bfa-103">win32LobAppRegistryRequirement resource type</span></span>

> <span data-ttu-id="b2bfa-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2bfa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2bfa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b2bfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2bfa-106">Содержит свойства реестра для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b2bfa-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="b2bfa-107">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="b2bfa-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b2bfa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2bfa-108">Properties</span></span>
|<span data-ttu-id="b2bfa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2bfa-109">Property</span></span>|<span data-ttu-id="b2bfa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b2bfa-110">Type</span></span>|<span data-ttu-id="b2bfa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2bfa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2bfa-112">operator</span><span class="sxs-lookup"><span data-stu-id="b2bfa-112">operator</span></span>|[<span data-ttu-id="b2bfa-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="b2bfa-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="b2bfa-114">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="b2bfa-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="b2bfa-115">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="b2bfa-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="b2bfa-116">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="b2bfa-116">detectionValue</span></span>|<span data-ttu-id="b2bfa-117">String</span><span class="sxs-lookup"><span data-stu-id="b2bfa-117">String</span></span>|<span data-ttu-id="b2bfa-118">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="b2bfa-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="b2bfa-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="b2bfa-119">check32BitOn64System</span></span>|<span data-ttu-id="b2bfa-120">Логический</span><span class="sxs-lookup"><span data-stu-id="b2bfa-120">Boolean</span></span>|<span data-ttu-id="b2bfa-121">Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="b2bfa-121">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="b2bfa-122">Ключевой</span><span class="sxs-lookup"><span data-stu-id="b2bfa-122">keyPath</span></span>|<span data-ttu-id="b2bfa-123">String</span><span class="sxs-lookup"><span data-stu-id="b2bfa-123">String</span></span>|<span data-ttu-id="b2bfa-124">Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)</span><span class="sxs-lookup"><span data-stu-id="b2bfa-124">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="b2bfa-125">valueName</span><span class="sxs-lookup"><span data-stu-id="b2bfa-125">valueName</span></span>|<span data-ttu-id="b2bfa-126">String</span><span class="sxs-lookup"><span data-stu-id="b2bfa-126">String</span></span>|<span data-ttu-id="b2bfa-127">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="b2bfa-127">The registry value name</span></span>|
|<span data-ttu-id="b2bfa-128">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="b2bfa-128">detectionType</span></span>|[<span data-ttu-id="b2bfa-129">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="b2bfa-129">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="b2bfa-130">Тип обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="b2bfa-130">The registry data detection type.</span></span> <span data-ttu-id="b2bfa-131">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="b2bfa-131">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2bfa-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b2bfa-132">Relationships</span></span>
<span data-ttu-id="b2bfa-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b2bfa-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2bfa-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2bfa-134">JSON Representation</span></span>
<span data-ttu-id="b2bfa-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2bfa-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryRequirement",
  "operator": "String",
  "detectionValue": "String",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String"
}
```



