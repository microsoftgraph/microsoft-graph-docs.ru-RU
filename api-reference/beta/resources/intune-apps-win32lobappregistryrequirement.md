---
title: Тип ресурса win32LobAppRegistryRequirement
description: Содержит свойства реестра для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a75e30c0cc84f9e775f4ee304e27eacb42b409f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975807"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="5e27e-103">Тип ресурса win32LobAppRegistryRequirement</span><span class="sxs-lookup"><span data-stu-id="5e27e-103">win32LobAppRegistryRequirement resource type</span></span>

> <span data-ttu-id="5e27e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e27e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5e27e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e27e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e27e-106">Содержит свойства реестра для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="5e27e-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="5e27e-107">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="5e27e-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5e27e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e27e-108">Properties</span></span>
|<span data-ttu-id="5e27e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e27e-109">Property</span></span>|<span data-ttu-id="5e27e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5e27e-110">Type</span></span>|<span data-ttu-id="5e27e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5e27e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e27e-112">operator</span><span class="sxs-lookup"><span data-stu-id="5e27e-112">operator</span></span>|[<span data-ttu-id="5e27e-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="5e27e-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="5e27e-114">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="5e27e-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="5e27e-115">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="5e27e-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="5e27e-116">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="5e27e-116">detectionValue</span></span>|<span data-ttu-id="5e27e-117">String</span><span class="sxs-lookup"><span data-stu-id="5e27e-117">String</span></span>|<span data-ttu-id="5e27e-118">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="5e27e-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="5e27e-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="5e27e-119">check32BitOn64System</span></span>|<span data-ttu-id="5e27e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e27e-120">Boolean</span></span>|<span data-ttu-id="5e27e-121">Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="5e27e-121">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="5e27e-122">Ключевой</span><span class="sxs-lookup"><span data-stu-id="5e27e-122">keyPath</span></span>|<span data-ttu-id="5e27e-123">String</span><span class="sxs-lookup"><span data-stu-id="5e27e-123">String</span></span>|<span data-ttu-id="5e27e-124">Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)</span><span class="sxs-lookup"><span data-stu-id="5e27e-124">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="5e27e-125">valueName</span><span class="sxs-lookup"><span data-stu-id="5e27e-125">valueName</span></span>|<span data-ttu-id="5e27e-126">String</span><span class="sxs-lookup"><span data-stu-id="5e27e-126">String</span></span>|<span data-ttu-id="5e27e-127">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="5e27e-127">The registry value name</span></span>|
|<span data-ttu-id="5e27e-128">Детектионтипе</span><span class="sxs-lookup"><span data-stu-id="5e27e-128">detectionType</span></span>|[<span data-ttu-id="5e27e-129">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="5e27e-129">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="5e27e-130">Тип обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="5e27e-130">The registry data detection type.</span></span> <span data-ttu-id="5e27e-131">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="5e27e-131">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e27e-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="5e27e-132">Relationships</span></span>
<span data-ttu-id="5e27e-133">Нет</span><span class="sxs-lookup"><span data-stu-id="5e27e-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e27e-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e27e-134">JSON Representation</span></span>
<span data-ttu-id="5e27e-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e27e-135">Here is a JSON representation of the resource.</span></span>
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





