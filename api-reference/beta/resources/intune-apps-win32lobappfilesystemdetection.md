---
title: Тип ресурса win32LobAppFileSystemDetection
description: Содержит путь файла или папки для обнаружения приложений Win32
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5fb4e66ce17fb7a964f3210244e2f3a7027c578
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415231"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="8cb0b-103">Тип ресурса win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="8cb0b-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="8cb0b-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="8cb0b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8cb0b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cb0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cb0b-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8cb0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cb0b-107">Содержит путь файла или папки для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="8cb0b-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="8cb0b-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="8cb0b-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8cb0b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8cb0b-109">Properties</span></span>
|<span data-ttu-id="8cb0b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8cb0b-110">Property</span></span>|<span data-ttu-id="8cb0b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8cb0b-111">Type</span></span>|<span data-ttu-id="8cb0b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8cb0b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb0b-113">path</span><span class="sxs-lookup"><span data-stu-id="8cb0b-113">path</span></span>|<span data-ttu-id="8cb0b-114">String</span><span class="sxs-lookup"><span data-stu-id="8cb0b-114">String</span></span>|<span data-ttu-id="8cb0b-115">Путь файла или папки для обнаружения Win32 строки из бизнес-приложения</span><span class="sxs-lookup"><span data-stu-id="8cb0b-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="8cb0b-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="8cb0b-116">fileOrFolderName</span></span>|<span data-ttu-id="8cb0b-117">String</span><span class="sxs-lookup"><span data-stu-id="8cb0b-117">String</span></span>|<span data-ttu-id="8cb0b-118">Имя файла или папки для обнаружения Win32 строки из бизнес-приложения</span><span class="sxs-lookup"><span data-stu-id="8cb0b-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="8cb0b-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="8cb0b-119">check32BitOn64System</span></span>|<span data-ttu-id="8cb0b-120">Логический</span><span class="sxs-lookup"><span data-stu-id="8cb0b-120">Boolean</span></span>|<span data-ttu-id="8cb0b-121">Значение, указывающее, является ли этот файл или папку для проверки 32-разрядная версия приложения на 64-разрядных систем</span><span class="sxs-lookup"><span data-stu-id="8cb0b-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="8cb0b-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="8cb0b-122">detectionType</span></span>|[<span data-ttu-id="8cb0b-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="8cb0b-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="8cb0b-124">Обнаружение тип файловой системы.</span><span class="sxs-lookup"><span data-stu-id="8cb0b-124">The file system detection type.</span></span> <span data-ttu-id="8cb0b-125">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="8cb0b-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="8cb0b-126">operator</span><span class="sxs-lookup"><span data-stu-id="8cb0b-126">operator</span></span>|[<span data-ttu-id="8cb0b-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="8cb0b-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="8cb0b-128">Оператор для обнаружения файла или fodler.</span><span class="sxs-lookup"><span data-stu-id="8cb0b-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="8cb0b-129">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="8cb0b-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="8cb0b-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="8cb0b-130">detectionValue</span></span>|<span data-ttu-id="8cb0b-131">String</span><span class="sxs-lookup"><span data-stu-id="8cb0b-131">String</span></span>|<span data-ttu-id="8cb0b-132">Значение обнаружения файла или папки</span><span class="sxs-lookup"><span data-stu-id="8cb0b-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cb0b-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="8cb0b-133">Relationships</span></span>
<span data-ttu-id="8cb0b-134">Нет</span><span class="sxs-lookup"><span data-stu-id="8cb0b-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cb0b-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8cb0b-135">JSON Representation</span></span>
<span data-ttu-id="8cb0b-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8cb0b-136">Here is a JSON representation of the resource.</span></span>
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




