---
author: nilakhan
description: Представляет сведения для отправки документа на печать
title: Тип ресурса Принтдокументуплоадпропертиес
localization_priority: Normal
doc_type: resourcePageType
ms.prod: universal-print
ms.openlocfilehash: 1249eaae4d62cffe14935587c655ba402237b0ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727971"
---
# <a name="printdocumentuploadproperties-resource-type"></a><span data-ttu-id="9195e-103">Тип ресурса Принтдокументуплоадпропертиес</span><span class="sxs-lookup"><span data-stu-id="9195e-103">printDocumentUploadProperties resource type</span></span>

<span data-ttu-id="9195e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9195e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9195e-105">Описывает отправляемый документ</span><span class="sxs-lookup"><span data-stu-id="9195e-105">Describes the document that is being uploaded</span></span>

## <a name="json-representation"></a><span data-ttu-id="9195e-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9195e-106">JSON representation</span></span>

<span data-ttu-id="9195e-107">Ниже показано представление JSON ресурса.</span><span class="sxs-lookup"><span data-stu-id="9195e-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.printDocumentUploadProperties",
  "baseType": null
}-->

```json
{
  "contentType": "String",
  "documentName": "String",
  "size": "Int64",
}
```

## <a name="properties"></a><span data-ttu-id="9195e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9195e-108">Properties</span></span>


| <span data-ttu-id="9195e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9195e-109">Property</span></span>       | <span data-ttu-id="9195e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9195e-110">Type</span></span>              |<span data-ttu-id="9195e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9195e-111">Description</span></span>
|:-------------------|:------------------|:------------------------------------
| <span data-ttu-id="9195e-112">contentType</span><span class="sxs-lookup"><span data-stu-id="9195e-112">contentType</span></span> | <span data-ttu-id="9195e-113">String</span><span class="sxs-lookup"><span data-stu-id="9195e-113">String</span></span>    | <span data-ttu-id="9195e-114">Тип контента документа (MIME).</span><span class="sxs-lookup"><span data-stu-id="9195e-114">The document's content (MIME) type.</span></span>
| <span data-ttu-id="9195e-115">Имя_документа</span><span class="sxs-lookup"><span data-stu-id="9195e-115">documentName</span></span> | <span data-ttu-id="9195e-116">Строка</span><span class="sxs-lookup"><span data-stu-id="9195e-116">String</span></span> | <span data-ttu-id="9195e-117">Имя документа.</span><span class="sxs-lookup"><span data-stu-id="9195e-117">The document's name.</span></span>
| <span data-ttu-id="9195e-118">size</span><span class="sxs-lookup"><span data-stu-id="9195e-118">size</span></span>          | <span data-ttu-id="9195e-119">Int64</span><span class="sxs-lookup"><span data-stu-id="9195e-119">Int64</span></span>            | <span data-ttu-id="9195e-120">Размер документа в байтах.</span><span class="sxs-lookup"><span data-stu-id="9195e-120">The document's size in bytes.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "printDocumentUploadProperties",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
