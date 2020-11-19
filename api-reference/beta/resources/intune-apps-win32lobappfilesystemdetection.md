---
title: Тип ресурса win32LobAppFileSystemDetection
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c3d4d3ef791b4e0056ae0410c1e576a313af0f3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217096"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="c22c1-103">Тип ресурса win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="c22c1-103">win32LobAppFileSystemDetection resource type</span></span>

<span data-ttu-id="c22c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c22c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c22c1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c22c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c22c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c22c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c22c1-107">Содержит путь к файлу или папке для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="c22c1-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="c22c1-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="c22c1-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c22c1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c22c1-109">Properties</span></span>
|<span data-ttu-id="c22c1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c22c1-110">Property</span></span>|<span data-ttu-id="c22c1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c22c1-111">Type</span></span>|<span data-ttu-id="c22c1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c22c1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c22c1-113">path</span><span class="sxs-lookup"><span data-stu-id="c22c1-113">path</span></span>|<span data-ttu-id="c22c1-114">String</span><span class="sxs-lookup"><span data-stu-id="c22c1-114">String</span></span>|<span data-ttu-id="c22c1-115">Путь к файлу или папке для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="c22c1-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="c22c1-116">филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="c22c1-116">fileOrFolderName</span></span>|<span data-ttu-id="c22c1-117">String</span><span class="sxs-lookup"><span data-stu-id="c22c1-117">String</span></span>|<span data-ttu-id="c22c1-118">Имя файла или папки для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="c22c1-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="c22c1-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="c22c1-119">check32BitOn64System</span></span>|<span data-ttu-id="c22c1-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="c22c1-120">Boolean</span></span>|<span data-ttu-id="c22c1-121">Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="c22c1-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="c22c1-122">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="c22c1-122">detectionType</span></span>|[<span data-ttu-id="c22c1-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="c22c1-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="c22c1-124">Тип обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="c22c1-124">The file system detection type.</span></span> <span data-ttu-id="c22c1-125">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="c22c1-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="c22c1-126">operator</span><span class="sxs-lookup"><span data-stu-id="c22c1-126">operator</span></span>|[<span data-ttu-id="c22c1-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="c22c1-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="c22c1-128">Оператор для обнаружения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="c22c1-128">The operator for file or folder detection.</span></span> <span data-ttu-id="c22c1-129">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="c22c1-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="c22c1-130">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="c22c1-130">detectionValue</span></span>|<span data-ttu-id="c22c1-131">String</span><span class="sxs-lookup"><span data-stu-id="c22c1-131">String</span></span>|<span data-ttu-id="c22c1-132">Значение обнаружения файлов или папок</span><span class="sxs-lookup"><span data-stu-id="c22c1-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="c22c1-133">Связи</span><span class="sxs-lookup"><span data-stu-id="c22c1-133">Relationships</span></span>
<span data-ttu-id="c22c1-134">Нет</span><span class="sxs-lookup"><span data-stu-id="c22c1-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c22c1-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c22c1-135">JSON Representation</span></span>
<span data-ttu-id="c22c1-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c22c1-136">Here is a JSON representation of the resource.</span></span>
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




