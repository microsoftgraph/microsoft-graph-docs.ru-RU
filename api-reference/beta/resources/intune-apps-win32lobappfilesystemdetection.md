---
title: Тип ресурса win32LobAppFileSystemDetection
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c35fb1855c0aff33c12a84e9d78e7ec4ebd76a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012312"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="d220c-103">Тип ресурса win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="d220c-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="d220c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d220c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d220c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d220c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d220c-106">Содержит путь к файлу или папке для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="d220c-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="d220c-107">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="d220c-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d220c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d220c-108">Properties</span></span>
|<span data-ttu-id="d220c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d220c-109">Property</span></span>|<span data-ttu-id="d220c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d220c-110">Type</span></span>|<span data-ttu-id="d220c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d220c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d220c-112">path</span><span class="sxs-lookup"><span data-stu-id="d220c-112">path</span></span>|<span data-ttu-id="d220c-113">String</span><span class="sxs-lookup"><span data-stu-id="d220c-113">String</span></span>|<span data-ttu-id="d220c-114">Путь к файлу или папке для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="d220c-114">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="d220c-115">Филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="d220c-115">fileOrFolderName</span></span>|<span data-ttu-id="d220c-116">String</span><span class="sxs-lookup"><span data-stu-id="d220c-116">String</span></span>|<span data-ttu-id="d220c-117">Имя файла или папки для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="d220c-117">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="d220c-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="d220c-118">check32BitOn64System</span></span>|<span data-ttu-id="d220c-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d220c-119">Boolean</span></span>|<span data-ttu-id="d220c-120">Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="d220c-120">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="d220c-121">Детектионтипе</span><span class="sxs-lookup"><span data-stu-id="d220c-121">detectionType</span></span>|[<span data-ttu-id="d220c-122">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="d220c-122">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="d220c-123">Тип обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="d220c-123">The file system detection type.</span></span> <span data-ttu-id="d220c-124">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="d220c-124">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="d220c-125">operator</span><span class="sxs-lookup"><span data-stu-id="d220c-125">operator</span></span>|[<span data-ttu-id="d220c-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="d220c-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="d220c-127">Оператор для обнаружения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="d220c-127">The operator for file or folder detection.</span></span> <span data-ttu-id="d220c-128">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="d220c-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="d220c-129">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="d220c-129">detectionValue</span></span>|<span data-ttu-id="d220c-130">String</span><span class="sxs-lookup"><span data-stu-id="d220c-130">String</span></span>|<span data-ttu-id="d220c-131">Значение обнаружения файлов или папок</span><span class="sxs-lookup"><span data-stu-id="d220c-131">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="d220c-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="d220c-132">Relationships</span></span>
<span data-ttu-id="d220c-133">Нет</span><span class="sxs-lookup"><span data-stu-id="d220c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d220c-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d220c-134">JSON Representation</span></span>
<span data-ttu-id="d220c-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d220c-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```





