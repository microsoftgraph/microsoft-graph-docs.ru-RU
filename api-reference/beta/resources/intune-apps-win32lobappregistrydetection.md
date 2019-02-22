---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для обнаружения приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 076251ea185359127c3dad3610ec944f7cdb3178
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169547"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="3ccf4-103">Тип ресурса win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="3ccf4-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="3ccf4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ccf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ccf4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ccf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ccf4-106">Содержит свойства реестра для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="3ccf4-106">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="3ccf4-107">НаСледуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="3ccf4-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ccf4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3ccf4-108">Properties</span></span>
|<span data-ttu-id="3ccf4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ccf4-109">Property</span></span>|<span data-ttu-id="3ccf4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3ccf4-110">Type</span></span>|<span data-ttu-id="3ccf4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3ccf4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ccf4-112">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="3ccf4-112">check32BitOn64System</span></span>|<span data-ttu-id="3ccf4-113">Логический</span><span class="sxs-lookup"><span data-stu-id="3ccf4-113">Boolean</span></span>|<span data-ttu-id="3ccf4-114">Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="3ccf4-114">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="3ccf4-115">Ключевой</span><span class="sxs-lookup"><span data-stu-id="3ccf4-115">keyPath</span></span>|<span data-ttu-id="3ccf4-116">String</span><span class="sxs-lookup"><span data-stu-id="3ccf4-116">String</span></span>|<span data-ttu-id="3ccf4-117">Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)</span><span class="sxs-lookup"><span data-stu-id="3ccf4-117">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="3ccf4-118">valueName</span><span class="sxs-lookup"><span data-stu-id="3ccf4-118">valueName</span></span>|<span data-ttu-id="3ccf4-119">String</span><span class="sxs-lookup"><span data-stu-id="3ccf4-119">String</span></span>|<span data-ttu-id="3ccf4-120">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="3ccf4-120">The registry value name</span></span>|
|<span data-ttu-id="3ccf4-121">Детектионтипе</span><span class="sxs-lookup"><span data-stu-id="3ccf4-121">detectionType</span></span>|[<span data-ttu-id="3ccf4-122">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="3ccf4-122">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="3ccf4-123">Тип обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="3ccf4-123">The registry data detection type.</span></span> <span data-ttu-id="3ccf4-124">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="3ccf4-124">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="3ccf4-125">operator</span><span class="sxs-lookup"><span data-stu-id="3ccf4-125">operator</span></span>|[<span data-ttu-id="3ccf4-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="3ccf4-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="3ccf4-127">Оператор для обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="3ccf4-127">The operator for registry data detection.</span></span> <span data-ttu-id="3ccf4-128">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="3ccf4-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="3ccf4-129">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="3ccf4-129">detectionValue</span></span>|<span data-ttu-id="3ccf4-130">String</span><span class="sxs-lookup"><span data-stu-id="3ccf4-130">String</span></span>|<span data-ttu-id="3ccf4-131">Значение обнаружения в реестре</span><span class="sxs-lookup"><span data-stu-id="3ccf4-131">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ccf4-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="3ccf4-132">Relationships</span></span>
<span data-ttu-id="3ccf4-133">Нет</span><span class="sxs-lookup"><span data-stu-id="3ccf4-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ccf4-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3ccf4-134">JSON Representation</span></span>
<span data-ttu-id="3ccf4-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ccf4-135">Here is a JSON representation of the resource.</span></span>
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




