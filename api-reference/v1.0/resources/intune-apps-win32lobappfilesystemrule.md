---
title: тип ресурса win32LobAppFileSystemRule
description: Сложный тип для хранения данных правил файлов или папок для приложения LOB Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a0c8a45a9f3d49c671949a2b5ad3b9bd549ee8d7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752401"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="913ea-103">тип ресурса win32LobAppFileSystemRule</span><span class="sxs-lookup"><span data-stu-id="913ea-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="913ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="913ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="913ea-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="913ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="913ea-106">Сложный тип для хранения данных правил файлов или папок для приложения LOB Win32.</span><span class="sxs-lookup"><span data-stu-id="913ea-106">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="913ea-107">Наследует [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="913ea-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="913ea-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="913ea-108">Properties</span></span>
|<span data-ttu-id="913ea-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="913ea-109">Property</span></span>|<span data-ttu-id="913ea-110">Тип</span><span class="sxs-lookup"><span data-stu-id="913ea-110">Type</span></span>|<span data-ttu-id="913ea-111">Описание</span><span class="sxs-lookup"><span data-stu-id="913ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="913ea-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="913ea-112">ruleType</span></span>|[<span data-ttu-id="913ea-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="913ea-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="913ea-114">Тип правила, указывающий цель правила.</span><span class="sxs-lookup"><span data-stu-id="913ea-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="913ea-115">Унаследованный от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="913ea-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="913ea-116">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="913ea-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="913ea-117">path</span><span class="sxs-lookup"><span data-stu-id="913ea-117">path</span></span>|<span data-ttu-id="913ea-118">String</span><span class="sxs-lookup"><span data-stu-id="913ea-118">String</span></span>|<span data-ttu-id="913ea-119">Путь к файлу или папке.</span><span class="sxs-lookup"><span data-stu-id="913ea-119">The file or folder path to look up.</span></span>|
|<span data-ttu-id="913ea-120">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="913ea-120">fileOrFolderName</span></span>|<span data-ttu-id="913ea-121">String</span><span class="sxs-lookup"><span data-stu-id="913ea-121">String</span></span>|<span data-ttu-id="913ea-122">Имя файла или папки.</span><span class="sxs-lookup"><span data-stu-id="913ea-122">The file or folder name to look up.</span></span>|
|<span data-ttu-id="913ea-123">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="913ea-123">check32BitOn64System</span></span>|<span data-ttu-id="913ea-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="913ea-124">Boolean</span></span>|<span data-ttu-id="913ea-125">Значение, указывающее, следует ли расширять переменные среды в 32-битной среде на 64-битных системах.</span><span class="sxs-lookup"><span data-stu-id="913ea-125">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="913ea-126">operationType</span><span class="sxs-lookup"><span data-stu-id="913ea-126">operationType</span></span>|[<span data-ttu-id="913ea-127">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="913ea-127">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="913ea-128">Тип операции файловой системы.</span><span class="sxs-lookup"><span data-stu-id="913ea-128">The file system operation type.</span></span> <span data-ttu-id="913ea-129">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="913ea-129">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="913ea-130">operator</span><span class="sxs-lookup"><span data-stu-id="913ea-130">operator</span></span>|[<span data-ttu-id="913ea-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="913ea-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="913ea-132">Оператор обнаружения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="913ea-132">The operator for file or folder detection.</span></span> <span data-ttu-id="913ea-133">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="913ea-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="913ea-134">comparisonValue</span><span class="sxs-lookup"><span data-stu-id="913ea-134">comparisonValue</span></span>|<span data-ttu-id="913ea-135">String</span><span class="sxs-lookup"><span data-stu-id="913ea-135">String</span></span>|<span data-ttu-id="913ea-136">Значение сравнения файла или папки.</span><span class="sxs-lookup"><span data-stu-id="913ea-136">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="913ea-137">Отношения</span><span class="sxs-lookup"><span data-stu-id="913ea-137">Relationships</span></span>
<span data-ttu-id="913ea-138">Нет</span><span class="sxs-lookup"><span data-stu-id="913ea-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="913ea-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="913ea-139">JSON Representation</span></span>
<span data-ttu-id="913ea-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="913ea-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRule",
  "ruleType": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "operationType": "String",
  "operator": "String",
  "comparisonValue": "String"
}
```




