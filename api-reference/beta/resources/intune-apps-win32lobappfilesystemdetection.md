---
title: Тип ресурса win32LobAppFileSystemDetection
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da95d263af1bf2e217ab5468659b17eed2cb3f8c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797656"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="8df61-103">Тип ресурса win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="8df61-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="8df61-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8df61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8df61-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8df61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8df61-106">Содержит путь к файлу или папке для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="8df61-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="8df61-107">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="8df61-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8df61-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8df61-108">Properties</span></span>
|<span data-ttu-id="8df61-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8df61-109">Property</span></span>|<span data-ttu-id="8df61-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8df61-110">Type</span></span>|<span data-ttu-id="8df61-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8df61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8df61-112">path</span><span class="sxs-lookup"><span data-stu-id="8df61-112">path</span></span>|<span data-ttu-id="8df61-113">String</span><span class="sxs-lookup"><span data-stu-id="8df61-113">String</span></span>|<span data-ttu-id="8df61-114">Путь к файлу или папке для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="8df61-114">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="8df61-115">филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="8df61-115">fileOrFolderName</span></span>|<span data-ttu-id="8df61-116">String</span><span class="sxs-lookup"><span data-stu-id="8df61-116">String</span></span>|<span data-ttu-id="8df61-117">Имя файла или папки для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="8df61-117">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="8df61-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="8df61-118">check32BitOn64System</span></span>|<span data-ttu-id="8df61-119">Логический</span><span class="sxs-lookup"><span data-stu-id="8df61-119">Boolean</span></span>|<span data-ttu-id="8df61-120">Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="8df61-120">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="8df61-121">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="8df61-121">detectionType</span></span>|[<span data-ttu-id="8df61-122">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="8df61-122">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="8df61-123">Тип обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="8df61-123">The file system detection type.</span></span> <span data-ttu-id="8df61-124">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="8df61-124">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="8df61-125">operator</span><span class="sxs-lookup"><span data-stu-id="8df61-125">operator</span></span>|[<span data-ttu-id="8df61-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="8df61-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="8df61-127">Оператор для обнаружения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="8df61-127">The operator for file or folder detection.</span></span> <span data-ttu-id="8df61-128">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="8df61-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="8df61-129">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="8df61-129">detectionValue</span></span>|<span data-ttu-id="8df61-130">String</span><span class="sxs-lookup"><span data-stu-id="8df61-130">String</span></span>|<span data-ttu-id="8df61-131">Значение обнаружения файлов или папок</span><span class="sxs-lookup"><span data-stu-id="8df61-131">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8df61-132">Связи</span><span class="sxs-lookup"><span data-stu-id="8df61-132">Relationships</span></span>
<span data-ttu-id="8df61-133">Нет</span><span class="sxs-lookup"><span data-stu-id="8df61-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8df61-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8df61-134">JSON Representation</span></span>
<span data-ttu-id="8df61-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8df61-135">Here is a JSON representation of the resource.</span></span>
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



