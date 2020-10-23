---
title: Тип ресурса win32LobAppRegistryRequirement
description: Содержит свойства реестра для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 175896a3b086821e4c36a26b5644d08e503d019d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706221"
---
# <a name="win32lobappregistryrequirement-resource-type"></a><span data-ttu-id="ec49c-103">Тип ресурса win32LobAppRegistryRequirement</span><span class="sxs-lookup"><span data-stu-id="ec49c-103">win32LobAppRegistryRequirement resource type</span></span>

<span data-ttu-id="ec49c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec49c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec49c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ec49c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec49c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ec49c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec49c-107">Содержит свойства реестра для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="ec49c-107">Contains registry properties to detect a Win32 App</span></span>


<span data-ttu-id="ec49c-108">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="ec49c-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec49c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="ec49c-109">Properties</span></span>
|<span data-ttu-id="ec49c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="ec49c-110">Property</span></span>|<span data-ttu-id="ec49c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="ec49c-111">Type</span></span>|<span data-ttu-id="ec49c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="ec49c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec49c-113">operator</span><span class="sxs-lookup"><span data-stu-id="ec49c-113">operator</span></span>|[<span data-ttu-id="ec49c-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="ec49c-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="ec49c-115">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="ec49c-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="ec49c-116">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="ec49c-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="ec49c-117">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="ec49c-117">detectionValue</span></span>|<span data-ttu-id="ec49c-118">Строка</span><span class="sxs-lookup"><span data-stu-id="ec49c-118">String</span></span>|<span data-ttu-id="ec49c-119">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="ec49c-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="ec49c-120">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="ec49c-120">check32BitOn64System</span></span>|<span data-ttu-id="ec49c-121">Логический</span><span class="sxs-lookup"><span data-stu-id="ec49c-121">Boolean</span></span>|<span data-ttu-id="ec49c-122">Значение, указывающее, является ли этот путь реестра для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="ec49c-122">A value indicating whether this registry path is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="ec49c-123">Ключевой</span><span class="sxs-lookup"><span data-stu-id="ec49c-123">keyPath</span></span>|<span data-ttu-id="ec49c-124">Строка</span><span class="sxs-lookup"><span data-stu-id="ec49c-124">String</span></span>|<span data-ttu-id="ec49c-125">Путь к разделу реестра для определения бизнес-приложения Win32 (LoB)</span><span class="sxs-lookup"><span data-stu-id="ec49c-125">The registry key path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="ec49c-126">valueName</span><span class="sxs-lookup"><span data-stu-id="ec49c-126">valueName</span></span>|<span data-ttu-id="ec49c-127">Строка</span><span class="sxs-lookup"><span data-stu-id="ec49c-127">String</span></span>|<span data-ttu-id="ec49c-128">Имя значения реестра</span><span class="sxs-lookup"><span data-stu-id="ec49c-128">The registry value name</span></span>|
|<span data-ttu-id="ec49c-129">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="ec49c-129">detectionType</span></span>|[<span data-ttu-id="ec49c-130">win32LobAppRegistryDetectionType</span><span class="sxs-lookup"><span data-stu-id="ec49c-130">win32LobAppRegistryDetectionType</span></span>](../resources/intune-apps-win32lobappregistrydetectiontype.md)|<span data-ttu-id="ec49c-131">Тип обнаружения данных в реестре.</span><span class="sxs-lookup"><span data-stu-id="ec49c-131">The registry data detection type.</span></span> <span data-ttu-id="ec49c-132">Возможные значения: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span><span class="sxs-lookup"><span data-stu-id="ec49c-132">Possible values are: `notConfigured`, `exists`, `doesNotExist`, `string`, `integer`, `version`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec49c-133">Связи</span><span class="sxs-lookup"><span data-stu-id="ec49c-133">Relationships</span></span>
<span data-ttu-id="ec49c-134">Нет</span><span class="sxs-lookup"><span data-stu-id="ec49c-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec49c-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ec49c-135">JSON Representation</span></span>
<span data-ttu-id="ec49c-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ec49c-136">Here is a JSON representation of the resource.</span></span>
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





