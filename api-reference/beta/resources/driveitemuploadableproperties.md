---
title: Тип ресурса Дривеитемуплоадаблепропертиес
description: Ресурс Дривеитемуплоадаблепропертиес представляет элемент, который отправляется при создании сеанса отправки.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f8511bba850c1d165fe9b7082b7df51900b17962
ms.sourcegitcommit: 2fb178ae78b5ecc47207d2b19d0c5a46e07e0960
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "37333436"
---
# <a name="driveitemuploadableproperties-resource-type"></a><span data-ttu-id="54b64-103">Тип ресурса Дривеитемуплоадаблепропертиес</span><span class="sxs-lookup"><span data-stu-id="54b64-103">driveItemUploadableProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54b64-104">Ресурс **дривеитемуплоадаблепропертиес** представляет элемент, который отправляется при [создании сеанса отправки](../api/driveitem-createuploadsession.md).</span><span class="sxs-lookup"><span data-stu-id="54b64-104">The **driveItemUploadableProperties** resource represents an item being uploaded when [creating an upload session](../api/driveitem-createuploadsession.md).</span></span>

## <a name="properties"></a><span data-ttu-id="54b64-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="54b64-105">Properties</span></span>

| <span data-ttu-id="54b64-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="54b64-106">Property</span></span>     | <span data-ttu-id="54b64-107">Тип</span><span class="sxs-lookup"><span data-stu-id="54b64-107">Type</span></span>                              | <span data-ttu-id="54b64-108">Описание</span><span class="sxs-lookup"><span data-stu-id="54b64-108">Description</span></span>                                                                                         |
|:-------------|:----------------------------------|:----------------------------------------------------------------------------------------------------|
|<span data-ttu-id="54b64-109">description</span><span class="sxs-lookup"><span data-stu-id="54b64-109">description</span></span>   |<span data-ttu-id="54b64-110">String</span><span class="sxs-lookup"><span data-stu-id="54b64-110">String</span></span>                             | <span data-ttu-id="54b64-111">Предоставляет видимое пользователю описание элемента.</span><span class="sxs-lookup"><span data-stu-id="54b64-111">Provides a user-visible description of the item.</span></span> <span data-ttu-id="54b64-112">Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="54b64-112">Read-write.</span></span> <span data-ttu-id="54b64-113">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="54b64-113">Only on OneDrive Personal.</span></span>             |
|<span data-ttu-id="54b64-114">филесизе</span><span class="sxs-lookup"><span data-stu-id="54b64-114">fileSize</span></span>      |<span data-ttu-id="54b64-115">Int64</span><span class="sxs-lookup"><span data-stu-id="54b64-115">Int64</span></span>                              | <span data-ttu-id="54b64-116">Предоставляет ожидаемый размер файла для выполнения проверки квоты перед отправкой.</span><span class="sxs-lookup"><span data-stu-id="54b64-116">Provides an expected file size to perform a quota check prior to upload.</span></span> <span data-ttu-id="54b64-117">Только в OneDrive персональный.</span><span class="sxs-lookup"><span data-stu-id="54b64-117">Only on OneDrive Personal.</span></span> |
|<span data-ttu-id="54b64-118">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="54b64-118">fileSystemInfo</span></span>|[<span data-ttu-id="54b64-119">fileSystemInfo</span><span class="sxs-lookup"><span data-stu-id="54b64-119">fileSystemInfo</span></span>](filesysteminfo.md)| <span data-ttu-id="54b64-p103">Сведения о файловой системе на клиенте. Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="54b64-p103">File system information on client. Read-write.</span></span>                                                      |
|<span data-ttu-id="54b64-122">name</span><span class="sxs-lookup"><span data-stu-id="54b64-122">name</span></span>          |<span data-ttu-id="54b64-123">String</span><span class="sxs-lookup"><span data-stu-id="54b64-123">String</span></span>                             | <span data-ttu-id="54b64-p104">Имя элемента (имя и расширение файла). Чтение и запись.</span><span class="sxs-lookup"><span data-stu-id="54b64-p104">The name of the item (filename and extension). Read-write.</span></span>                                          |

## <a name="json-representation"></a><span data-ttu-id="54b64-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54b64-126">JSON representation</span></span>

<span data-ttu-id="54b64-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54b64-127">The following is a JSON representation of the resource.</span></span>

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