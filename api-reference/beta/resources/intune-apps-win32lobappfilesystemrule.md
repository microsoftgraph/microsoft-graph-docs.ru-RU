---
title: Тип ресурса win32LobAppFileSystemRule
description: Сложный тип для хранения данных правила для файлов или папок для бизнес-приложения Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c83fa4bf5f3d24a4b171a8492f4212720242acdf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033785"
---
# <a name="win32lobappfilesystemrule-resource-type"></a><span data-ttu-id="47afc-103">Тип ресурса win32LobAppFileSystemRule</span><span class="sxs-lookup"><span data-stu-id="47afc-103">win32LobAppFileSystemRule resource type</span></span>

<span data-ttu-id="47afc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47afc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47afc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47afc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47afc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="47afc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47afc-107">Сложный тип для хранения данных правила для файлов или папок для бизнес-приложения Win32.</span><span class="sxs-lookup"><span data-stu-id="47afc-107">A complex type to store file or folder rule data for a Win32 LOB app.</span></span>


<span data-ttu-id="47afc-108">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="47afc-108">Inherits from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span></span>

## <a name="properties"></a><span data-ttu-id="47afc-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="47afc-109">Properties</span></span>
|<span data-ttu-id="47afc-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="47afc-110">Property</span></span>|<span data-ttu-id="47afc-111">Тип</span><span class="sxs-lookup"><span data-stu-id="47afc-111">Type</span></span>|<span data-ttu-id="47afc-112">Описание</span><span class="sxs-lookup"><span data-stu-id="47afc-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47afc-113">ruleType</span><span class="sxs-lookup"><span data-stu-id="47afc-113">ruleType</span></span>|[<span data-ttu-id="47afc-114">win32LobAppRuleType</span><span class="sxs-lookup"><span data-stu-id="47afc-114">win32LobAppRuleType</span></span>](../resources/intune-apps-win32lobappruletype.md)|<span data-ttu-id="47afc-115">Тип правила, указывающий назначение правила.</span><span class="sxs-lookup"><span data-stu-id="47afc-115">The rule type indicating the purpose of the rule.</span></span> <span data-ttu-id="47afc-116">Наследуется от [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span><span class="sxs-lookup"><span data-stu-id="47afc-116">Inherited from [win32LobAppRule](../resources/intune-apps-win32lobapprule.md).</span></span> <span data-ttu-id="47afc-117">Возможные значения: `detection`, `requirement`.</span><span class="sxs-lookup"><span data-stu-id="47afc-117">Possible values are: `detection`, `requirement`.</span></span>|
|<span data-ttu-id="47afc-118">path</span><span class="sxs-lookup"><span data-stu-id="47afc-118">path</span></span>|<span data-ttu-id="47afc-119">String</span><span class="sxs-lookup"><span data-stu-id="47afc-119">String</span></span>|<span data-ttu-id="47afc-120">Путь к файлу или папке для поиска.</span><span class="sxs-lookup"><span data-stu-id="47afc-120">The file or folder path to look up.</span></span>|
|<span data-ttu-id="47afc-121">филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="47afc-121">fileOrFolderName</span></span>|<span data-ttu-id="47afc-122">String</span><span class="sxs-lookup"><span data-stu-id="47afc-122">String</span></span>|<span data-ttu-id="47afc-123">Имя файла или папки для поиска.</span><span class="sxs-lookup"><span data-stu-id="47afc-123">The file or folder name to look up.</span></span>|
|<span data-ttu-id="47afc-124">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="47afc-124">check32BitOn64System</span></span>|<span data-ttu-id="47afc-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="47afc-125">Boolean</span></span>|<span data-ttu-id="47afc-126">Значение, указывающее, следует ли развертывать переменные среды в 32 – разрядном контексте в 64 – разрядных системах.</span><span class="sxs-lookup"><span data-stu-id="47afc-126">A value indicating whether to expand environment variables in the 32-bit context on 64-bit systems.</span></span>|
|<span data-ttu-id="47afc-127">оператионтипе</span><span class="sxs-lookup"><span data-stu-id="47afc-127">operationType</span></span>|[<span data-ttu-id="47afc-128">win32LobAppFileSystemOperationType</span><span class="sxs-lookup"><span data-stu-id="47afc-128">win32LobAppFileSystemOperationType</span></span>](../resources/intune-apps-win32lobappfilesystemoperationtype.md)|<span data-ttu-id="47afc-129">Тип операции файловой системы.</span><span class="sxs-lookup"><span data-stu-id="47afc-129">The file system operation type.</span></span> <span data-ttu-id="47afc-130">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="47afc-130">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="47afc-131">operator</span><span class="sxs-lookup"><span data-stu-id="47afc-131">operator</span></span>|[<span data-ttu-id="47afc-132">win32LobAppRuleOperator</span><span class="sxs-lookup"><span data-stu-id="47afc-132">win32LobAppRuleOperator</span></span>](../resources/intune-apps-win32lobappruleoperator.md)|<span data-ttu-id="47afc-133">Оператор для обнаружения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="47afc-133">The operator for file or folder detection.</span></span> <span data-ttu-id="47afc-134">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="47afc-134">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="47afc-135">компарисонвалуе</span><span class="sxs-lookup"><span data-stu-id="47afc-135">comparisonValue</span></span>|<span data-ttu-id="47afc-136">String</span><span class="sxs-lookup"><span data-stu-id="47afc-136">String</span></span>|<span data-ttu-id="47afc-137">Значение сравнения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="47afc-137">The file or folder comparison value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47afc-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="47afc-138">Relationships</span></span>
<span data-ttu-id="47afc-139">Нет</span><span class="sxs-lookup"><span data-stu-id="47afc-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47afc-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="47afc-140">JSON Representation</span></span>
<span data-ttu-id="47afc-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="47afc-141">Here is a JSON representation of the resource.</span></span>
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






