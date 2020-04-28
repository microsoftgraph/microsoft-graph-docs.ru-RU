---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b6f28d6c042ab86273cd11d9e756bb4941e315b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422741"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="e47f5-103">Тип ресурса win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="e47f5-103">win32LobAppRegistryDetection resource type</span></span>

<span data-ttu-id="e47f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e47f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e47f5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e47f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e47f5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e47f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e47f5-107">Содержит свойства реестра для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="e47f5-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="e47f5-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="e47f5-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e47f5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e47f5-109">Properties</span></span>
|<span data-ttu-id="e47f5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e47f5-110">Property</span></span>|<span data-ttu-id="e47f5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e47f5-111">Type</span></span>|<span data-ttu-id="e47f5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e47f5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e47f5-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="e47f5-113">check32BitOn64System</span></span>|<span data-ttu-id="e47f5-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="e47f5-114">Boolean</span></span>|<span data-ttu-id="e47f5-115">Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="e47f5-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="e47f5-116">Ключевой</span><span class="sxs-lookup"><span data-stu-id="e47f5-116">keyPath</span></span>|<span data-ttu-id="e47f5-117">String</span><span class="sxs-lookup"><span data-stu-id="e47f5-117">String</span></span>|<span data-ttu-id="e47f5-118">Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)</span><span class="sxs-lookup"><span data-stu-id="e47f5-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="e47f5-119">valueName</span><span class="sxs-lookup"><span data-stu-id="e47f5-119">valueName</span></span>|<span data-ttu-id="e47f5-120">String</span><span class="sxs-lookup"><span data-stu-id="e47f5-120">String</span></span>|<span data-ttu-id="e47f5-121">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="e47f5-121">The registry value name</span></span>|
|<span data-ttu-id="e47f5-122">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="e47f5-122">detectionType</span></span>|[<span data-ttu-id="e47f5-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="e47f5-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="e47f5-124">Тип обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="e47f5-124">The registry data detection type.</span></span> <span data-ttu-id="e47f5-125">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="e47f5-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="e47f5-126">operator</span><span class="sxs-lookup"><span data-stu-id="e47f5-126">operator</span></span>|[<span data-ttu-id="e47f5-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="e47f5-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="e47f5-128">Оператор для обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="e47f5-128">The operator for registry data detection.</span></span> <span data-ttu-id="e47f5-129">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="e47f5-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e47f5-130">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="e47f5-130">detectionValue</span></span>|<span data-ttu-id="e47f5-131">String</span><span class="sxs-lookup"><span data-stu-id="e47f5-131">String</span></span>|<span data-ttu-id="e47f5-132">Значение обнаружения в реестре</span><span class="sxs-lookup"><span data-stu-id="e47f5-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="e47f5-133">Связи</span><span class="sxs-lookup"><span data-stu-id="e47f5-133">Relationships</span></span>
<span data-ttu-id="e47f5-134">Нет</span><span class="sxs-lookup"><span data-stu-id="e47f5-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e47f5-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e47f5-135">JSON Representation</span></span>
<span data-ttu-id="e47f5-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e47f5-136">Here is a JSON representation of the resource.</span></span>
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



