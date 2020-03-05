---
title: Тип ресурса win32LobAppRegistryDetection
description: Содержит свойства реестра для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da9f63d4a16df728320e0f3144bee32ad90f2922
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42490464"
---
# <a name="win32lobappregistrydetection-resource-type"></a><span data-ttu-id="60830-103">Тип ресурса win32LobAppRegistryDetection</span><span class="sxs-lookup"><span data-stu-id="60830-103">win32LobAppRegistryDetection resource type</span></span>

<span data-ttu-id="60830-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="60830-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60830-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="60830-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60830-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="60830-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60830-107">Содержит свойства реестра для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="60830-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="60830-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="60830-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="60830-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="60830-109">Properties</span></span>
|<span data-ttu-id="60830-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="60830-110">Property</span></span>|<span data-ttu-id="60830-111">Тип</span><span class="sxs-lookup"><span data-stu-id="60830-111">Type</span></span>|<span data-ttu-id="60830-112">Описание</span><span class="sxs-lookup"><span data-stu-id="60830-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60830-113">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="60830-113">check32BitOn64System</span></span>|<span data-ttu-id="60830-114">Логический</span><span class="sxs-lookup"><span data-stu-id="60830-114">Boolean</span></span>|<span data-ttu-id="60830-115">Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="60830-115">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="60830-116">Ключевой</span><span class="sxs-lookup"><span data-stu-id="60830-116">keyPath</span></span>|<span data-ttu-id="60830-117">String</span><span class="sxs-lookup"><span data-stu-id="60830-117">String</span></span>|<span data-ttu-id="60830-118">Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)</span><span class="sxs-lookup"><span data-stu-id="60830-118">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="60830-119">valueName</span><span class="sxs-lookup"><span data-stu-id="60830-119">valueName</span></span>|<span data-ttu-id="60830-120">String</span><span class="sxs-lookup"><span data-stu-id="60830-120">String</span></span>|<span data-ttu-id="60830-121">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="60830-121">The registry value name</span></span>|
|<span data-ttu-id="60830-122">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="60830-122">detectionType</span></span>|[<span data-ttu-id="60830-123">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="60830-123">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="60830-124">Тип обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="60830-124">The registry data detection type.</span></span> <span data-ttu-id="60830-125">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="60830-125">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|
|<span data-ttu-id="60830-126">operator</span><span class="sxs-lookup"><span data-stu-id="60830-126">operator</span></span>|[<span data-ttu-id="60830-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="60830-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="60830-128">Оператор для обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="60830-128">The operator for registry data detection.</span></span> <span data-ttu-id="60830-129">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="60830-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="60830-130">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="60830-130">detectionValue</span></span>|<span data-ttu-id="60830-131">String</span><span class="sxs-lookup"><span data-stu-id="60830-131">String</span></span>|<span data-ttu-id="60830-132">Значение обнаружения в реестре</span><span class="sxs-lookup"><span data-stu-id="60830-132">The registry detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="60830-133">Связи</span><span class="sxs-lookup"><span data-stu-id="60830-133">Relationships</span></span>
<span data-ttu-id="60830-134">Нет</span><span class="sxs-lookup"><span data-stu-id="60830-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60830-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="60830-135">JSON Representation</span></span>
<span data-ttu-id="60830-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60830-136">Here is a JSON representation of the resource.</span></span>
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



