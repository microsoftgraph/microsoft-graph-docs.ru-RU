---
title: Тип ресурса win32LobAppFileSystemRequirement
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab011739ed24a0f9880ccc72461f0c4eef5c0655
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708979"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="a6681-103">Тип ресурса win32LobAppFileSystemRequirement</span><span class="sxs-lookup"><span data-stu-id="a6681-103">win32LobAppFileSystemRequirement resource type</span></span>

<span data-ttu-id="a6681-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6681-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6681-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6681-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6681-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a6681-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6681-107">Содержит путь к файлу или папке для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="a6681-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="a6681-108">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="a6681-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a6681-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6681-109">Properties</span></span>
|<span data-ttu-id="a6681-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6681-110">Property</span></span>|<span data-ttu-id="a6681-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a6681-111">Type</span></span>|<span data-ttu-id="a6681-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a6681-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6681-113">operator</span><span class="sxs-lookup"><span data-stu-id="a6681-113">operator</span></span>|[<span data-ttu-id="a6681-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="a6681-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="a6681-115">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="a6681-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="a6681-116">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="a6681-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="a6681-117">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="a6681-117">detectionValue</span></span>|<span data-ttu-id="a6681-118">Строка</span><span class="sxs-lookup"><span data-stu-id="a6681-118">String</span></span>|<span data-ttu-id="a6681-119">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="a6681-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="a6681-120">path</span><span class="sxs-lookup"><span data-stu-id="a6681-120">path</span></span>|<span data-ttu-id="a6681-121">String</span><span class="sxs-lookup"><span data-stu-id="a6681-121">String</span></span>|<span data-ttu-id="a6681-122">Путь к файлу или папке для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="a6681-122">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="a6681-123">филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="a6681-123">fileOrFolderName</span></span>|<span data-ttu-id="a6681-124">Строка</span><span class="sxs-lookup"><span data-stu-id="a6681-124">String</span></span>|<span data-ttu-id="a6681-125">Имя файла или папки для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="a6681-125">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="a6681-126">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="a6681-126">check32BitOn64System</span></span>|<span data-ttu-id="a6681-127">Логический</span><span class="sxs-lookup"><span data-stu-id="a6681-127">Boolean</span></span>|<span data-ttu-id="a6681-128">Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="a6681-128">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="a6681-129">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="a6681-129">detectionType</span></span>|[<span data-ttu-id="a6681-130">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="a6681-130">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="a6681-131">Тип обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="a6681-131">The file system detection type.</span></span> <span data-ttu-id="a6681-132">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="a6681-132">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6681-133">Связи</span><span class="sxs-lookup"><span data-stu-id="a6681-133">Relationships</span></span>
<span data-ttu-id="a6681-134">Нет</span><span class="sxs-lookup"><span data-stu-id="a6681-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6681-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6681-135">JSON Representation</span></span>
<span data-ttu-id="a6681-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6681-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemRequirement",
  "operator": "String",
  "detectionValue": "String",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String"
}
```





