---
title: Тип ресурса win32LobAppFileSystemRequirement
description: Содержит путь к файлу или папке для обнаружения приложения Win32
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 498e4b953b283ac0a0cffa6a7a21ea91232b724b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949593"
---
# <a name="win32lobappfilesystemrequirement-resource-type"></a><span data-ttu-id="55066-103">Тип ресурса win32LobAppFileSystemRequirement</span><span class="sxs-lookup"><span data-stu-id="55066-103">win32LobAppFileSystemRequirement resource type</span></span>

> <span data-ttu-id="55066-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="55066-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55066-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="55066-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55066-106">Содержит путь к файлу или папке для обнаружения приложения Win32</span><span class="sxs-lookup"><span data-stu-id="55066-106">Contains file or folder path to detect a Win32 App</span></span>


<span data-ttu-id="55066-107">Наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="55066-107">Inherits from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>

## <a name="properties"></a><span data-ttu-id="55066-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="55066-108">Properties</span></span>
|<span data-ttu-id="55066-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="55066-109">Property</span></span>|<span data-ttu-id="55066-110">Тип</span><span class="sxs-lookup"><span data-stu-id="55066-110">Type</span></span>|<span data-ttu-id="55066-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55066-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55066-112">operator</span><span class="sxs-lookup"><span data-stu-id="55066-112">operator</span></span>|[<span data-ttu-id="55066-113">win32LobAppDetectionOperator</span><span class="sxs-lookup"><span data-stu-id="55066-113">win32LobAppDetectionOperator</span></span>](../resources/intune-apps-win32lobappdetectionoperator.md)|<span data-ttu-id="55066-114">Оператор обнаружения наследуется от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span><span class="sxs-lookup"><span data-stu-id="55066-114">The operator for detection Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md).</span></span> <span data-ttu-id="55066-115">Возможные значения: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span><span class="sxs-lookup"><span data-stu-id="55066-115">Possible values are: `notConfigured`, `equal`, `notEqual`, `greaterThan`, `greaterThanOrEqual`, `lessThan`, `lessThanOrEqual`.</span></span>|
|<span data-ttu-id="55066-116">Детектионвалуе</span><span class="sxs-lookup"><span data-stu-id="55066-116">detectionValue</span></span>|<span data-ttu-id="55066-117">Строка</span><span class="sxs-lookup"><span data-stu-id="55066-117">String</span></span>|<span data-ttu-id="55066-118">Значение обнаружения, унаследованное от [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span><span class="sxs-lookup"><span data-stu-id="55066-118">The detection value Inherited from [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)</span></span>|
|<span data-ttu-id="55066-119">path</span><span class="sxs-lookup"><span data-stu-id="55066-119">path</span></span>|<span data-ttu-id="55066-120">String</span><span class="sxs-lookup"><span data-stu-id="55066-120">String</span></span>|<span data-ttu-id="55066-121">Путь к файлу или папке для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="55066-121">The file or folder path to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="55066-122">Филеорфолдернаме</span><span class="sxs-lookup"><span data-stu-id="55066-122">fileOrFolderName</span></span>|<span data-ttu-id="55066-123">Строка</span><span class="sxs-lookup"><span data-stu-id="55066-123">String</span></span>|<span data-ttu-id="55066-124">Имя файла или папки для определения бизнес-приложения Win32</span><span class="sxs-lookup"><span data-stu-id="55066-124">The file or folder name to detect Win32 Line of Business (LoB) app</span></span>|
|<span data-ttu-id="55066-125">check32BitOn64System</span><span class="sxs-lookup"><span data-stu-id="55066-125">check32BitOn64System</span></span>|<span data-ttu-id="55066-126">Логический</span><span class="sxs-lookup"><span data-stu-id="55066-126">Boolean</span></span>|<span data-ttu-id="55066-127">Значение, указывающее, предназначен ли этот файл или папка для проверки 32-разрядного приложения в 64-разрядной системе</span><span class="sxs-lookup"><span data-stu-id="55066-127">A value indicating whether this file or folder is for checking 32-bit app on 64-bit system</span></span>|
|<span data-ttu-id="55066-128">Детектионтипе</span><span class="sxs-lookup"><span data-stu-id="55066-128">detectionType</span></span>|[<span data-ttu-id="55066-129">win32LobAppFileSystemDetectionType</span><span class="sxs-lookup"><span data-stu-id="55066-129">win32LobAppFileSystemDetectionType</span></span>](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|<span data-ttu-id="55066-130">Тип обнаружения файловой системы.</span><span class="sxs-lookup"><span data-stu-id="55066-130">The file system detection type.</span></span> <span data-ttu-id="55066-131">Возможные значения: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span><span class="sxs-lookup"><span data-stu-id="55066-131">Possible values are: `notConfigured`, `exists`, `modifiedDate`, `createdDate`, `version`, `sizeInMB`, `doesNotExist`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55066-132">Связи</span><span class="sxs-lookup"><span data-stu-id="55066-132">Relationships</span></span>
<span data-ttu-id="55066-133">Нет</span><span class="sxs-lookup"><span data-stu-id="55066-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55066-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55066-134">JSON Representation</span></span>
<span data-ttu-id="55066-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55066-135">Here is a JSON representation of the resource.</span></span>
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




