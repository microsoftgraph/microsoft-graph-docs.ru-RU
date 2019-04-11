---
title: Тип ресурса win32LobAppFileSystemDetection
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e899a9caa5e4f21292ec56c5595bc77d3b68bcc2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803250"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="6a7ef-103">Тип ресурса win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="6a7ef-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="6a7ef-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a7ef-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a7ef-106">Содержит путь к файлу или папке для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="6a7ef-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="6a7ef-107">НаСледуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="6a7ef-107">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6a7ef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a7ef-108">Properties</span></span>
|<span data-ttu-id="6a7ef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a7ef-109">Property</span></span>|<span data-ttu-id="6a7ef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6a7ef-110">Type</span></span>|<span data-ttu-id="6a7ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a7ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a7ef-112">path</span><span class="sxs-lookup"><span data-stu-id="6a7ef-112">path</span></span>|<span data-ttu-id="6a7ef-113">String</span><span class="sxs-lookup"><span data-stu-id="6a7ef-113">String</span></span>|<span data-ttu-id="6a7ef-114">Путь к файлу или папке для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="6a7ef-114">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="6a7ef-115">Филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="6a7ef-115">fileOrFolderName</span></span>|<span data-ttu-id="6a7ef-116">String</span><span class="sxs-lookup"><span data-stu-id="6a7ef-116">String</span></span>|<span data-ttu-id="6a7ef-117">Имя файла или папки для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="6a7ef-117">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="6a7ef-118">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="6a7ef-118">check32BitOn64System</span></span>|<span data-ttu-id="6a7ef-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a7ef-119">Boolean</span></span>|<span data-ttu-id="6a7ef-120">Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="6a7ef-120">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="6a7ef-121">Детектионтипе</span><span class="sxs-lookup"><span data-stu-id="6a7ef-121">detectionType</span></span>|[<span data-ttu-id="6a7ef-122">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="6a7ef-122">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="6a7ef-123">Тип обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-123">The file system detection type.</span></span> <span data-ttu-id="6a7ef-124">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-124">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|
|<span data-ttu-id="6a7ef-125">operator</span><span class="sxs-lookup"><span data-stu-id="6a7ef-125">operator</span></span>|[<span data-ttu-id="6a7ef-126">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="6a7ef-126">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="6a7ef-127">Оператор для обнаружения файлов или папок.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-127">The operator for file or folder detection.</span></span> <span data-ttu-id="6a7ef-128">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-128">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="6a7ef-129">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="6a7ef-129">detectionValue</span></span>|<span data-ttu-id="6a7ef-130">String</span><span class="sxs-lookup"><span data-stu-id="6a7ef-130">String</span></span>|<span data-ttu-id="6a7ef-131">Значение обнаружения файлов или папок</span><span class="sxs-lookup"><span data-stu-id="6a7ef-131">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a7ef-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="6a7ef-132">Relationships</span></span>
<span data-ttu-id="6a7ef-133">Нет</span><span class="sxs-lookup"><span data-stu-id="6a7ef-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a7ef-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a7ef-134">JSON Representation</span></span>
<span data-ttu-id="6a7ef-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a7ef-135">Here is a JSON representation of the resource.</span></span>
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





