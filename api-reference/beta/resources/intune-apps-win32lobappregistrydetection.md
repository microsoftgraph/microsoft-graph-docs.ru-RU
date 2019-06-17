---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3013ca82a0545379c96cf832818783dedd4576f4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986108"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="68cf8-103">Тип ресурса win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="68cf8-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="68cf8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68cf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68cf8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68cf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68cf8-106">Содержит свойства реестра для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="68cf8-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="68cf8-107">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="68cf8-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68cf8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="68cf8-108">Properties</span></span>
|<span data-ttu-id="68cf8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="68cf8-109">Property</span></span>|<span data-ttu-id="68cf8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="68cf8-110">Type</span></span>|<span data-ttu-id="68cf8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="68cf8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68cf8-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="68cf8-112">check32BitOn64System</span></span>|<span data-ttu-id="68cf8-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="68cf8-113">Boolean</span></span>|<span data-ttu-id="68cf8-114">Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="68cf8-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="68cf8-115">Ключевой</span><span class="sxs-lookup"><span data-stu-id="68cf8-115">keyPath</span></span>|<span data-ttu-id="68cf8-116">String</span><span class="sxs-lookup"><span data-stu-id="68cf8-116">String</span></span>|<span data-ttu-id="68cf8-117">Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)</span><span class="sxs-lookup"><span data-stu-id="68cf8-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="68cf8-118">valueName</span><span class="sxs-lookup"><span data-stu-id="68cf8-118">valueName</span></span>|<span data-ttu-id="68cf8-119">String</span><span class="sxs-lookup"><span data-stu-id="68cf8-119">String</span></span>|<span data-ttu-id="68cf8-120">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="68cf8-120">The registry value name</span></span>|
|<span data-ttu-id="68cf8-121">Детектионтипе</span><span class="sxs-lookup"><span data-stu-id="68cf8-121">detectionType</span></span>|[<span data-ttu-id="68cf8-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="68cf8-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="68cf8-123">Тип обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="68cf8-123">The registry data detection type.</span></span> <span data-ttu-id="68cf8-124">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="68cf8-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="68cf8-125">operator</span><span class="sxs-lookup"><span data-stu-id="68cf8-125">operator</span></span>|[<span data-ttu-id="68cf8-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="68cf8-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="68cf8-127">Оператор для обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="68cf8-127">The operator for registry data detection.</span></span> <span data-ttu-id="68cf8-128">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="68cf8-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="68cf8-129">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="68cf8-129">detectionValue</span></span>|<span data-ttu-id="68cf8-130">String</span><span class="sxs-lookup"><span data-stu-id="68cf8-130">String</span></span>|<span data-ttu-id="68cf8-131">Значение обнаружения в реестре</span><span class="sxs-lookup"><span data-stu-id="68cf8-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="68cf8-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="68cf8-132">Relationships</span></span>
<span data-ttu-id="68cf8-133">Нет</span><span class="sxs-lookup"><span data-stu-id="68cf8-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68cf8-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68cf8-134">JSON Representation</span></span>
<span data-ttu-id="68cf8-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68cf8-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





