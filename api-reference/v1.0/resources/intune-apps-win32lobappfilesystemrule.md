---
title: Тип ресурса win32LobAppFileSystemRule
description: Сложный тип для хранения данных правила для файлов или папок для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e3873b85256f1c79c0102e1f410619d98c51594
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080174"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="b3833-103">Тип ресурса win32LobAppFileSystemRule</span><span class="sxs-lookup"><span data-stu-id="b3833-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="b3833-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3833-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3833-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3833-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3833-106">Сложный тип для хранения данных правила для файлов или папок для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="b3833-106">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="b3833-107">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="b3833-107">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3833-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3833-108">Properties</span></span>
|<span data-ttu-id="b3833-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3833-109">Property</span></span>|<span data-ttu-id="b3833-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b3833-110">Type</span></span>|<span data-ttu-id="b3833-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b3833-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3833-112">ruleType</span><span class="sxs-lookup"><span data-stu-id="b3833-112">ruleType</span></span>|[<span data-ttu-id="b3833-113">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="b3833-113">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="b3833-114">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="b3833-114">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="b3833-115">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="b3833-115">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="b3833-116">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="b3833-116">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="b3833-117">path</span><span class="sxs-lookup"><span data-stu-id="b3833-117">path</span></span>|<span data-ttu-id="b3833-118">String</span><span class="sxs-lookup"><span data-stu-id="b3833-118">String</span></span>|<span data-ttu-id="b3833-119">Путь к файлу или папке для поиска.</span><span class="sxs-lookup"><span data-stu-id="b3833-119">The file or folder path to look up.</span></span>|
|<span data-ttu-id="b3833-120">филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="b3833-120">fileOrFolderName</span></span>|<span data-ttu-id="b3833-121">Строка</span><span class="sxs-lookup"><span data-stu-id="b3833-121">String</span></span>|<span data-ttu-id="b3833-122">Имя файла или папки для поиска.</span><span class="sxs-lookup"><span data-stu-id="b3833-122">The file or folder name to look up.</span></span>|
|<span data-ttu-id="b3833-123">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="b3833-123">check32BitOn64System</span></span>|<span data-ttu-id="b3833-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3833-124">Boolean</span></span>|<span data-ttu-id="b3833-125">Значение, указывающее, следует ли развертывать переменные среды в 32 – разрядном контексте в 64 – разрядных системах.</span><span class="sxs-lookup"><span data-stu-id="b3833-125">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="b3833-126">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="b3833-126">operationType</span></span>|[<span data-ttu-id="b3833-127">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="b3833-127">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="b3833-128">Тип операции файловой системы.</span><span class="sxs-lookup"><span data-stu-id="b3833-128">The file system operation type.</span></span> <span data-ttu-id="b3833-129">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="b3833-129">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="b3833-130">operator</span><span class="sxs-lookup"><span data-stu-id="b3833-130">operator</span></span>|[<span data-ttu-id="b3833-131">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="b3833-131">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="b3833-132">Оператор для обнаружения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="b3833-132">The operator for file or folder detection.</span></span> <span data-ttu-id="b3833-133">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="b3833-133">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="b3833-134">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="b3833-134">comparisonValue</span></span>|<span data-ttu-id="b3833-135">Строка</span><span class="sxs-lookup"><span data-stu-id="b3833-135">String</span></span>|<span data-ttu-id="b3833-136">Значение сравнения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="b3833-136">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3833-137">Связи</span><span class="sxs-lookup"><span data-stu-id="b3833-137">Relationships</span></span>
<span data-ttu-id="b3833-138">Нет</span><span class="sxs-lookup"><span data-stu-id="b3833-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3833-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3833-139">JSON Representation</span></span>
<span data-ttu-id="b3833-140">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3833-140">Here is a JSON representation of the resource.</span></span>
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





