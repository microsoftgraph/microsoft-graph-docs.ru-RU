---
title: Тип ресурса win32LobAppFileSystemDetection
description: Содержит путь файла или папки для обнаружения приложений Win32
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c901949295b1ff411dec5e9827b7991c922c2315
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958210"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a><span data-ttu-id="55450-103">Тип ресурса win32LobAppFileSystemDetection</span><span class="sxs-lookup"><span data-stu-id="55450-103">win32LobAppFileSystemDetection resource type</span></span>

> <span data-ttu-id="55450-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="55450-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55450-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55450-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="55450-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="55450-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55450-107">Содержит путь файла или папки для обнаружения приложений Win32</span><span class="sxs-lookup"><span data-stu-id="55450-107">Contains file or folder path to detect a Win32 App</span></span>

<span data-ttu-id="55450-108">Наследуется от [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span><span class="sxs-lookup"><span data-stu-id="55450-108">Inherits from [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)</span></span>

## <a name="properties"></a><span data-ttu-id="55450-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="55450-109">Properties</span></span>
|<span data-ttu-id="55450-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="55450-110">Property</span></span>|<span data-ttu-id="55450-111">Тип</span><span class="sxs-lookup"><span data-stu-id="55450-111">Type</span></span>|<span data-ttu-id="55450-112">Описание</span><span class="sxs-lookup"><span data-stu-id="55450-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55450-113">path</span><span class="sxs-lookup"><span data-stu-id="55450-113">path</span></span>|<span data-ttu-id="55450-114">String</span><span class="sxs-lookup"><span data-stu-id="55450-114">String</span></span>|<span data-ttu-id="55450-115">Путь файла или папки для обнаружения Win32 строки из бизнес-приложения</span><span class="sxs-lookup"><span data-stu-id="55450-115">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="55450-116">fileOrFolderName</span><span class="sxs-lookup"><span data-stu-id="55450-116">fileOrFolderName</span></span>|<span data-ttu-id="55450-117">Строка</span><span class="sxs-lookup"><span data-stu-id="55450-117">String</span></span>|<span data-ttu-id="55450-118">Имя файла или папки для обнаружения Win32 строки из бизнес-приложения</span><span class="sxs-lookup"><span data-stu-id="55450-118">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="55450-119">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="55450-119">check32BitOn64System</span></span>|<span data-ttu-id="55450-120">Логический</span><span class="sxs-lookup"><span data-stu-id="55450-120">Boolean</span></span>|<span data-ttu-id="55450-121">Значение, указывающее, является ли этот файл или папку для проверки 32-разрядная версия приложения на 64-разрядных систем</span><span class="sxs-lookup"><span data-stu-id="55450-121">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="55450-122">detectionType</span><span class="sxs-lookup"><span data-stu-id="55450-122">detectionType</span></span>|[<span data-ttu-id="55450-123">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="55450-123">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="55450-124">Обнаружение тип файловой системы.</span><span class="sxs-lookup"><span data-stu-id="55450-124">The file system detection type.</span></span> <span data-ttu-id="55450-125">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span><span class="sxs-lookup"><span data-stu-id="55450-125">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`.</span></span>|
|<span data-ttu-id="55450-126">operator</span><span class="sxs-lookup"><span data-stu-id="55450-126">operator</span></span>|[<span data-ttu-id="55450-127">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="55450-127">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="55450-128">Оператор для обнаружения файла или fodler.</span><span class="sxs-lookup"><span data-stu-id="55450-128">The operator for file or fodler detection.</span></span> <span data-ttu-id="55450-129">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="55450-129">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="55450-130">detectionValue</span><span class="sxs-lookup"><span data-stu-id="55450-130">detectionValue</span></span>|<span data-ttu-id="55450-131">Строка</span><span class="sxs-lookup"><span data-stu-id="55450-131">String</span></span>|<span data-ttu-id="55450-132">Значение обнаружения файла или папки</span><span class="sxs-lookup"><span data-stu-id="55450-132">The file or folder detection value</span></span>|

## <a name="relationships"></a><span data-ttu-id="55450-133">Связи</span><span class="sxs-lookup"><span data-stu-id="55450-133">Relationships</span></span>
<span data-ttu-id="55450-134">Нет</span><span class="sxs-lookup"><span data-stu-id="55450-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55450-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55450-135">JSON Representation</span></span>
<span data-ttu-id="55450-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55450-136">Here is a JSON representation of the resource.</span></span>
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





