---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для определения приложения Win32
ms.openlocfilehash: d0cab24f2f0eb4d0ad82d60285a4d0aca9ea6dda
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075867"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="e2836-103">Тип ресурса win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="e2836-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="e2836-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e2836-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e2836-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e2836-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e2836-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e2836-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2836-107">Содержит свойства реестра для определения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="e2836-107">Contains registry properties to detect a Win32 App</span></span>

<span data-ttu-id="e2836-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="e2836-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2836-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2836-109">Properties</span></span>
|<span data-ttu-id="e2836-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2836-110">Property</span></span>|<span data-ttu-id="e2836-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e2836-111">Type</span></span>|<span data-ttu-id="e2836-112">Description</span><span class="sxs-lookup"><span data-stu-id="e2836-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2836-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="e2836-113">check32BitOn64System</span></span>|<span data-ttu-id="e2836-114">Логический</span><span class="sxs-lookup"><span data-stu-id="e2836-114">Boolean</span></span>|<span data-ttu-id="e2836-115">Значение, указывающее, является ли этот путь в реестре для проверки 32-разрядная версия приложения на 64-разрядных систем</span><span class="sxs-lookup"><span data-stu-id="e2836-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="e2836-116">ключевого пути</span><span class="sxs-lookup"><span data-stu-id="e2836-116">keyPath</span></span>|<span data-ttu-id="e2836-117">String</span><span class="sxs-lookup"><span data-stu-id="e2836-117">String</span></span>|<span data-ttu-id="e2836-118">Путь к разделу реестра для определения Win32 строки из бизнес-приложения</span><span class="sxs-lookup"><span data-stu-id="e2836-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="e2836-119">Имени</span><span class="sxs-lookup"><span data-stu-id="e2836-119">valueName</span></span>|<span data-ttu-id="e2836-120">String</span><span class="sxs-lookup"><span data-stu-id="e2836-120">String</span></span>|<span data-ttu-id="e2836-121">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="e2836-121">The registry value name</span></span>|
|<span data-ttu-id="e2836-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="e2836-122">detectionType</span></span>|[<span data-ttu-id="e2836-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="e2836-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="e2836-124">Тип обнаружения данных реестра.</span><span class="sxs-lookup"><span data-stu-id="e2836-124">The registry data detection type.</span></span> <span data-ttu-id="e2836-125">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="e2836-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="e2836-126">operator</span><span class="sxs-lookup"><span data-stu-id="e2836-126">operator</span></span>|[<span data-ttu-id="e2836-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="e2836-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="e2836-128">Оператор для обнаружения данных реестра.</span><span class="sxs-lookup"><span data-stu-id="e2836-128">The operator for registry data detection.</span></span> <span data-ttu-id="e2836-129">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="e2836-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="e2836-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="e2836-130">detectionValue</span></span>|<span data-ttu-id="e2836-131">String</span><span class="sxs-lookup"><span data-stu-id="e2836-131">String</span></span>|<span data-ttu-id="e2836-132">Определение значения реестра</span><span class="sxs-lookup"><span data-stu-id="e2836-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2836-133">Связи</span><span class="sxs-lookup"><span data-stu-id="e2836-133">Relationships</span></span>
<span data-ttu-id="e2836-134">Нет</span><span class="sxs-lookup"><span data-stu-id="e2836-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2836-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2836-135">JSON Representation</span></span>
<span data-ttu-id="e2836-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2836-136">Here is a JSON representation of the resource.</span></span>
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





