---
title: Тип ресурса Дривеитемуплоадаблепропертиес
description: Ресурс Дривеитемуплоадаблепропертиес представляет элемент, который отправляется при создании сеанса отправки.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a68180476910051dc3633ee5dce7363c77eb60ae
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505562"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="a6b63-103">Тип ресурса Дривеитемуплоадаблепропертиес</span><span class="sxs-lookup"><span data-stu-id="a6b63-103">driveItemUploadableProperties resource type</span></span>

<span data-ttu-id="a6b63-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a6b63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6b63-105">Ресурс **дривеитемуплоадаблепропертиес** представляет элемент, который отправляется при [создании сеанса отправки](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="a6b63-105">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a6b63-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a6b63-106">Properties</span></span>

| <span data-ttu-id="a6b63-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a6b63-107">Property</span></span>     | <span data-ttu-id="a6b63-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a6b63-108">Type</span></span>                              | <span data-ttu-id="a6b63-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a6b63-109">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="a6b63-110">description</span><span class="sxs-lookup"><span data-stu-id="a6b63-110">description</span></span>   |<span data-ttu-id="a6b63-111">String</span><span class="sxs-lookup"><span data-stu-id="a6b63-111">String</span></span>                             | <span data-ttu-id="a6b63-112">Предоставляет видимое пользователю описание элемента.</span><span class="sxs-lookup"><span data-stu-id="a6b63-112">Provides a user-visible description of the item.</span></span> <span data-ttu-id="a6b63-113">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="a6b63-113">Read-write.</span></span> <span data-ttu-id="a6b63-114">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="a6b63-114">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="a6b63-115">филесизе</span><span class="sxs-lookup"><span data-stu-id="a6b63-115">fileSize</span></span>      |<span data-ttu-id="a6b63-116">Int64</span><span class="sxs-lookup"><span data-stu-id="a6b63-116">Int64</span></span>                              | <span data-ttu-id="a6b63-117">Предоставляет ожидаемый размер файла для выполнения проверки квоты перед отправкой.</span><span class="sxs-lookup"><span data-stu-id="a6b63-117">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="a6b63-118">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="a6b63-118">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="a6b63-119">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="a6b63-119">fileSystemInfo</span></span>|[<span data-ttu-id="a6b63-120">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="a6b63-120">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="a6b63-p103">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="a6b63-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="a6b63-123">name</span><span class="sxs-lookup"><span data-stu-id="a6b63-123">name</span></span>          |<span data-ttu-id="a6b63-124">String</span><span class="sxs-lookup"><span data-stu-id="a6b63-124">String</span></span>                             | <span data-ttu-id="a6b63-p104">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="a6b63-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="a6b63-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a6b63-127">JSON representation</span></span>

<span data-ttu-id="a6b63-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a6b63-128">The following is a JSON representation of the resource.</span></span>

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