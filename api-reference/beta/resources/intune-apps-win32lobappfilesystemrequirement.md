---
title: Тип ресурса win32LobAppFileSystemRequirement
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 19ffbebea879856af5a00a77ad4329320be3f78f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966627"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="c0a6d-103">Тип ресурса win32LobAppFileSystemRequirement</span><span class="sxs-lookup"><span data-stu-id="c0a6d-103">win32LobAppFileSystemRequirement resource type</span></span>

<span data-ttu-id="c0a6d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0a6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0a6d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0a6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0a6d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0a6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0a6d-107">Содержит путь к файлу или папке для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="c0a6d-107">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="c0a6d-108">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="c0a6d-108">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c0a6d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0a6d-109">Properties</span></span>
|<span data-ttu-id="c0a6d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0a6d-110">Property</span></span>|<span data-ttu-id="c0a6d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c0a6d-111">Type</span></span>|<span data-ttu-id="c0a6d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c0a6d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0a6d-113">operator</span><span class="sxs-lookup"><span data-stu-id="c0a6d-113">operator</span></span>|[<span data-ttu-id="c0a6d-114">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="c0a6d-114">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="c0a6d-115">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="c0a6d-115">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="c0a6d-116">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="c0a6d-116">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="c0a6d-117">детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="c0a6d-117">detectionValue</span></span>|<span data-ttu-id="c0a6d-118">String</span><span class="sxs-lookup"><span data-stu-id="c0a6d-118">String</span></span>|<span data-ttu-id="c0a6d-119">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="c0a6d-119">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="c0a6d-120">path</span><span class="sxs-lookup"><span data-stu-id="c0a6d-120">path</span></span>|<span data-ttu-id="c0a6d-121">String</span><span class="sxs-lookup"><span data-stu-id="c0a6d-121">String</span></span>|<span data-ttu-id="c0a6d-122">Путь к файлу или папке для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="c0a6d-122">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="c0a6d-123">филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="c0a6d-123">fileOrFolderName</span></span>|<span data-ttu-id="c0a6d-124">String</span><span class="sxs-lookup"><span data-stu-id="c0a6d-124">String</span></span>|<span data-ttu-id="c0a6d-125">Имя файла или папки для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="c0a6d-125">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="c0a6d-126">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="c0a6d-126">check32BitOn64System</span></span>|<span data-ttu-id="c0a6d-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0a6d-127">Boolean</span></span>|<span data-ttu-id="c0a6d-128">Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="c0a6d-128">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="c0a6d-129">детектионтипе</span><span class="sxs-lookup"><span data-stu-id="c0a6d-129">detectionType</span></span>|[<span data-ttu-id="c0a6d-130">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="c0a6d-130">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="c0a6d-131">Тип обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="c0a6d-131">The file system detection type.</span></span> <span data-ttu-id="c0a6d-132">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="c0a6d-132">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0a6d-133">Связи</span><span class="sxs-lookup"><span data-stu-id="c0a6d-133">Relationships</span></span>
<span data-ttu-id="c0a6d-134">Нет</span><span class="sxs-lookup"><span data-stu-id="c0a6d-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0a6d-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0a6d-135">JSON Representation</span></span>
<span data-ttu-id="c0a6d-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0a6d-136">Here is a JSON representation of the resource.</span></span>
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






