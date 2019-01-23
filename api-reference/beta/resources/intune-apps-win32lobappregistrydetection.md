---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для определения приложения Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb10a96a14d3c26503b33191fbb3c1b883245da7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402666"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="52fdd-103">Тип ресурса win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="52fdd-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="52fdd-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="52fdd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="52fdd-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="52fdd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52fdd-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52fdd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52fdd-107">Содержит свойства реестра для определения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="52fdd-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="52fdd-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="52fdd-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52fdd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="52fdd-109">Properties</span></span>
|<span data-ttu-id="52fdd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="52fdd-110">Property</span></span>|<span data-ttu-id="52fdd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="52fdd-111">Type</span></span>|<span data-ttu-id="52fdd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="52fdd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52fdd-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="52fdd-113">check32BitOn64System</span></span>|<span data-ttu-id="52fdd-114">Логический</span><span class="sxs-lookup"><span data-stu-id="52fdd-114">Boolean</span></span>|<span data-ttu-id="52fdd-115">Значение, указывающее, является ли этот путь в реестре для проверки 32-разрядная версия приложения на 64-разрядных систем</span><span class="sxs-lookup"><span data-stu-id="52fdd-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="52fdd-116">ключевого пути</span><span class="sxs-lookup"><span data-stu-id="52fdd-116">keyPath</span></span>|<span data-ttu-id="52fdd-117">String</span><span class="sxs-lookup"><span data-stu-id="52fdd-117">String</span></span>|<span data-ttu-id="52fdd-118">Путь к разделу реестра для определения Win32 строки из бизнес-приложения</span><span class="sxs-lookup"><span data-stu-id="52fdd-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="52fdd-119">Имени</span><span class="sxs-lookup"><span data-stu-id="52fdd-119">valueName</span></span>|<span data-ttu-id="52fdd-120">String</span><span class="sxs-lookup"><span data-stu-id="52fdd-120">String</span></span>|<span data-ttu-id="52fdd-121">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="52fdd-121">The registry value name</span></span>|
|<span data-ttu-id="52fdd-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="52fdd-122">detectionType</span></span>|[<span data-ttu-id="52fdd-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="52fdd-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="52fdd-124">Тип обнаружения данных реестра.</span><span class="sxs-lookup"><span data-stu-id="52fdd-124">The registry data detection type.</span></span> <span data-ttu-id="52fdd-125">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="52fdd-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="52fdd-126">operator</span><span class="sxs-lookup"><span data-stu-id="52fdd-126">operator</span></span>|[<span data-ttu-id="52fdd-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="52fdd-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="52fdd-128">Оператор для обнаружения данных реестра.</span><span class="sxs-lookup"><span data-stu-id="52fdd-128">The operator for registry data detection.</span></span> <span data-ttu-id="52fdd-129">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="52fdd-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="52fdd-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="52fdd-130">detectionValue</span></span>|<span data-ttu-id="52fdd-131">String</span><span class="sxs-lookup"><span data-stu-id="52fdd-131">String</span></span>|<span data-ttu-id="52fdd-132">Определение значения реестра</span><span class="sxs-lookup"><span data-stu-id="52fdd-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="52fdd-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="52fdd-133">Relationships</span></span>
<span data-ttu-id="52fdd-134">Нет</span><span class="sxs-lookup"><span data-stu-id="52fdd-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52fdd-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52fdd-135">JSON Representation</span></span>
<span data-ttu-id="52fdd-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52fdd-136">Here is a JSON representation of the resource.</span></span>
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




