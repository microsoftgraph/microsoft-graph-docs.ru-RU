---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для определения приложения Win32
author: tfitzmac
ms.openlocfilehash: 5adeca1b569531d15657acc2a8960bab60580dc6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347742"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="10929-103">Тип ресурса win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="10929-103">win32LobAppRegistryDetection resource type</span></span>

> <span data-ttu-id="10929-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="10929-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10929-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10929-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10929-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="10929-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10929-107">Содержит свойства реестра для определения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="10929-107">Contains registry properties to detect a Win32 App</span></span>

<span data-ttu-id="10929-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="10929-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="10929-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="10929-109">Properties</span></span>
|<span data-ttu-id="10929-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="10929-110">Property</span></span>|<span data-ttu-id="10929-111">Тип</span><span class="sxs-lookup"><span data-stu-id="10929-111">Type</span></span>|<span data-ttu-id="10929-112">Описание</span><span class="sxs-lookup"><span data-stu-id="10929-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10929-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="10929-113">check32BitOn64System</span></span>|<span data-ttu-id="10929-114">Boolean.</span><span class="sxs-lookup"><span data-stu-id="10929-114">Boolean</span></span>|<span data-ttu-id="10929-115">Значение, указывающее, является ли этот путь в реестре для проверки 32-разрядная версия приложения на 64-разрядных систем</span><span class="sxs-lookup"><span data-stu-id="10929-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="10929-116">ключевого пути</span><span class="sxs-lookup"><span data-stu-id="10929-116">keyPath</span></span>|<span data-ttu-id="10929-117">String.</span><span class="sxs-lookup"><span data-stu-id="10929-117">String</span></span>|<span data-ttu-id="10929-118">Путь к разделу реестра для определения Win32 строки из бизнес-приложения</span><span class="sxs-lookup"><span data-stu-id="10929-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="10929-119">Имени</span><span class="sxs-lookup"><span data-stu-id="10929-119">valueName</span></span>|<span data-ttu-id="10929-120">String.</span><span class="sxs-lookup"><span data-stu-id="10929-120">String</span></span>|<span data-ttu-id="10929-121">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="10929-121">The registry value name</span></span>|
|<span data-ttu-id="10929-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="10929-122">detectionType</span></span>|[<span data-ttu-id="10929-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="10929-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="10929-124">Тип обнаружения данных реестра.</span><span class="sxs-lookup"><span data-stu-id="10929-124">The registry data detection type.</span></span> <span data-ttu-id="10929-125">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="10929-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="10929-126">operator</span><span class="sxs-lookup"><span data-stu-id="10929-126">operator</span></span>|[<span data-ttu-id="10929-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="10929-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="10929-128">Оператор для обнаружения данных реестра.</span><span class="sxs-lookup"><span data-stu-id="10929-128">The operator for registry data detection.</span></span> <span data-ttu-id="10929-129">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="10929-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="10929-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="10929-130">detectionValue</span></span>|<span data-ttu-id="10929-131">String.</span><span class="sxs-lookup"><span data-stu-id="10929-131">String</span></span>|<span data-ttu-id="10929-132">Определение значения реестра</span><span class="sxs-lookup"><span data-stu-id="10929-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="10929-133">Связи</span><span class="sxs-lookup"><span data-stu-id="10929-133">Relationships</span></span>
<span data-ttu-id="10929-134">Нет</span><span class="sxs-lookup"><span data-stu-id="10929-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="10929-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10929-135">JSON Representation</span></span>
<span data-ttu-id="10929-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10929-136">Here is a JSON representation of the resource.</span></span>
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





