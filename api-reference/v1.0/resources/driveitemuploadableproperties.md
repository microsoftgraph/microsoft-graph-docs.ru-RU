---
title: Тип ресурса Дривеитемуплоадаблепропертиес
description: Ресурс Дривеитемуплоадаблепропертиес представляет элемент, который отправляется при создании сеанса отправки.
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 1f3ef83f36af70aa2efd3cce8d0215d705114e50
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863875"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="d2596-103">Тип ресурса Дривеитемуплоадаблепропертиес</span><span class="sxs-lookup"><span data-stu-id="d2596-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="d2596-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d2596-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d2596-105">Представляет элемент, который отправляется при [создании сеанса отправки](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="d2596-105">Represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2596-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2596-106">JSON representation</span></span>

<span data-ttu-id="d2596-107">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2596-107">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.driveItemUploadableProperties",
  "baseType": null
}-->

```json
{
  "description": "String",
  "fileSize": 1024,
  "fileSystemInfo": {"@odata.type": "microsoft.graph.fileSystemInfo"},
  "name": "String"
}
```

## <a name="properties"></a><span data-ttu-id="d2596-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2596-108">Properties</span></span>

| <span data-ttu-id="d2596-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2596-109">Property</span></span>     | <span data-ttu-id="d2596-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d2596-110">Type</span></span>                              | <span data-ttu-id="d2596-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d2596-111">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="d2596-112">**description**</span><span class="sxs-lookup"><span data-stu-id="d2596-112">**description**</span></span>   |<span data-ttu-id="d2596-113">String</span><span class="sxs-lookup"><span data-stu-id="d2596-113">String</span></span>                             | <span data-ttu-id="d2596-114">Предоставляет видимое пользователю описание элемента.</span><span class="sxs-lookup"><span data-stu-id="d2596-114">Provides a user-visible description of the item.</span></span> <span data-ttu-id="d2596-115">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="d2596-115">Read-write.</span></span> <span data-ttu-id="d2596-116">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="d2596-116">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="d2596-117">**филесизе**</span><span class="sxs-lookup"><span data-stu-id="d2596-117">**fileSize**</span></span>      |<span data-ttu-id="d2596-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d2596-118">Int64</span></span>                              | <span data-ttu-id="d2596-119">Предоставляет ожидаемый размер файла для выполнения проверки квоты перед отправкой.</span><span class="sxs-lookup"><span data-stu-id="d2596-119">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="d2596-120">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="d2596-120">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="d2596-121">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="d2596-121">**fileSystemInfo**</span></span>|[<span data-ttu-id="d2596-122">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="d2596-122">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="d2596-123">File system information on client.</span><span class="sxs-lookup"><span data-stu-id="d2596-123">File system information on client.</span></span> <span data-ttu-id="d2596-124">Read-write.</span><span class="sxs-lookup"><span data-stu-id="d2596-124">Read-write.</span></span>                                                      |
|<span data-ttu-id="d2596-125">**name**</span><span class="sxs-lookup"><span data-stu-id="d2596-125">**name**</span></span>          |<span data-ttu-id="d2596-126">String</span><span class="sxs-lookup"><span data-stu-id="d2596-126">String</span></span>                             | <span data-ttu-id="d2596-127">The name of the item (filename and extension).</span><span class="sxs-lookup"><span data-stu-id="d2596-127">The name of the item (filename and extension).</span></span> <span data-ttu-id="d2596-128">Read-write.</span><span class="sxs-lookup"><span data-stu-id="d2596-128">Read-write.</span></span>                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->
