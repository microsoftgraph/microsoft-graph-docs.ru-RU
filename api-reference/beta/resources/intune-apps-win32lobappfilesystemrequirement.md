---
title: Тип ресурса win32LobAppFileSystemRequirement
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: efd0a202d6db1711caa4c7341367d3d1afe85038
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809306"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="b35a8-103">Тип ресурса win32LobAppFileSystemRequirement</span><span class="sxs-lookup"><span data-stu-id="b35a8-103">win32LobAppFileSystemRequirement resource type</span></span>

> <span data-ttu-id="b35a8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b35a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b35a8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b35a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b35a8-106">Содержит путь к файлу или папке для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b35a8-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="b35a8-107">НаСледуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="b35a8-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b35a8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b35a8-108">Properties</span></span>
|<span data-ttu-id="b35a8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b35a8-109">Property</span></span>|<span data-ttu-id="b35a8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b35a8-110">Type</span></span>|<span data-ttu-id="b35a8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b35a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b35a8-112">operator</span><span class="sxs-lookup"><span data-stu-id="b35a8-112">operator</span></span>|[<span data-ttu-id="b35a8-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="b35a8-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="b35a8-114">Оператор обнаружения наСледуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="b35a8-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="b35a8-115">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="b35a8-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="b35a8-116">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="b35a8-116">detectionValue</span></span>|<span data-ttu-id="b35a8-117">String</span><span class="sxs-lookup"><span data-stu-id="b35a8-117">String</span></span>|<span data-ttu-id="b35a8-118">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="b35a8-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="b35a8-119">path</span><span class="sxs-lookup"><span data-stu-id="b35a8-119">path</span></span>|<span data-ttu-id="b35a8-120">String</span><span class="sxs-lookup"><span data-stu-id="b35a8-120">String</span></span>|<span data-ttu-id="b35a8-121">Путь к файлу или папке для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b35a8-121">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="b35a8-122">Филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="b35a8-122">fileOrFolderName</span></span>|<span data-ttu-id="b35a8-123">String</span><span class="sxs-lookup"><span data-stu-id="b35a8-123">String</span></span>|<span data-ttu-id="b35a8-124">Имя файла или папки для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="b35a8-124">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="b35a8-125">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="b35a8-125">check32BitOn64System</span></span>|<span data-ttu-id="b35a8-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="b35a8-126">Boolean</span></span>|<span data-ttu-id="b35a8-127">Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="b35a8-127">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="b35a8-128">Детектионтипе</span><span class="sxs-lookup"><span data-stu-id="b35a8-128">detectionType</span></span>|[<span data-ttu-id="b35a8-129">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="b35a8-129">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="b35a8-130">Тип обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="b35a8-130">The file system detection type.</span></span> <span data-ttu-id="b35a8-131">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="b35a8-131">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b35a8-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="b35a8-132">Relationships</span></span>
<span data-ttu-id="b35a8-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b35a8-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b35a8-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b35a8-134">JSON Representation</span></span>
<span data-ttu-id="b35a8-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b35a8-135">Here is a JSON representation of the resource.</span></span>
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





