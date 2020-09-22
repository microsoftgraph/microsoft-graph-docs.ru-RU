---
title: Тип ресурса Дривеитемуплоадаблепропертиес
description: Ресурс Дривеитемуплоадаблепропертиес представляет элемент, который отправляется при создании сеанса отправки.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9505de9fd67a5f8cf8d7e89e964d98d758a22bde
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067386"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="855cc-103">Тип ресурса Дривеитемуплоадаблепропертиес</span><span class="sxs-lookup"><span data-stu-id="855cc-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="855cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="855cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="855cc-105">Ресурс **дривеитемуплоадаблепропертиес** представляет элемент, который отправляется при [создании сеанса отправки](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="855cc-105">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="855cc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="855cc-106">Properties</span></span>

| <span data-ttu-id="855cc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="855cc-107">Property</span></span>     | <span data-ttu-id="855cc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="855cc-108">Type</span></span>                              | <span data-ttu-id="855cc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="855cc-109">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="855cc-110">description</span><span class="sxs-lookup"><span data-stu-id="855cc-110">description</span></span>   |<span data-ttu-id="855cc-111">String</span><span class="sxs-lookup"><span data-stu-id="855cc-111">String</span></span>                             | <span data-ttu-id="855cc-112">Предоставляет видимое пользователю описание элемента.</span><span class="sxs-lookup"><span data-stu-id="855cc-112">Provides a user-visible description of the item.</span></span> <span data-ttu-id="855cc-113">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="855cc-113">Read-write.</span></span> <span data-ttu-id="855cc-114">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="855cc-114">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="855cc-115">филесизе</span><span class="sxs-lookup"><span data-stu-id="855cc-115">fileSize</span></span>      |<span data-ttu-id="855cc-116">Int64</span><span class="sxs-lookup"><span data-stu-id="855cc-116">Int64</span></span>                              | <span data-ttu-id="855cc-117">Предоставляет ожидаемый размер файла для выполнения проверки квоты перед отправкой.</span><span class="sxs-lookup"><span data-stu-id="855cc-117">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="855cc-118">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="855cc-118">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="855cc-119">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="855cc-119">fileSystemInfo</span></span>|[<span data-ttu-id="855cc-120">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="855cc-120">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="855cc-p103">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="855cc-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="855cc-123">name</span><span class="sxs-lookup"><span data-stu-id="855cc-123">name</span></span>          |<span data-ttu-id="855cc-124">String</span><span class="sxs-lookup"><span data-stu-id="855cc-124">String</span></span>                             | <span data-ttu-id="855cc-p104">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="855cc-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="855cc-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="855cc-127">JSON representation</span></span>

<span data-ttu-id="855cc-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="855cc-128">The following is a JSON representation of the resource.</span></span>

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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "driveItemUploadableProperties resource",
  "keywords": "driveItemUploadableProperties,createUploadSession",
  "section": "documentation",
  "tocPath": ""
}-->

