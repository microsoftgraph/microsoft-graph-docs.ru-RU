---
title: Тип ресурса win32LobAppRegistryRequirement
description: Содержит свойства реестра для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ba7d763416a45a8ced276ae738009ea0c03e32a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422655"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="aa64e-103">Тип ресурса win32LobAppRegistryRequirement</span><span class="sxs-lookup"><span data-stu-id="aa64e-103">win32LobAppRegistryRequirement resource type</span></span>

<span data-ttu-id="aa64e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa64e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aa64e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aa64e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa64e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="aa64e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa64e-107">Содержит свойства реестра для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="aa64e-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="aa64e-108">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="aa64e-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa64e-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="aa64e-109">Properties</span></span>
|<span data-ttu-id="aa64e-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="aa64e-110">Property</span></span>|<span data-ttu-id="aa64e-111">Тип</span><span class="sxs-lookup"><span data-stu-id="aa64e-111">Type</span></span>|<span data-ttu-id="aa64e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="aa64e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa64e-113">operator</span><span class="sxs-lookup"><span data-stu-id="aa64e-113">operator</span></span>|[<span data-ttu-id="aa64e-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="aa64e-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="aa64e-115">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="aa64e-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="aa64e-116">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="aa64e-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="aa64e-117">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="aa64e-117">detectionValue</span></span>|<span data-ttu-id="aa64e-118">String</span><span class="sxs-lookup"><span data-stu-id="aa64e-118">String</span></span>|<span data-ttu-id="aa64e-119">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="aa64e-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="aa64e-120">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="aa64e-120">check32BitOn64System</span></span>|<span data-ttu-id="aa64e-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa64e-121">Boolean</span></span>|<span data-ttu-id="aa64e-122">Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="aa64e-122">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="aa64e-123">Ключевой</span><span class="sxs-lookup"><span data-stu-id="aa64e-123">keyPath</span></span>|<span data-ttu-id="aa64e-124">String</span><span class="sxs-lookup"><span data-stu-id="aa64e-124">String</span></span>|<span data-ttu-id="aa64e-125">Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)</span><span class="sxs-lookup"><span data-stu-id="aa64e-125">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="aa64e-126">valueName</span><span class="sxs-lookup"><span data-stu-id="aa64e-126">valueName</span></span>|<span data-ttu-id="aa64e-127">String</span><span class="sxs-lookup"><span data-stu-id="aa64e-127">String</span></span>|<span data-ttu-id="aa64e-128">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="aa64e-128">The registry value name</span></span>|
|<span data-ttu-id="aa64e-129">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="aa64e-129">detectionType</span></span>|[<span data-ttu-id="aa64e-130">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="aa64e-130">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="aa64e-131">Тип обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="aa64e-131">The registry data detection type.</span></span> <span data-ttu-id="aa64e-132">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="aa64e-132">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa64e-133">Связи</span><span class="sxs-lookup"><span data-stu-id="aa64e-133">Relationships</span></span>
<span data-ttu-id="aa64e-134">Нет</span><span class="sxs-lookup"><span data-stu-id="aa64e-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa64e-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="aa64e-135">JSON Representation</span></span>
<span data-ttu-id="aa64e-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="aa64e-136">Here is a JSON representation of the resource.</span></span>
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



