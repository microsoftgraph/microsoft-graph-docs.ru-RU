---
title: Тип ресурса win32LobAppFileSystemRule
description: Сложный тип для хранения данных правила для файлов или папок для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fa01642dd36cd8dc79f713446df05a9559294f56
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790833"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="63805-103">Тип ресурса win32LobAppFileSystemRule</span><span class="sxs-lookup"><span data-stu-id="63805-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="63805-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63805-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="63805-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="63805-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63805-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="63805-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63805-107">Сложный тип для хранения данных правила для файлов или папок для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="63805-107">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="63805-108">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="63805-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63805-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="63805-109">Properties</span></span>
|<span data-ttu-id="63805-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="63805-110">Property</span></span>|<span data-ttu-id="63805-111">Тип</span><span class="sxs-lookup"><span data-stu-id="63805-111">Type</span></span>|<span data-ttu-id="63805-112">Описание</span><span class="sxs-lookup"><span data-stu-id="63805-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63805-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="63805-113">ruleType</span></span>|[<span data-ttu-id="63805-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="63805-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="63805-115">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="63805-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="63805-116">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="63805-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="63805-117">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="63805-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="63805-118">path</span><span class="sxs-lookup"><span data-stu-id="63805-118">path</span></span>|<span data-ttu-id="63805-119">String</span><span class="sxs-lookup"><span data-stu-id="63805-119">String</span></span>|<span data-ttu-id="63805-120">Путь к файлу или папке для поиска.</span><span class="sxs-lookup"><span data-stu-id="63805-120">The file or folder path to look up.</span></span>|
|<span data-ttu-id="63805-121">филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="63805-121">fileOrFolderName</span></span>|<span data-ttu-id="63805-122">String</span><span class="sxs-lookup"><span data-stu-id="63805-122">String</span></span>|<span data-ttu-id="63805-123">Имя файла или папки для поиска.</span><span class="sxs-lookup"><span data-stu-id="63805-123">The file or folder name to look up.</span></span>|
|<span data-ttu-id="63805-124">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="63805-124">check32BitOn64System</span></span>|<span data-ttu-id="63805-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="63805-125">Boolean</span></span>|<span data-ttu-id="63805-126">Значение, указывающее, следует ли развертывать переменные среды в 32 – разрядном контексте в 64 – разрядных системах.</span><span class="sxs-lookup"><span data-stu-id="63805-126">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="63805-127">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="63805-127">operationType</span></span>|[<span data-ttu-id="63805-128">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="63805-128">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="63805-129">Тип операции файловой системы.</span><span class="sxs-lookup"><span data-stu-id="63805-129">The file system operation type.</span></span> <span data-ttu-id="63805-130">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="63805-130">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="63805-131">operator</span><span class="sxs-lookup"><span data-stu-id="63805-131">operator</span></span>|[<span data-ttu-id="63805-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="63805-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="63805-133">Оператор для обнаружения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="63805-133">The operator for file or folder detection.</span></span> <span data-ttu-id="63805-134">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="63805-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="63805-135">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="63805-135">comparisonValue</span></span>|<span data-ttu-id="63805-136">String</span><span class="sxs-lookup"><span data-stu-id="63805-136">String</span></span>|<span data-ttu-id="63805-137">Значение сравнения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="63805-137">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63805-138">Связи</span><span class="sxs-lookup"><span data-stu-id="63805-138">Relationships</span></span>
<span data-ttu-id="63805-139">Нет</span><span class="sxs-lookup"><span data-stu-id="63805-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63805-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="63805-140">JSON Representation</span></span>
<span data-ttu-id="63805-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63805-141">Here is a JSON representation of the resource.</span></span>
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



