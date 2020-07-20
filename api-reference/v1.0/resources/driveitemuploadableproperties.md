---
title: Тип ресурса Дривеитемуплоадаблепропертиес
description: Ресурс Дривеитемуплоадаблепропертиес представляет элемент, который отправляется при создании сеанса отправки.
localization_priority: Normal
author: JeremyKelley
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 1f3ef83f36af70aa2efd3cce8d0215d705114e50
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863875"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="b49f7-103">Тип ресурса Дривеитемуплоадаблепропертиес</span><span class="sxs-lookup"><span data-stu-id="b49f7-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="b49f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b49f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b49f7-105">Представляет элемент, который отправляется при [создании сеанса отправки](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="b49f7-105">Represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b49f7-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b49f7-106">JSON representation</span></span>

<span data-ttu-id="b49f7-107">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b49f7-107">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b49f7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b49f7-108">Properties</span></span>

| <span data-ttu-id="b49f7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b49f7-109">Property</span></span>     | <span data-ttu-id="b49f7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b49f7-110">Type</span></span>                              | <span data-ttu-id="b49f7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b49f7-111">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="b49f7-112">**description**</span><span class="sxs-lookup"><span data-stu-id="b49f7-112">**description**</span></span>   |<span data-ttu-id="b49f7-113">String</span><span class="sxs-lookup"><span data-stu-id="b49f7-113">String</span></span>                             | <span data-ttu-id="b49f7-114">Предоставляет видимое пользователю описание элемента.</span><span class="sxs-lookup"><span data-stu-id="b49f7-114">Provides a user-visible description of the item.</span></span> <span data-ttu-id="b49f7-115">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="b49f7-115">Read-write.</span></span> <span data-ttu-id="b49f7-116">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="b49f7-116">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="b49f7-117">**филесизе**</span><span class="sxs-lookup"><span data-stu-id="b49f7-117">**fileSize**</span></span>      |<span data-ttu-id="b49f7-118">Int64</span><span class="sxs-lookup"><span data-stu-id="b49f7-118">Int64</span></span>                              | <span data-ttu-id="b49f7-119">Предоставляет ожидаемый размер файла для выполнения проверки квоты перед отправкой.</span><span class="sxs-lookup"><span data-stu-id="b49f7-119">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="b49f7-120">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="b49f7-120">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="b49f7-121">**fileSystemInfo**</span><span class="sxs-lookup"><span data-stu-id="b49f7-121">**fileSystemInfo**</span></span>|[<span data-ttu-id="b49f7-122">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="b49f7-122">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="b49f7-p103">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="b49f7-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="b49f7-125">**name**</span><span class="sxs-lookup"><span data-stu-id="b49f7-125">**name**</span></span>          |<span data-ttu-id="b49f7-126">String</span><span class="sxs-lookup"><span data-stu-id="b49f7-126">String</span></span>                             | <span data-ttu-id="b49f7-p104">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="b49f7-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->
