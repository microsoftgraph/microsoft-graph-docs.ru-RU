---
title: Тип ресурса fileHash
description: Содержит сведения о состоянии хэшей файлов (криптографии и зависящие от местонахождения).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 532389671cacb907c7e85862a621b936ec1691a0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973536"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="1c6e7-103">Тип ресурса fileHash</span><span class="sxs-lookup"><span data-stu-id="1c6e7-103">fileHash resource type</span></span>

<span data-ttu-id="1c6e7-104">Содержит сведения о состоянии хэшей файлов (криптографии и зависящие от местонахождения).</span><span class="sxs-lookup"><span data-stu-id="1c6e7-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="1c6e7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c6e7-105">Properties</span></span>

| <span data-ttu-id="1c6e7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c6e7-106">Property</span></span>     | <span data-ttu-id="1c6e7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1c6e7-107">Type</span></span>        | <span data-ttu-id="1c6e7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1c6e7-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1c6e7-109">Хаштипе</span><span class="sxs-lookup"><span data-stu-id="1c6e7-109">hashType</span></span>|<span data-ttu-id="1c6e7-110">Перечисление [филехаштипе](filehashtypeenumtype.md)</span><span class="sxs-lookup"><span data-stu-id="1c6e7-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="1c6e7-111">Тип хэша файла.</span><span class="sxs-lookup"><span data-stu-id="1c6e7-111">File hash type.</span></span> <span data-ttu-id="1c6e7-112">Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="1c6e7-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="1c6e7-113">Хашвалуе</span><span class="sxs-lookup"><span data-stu-id="1c6e7-113">hashValue</span></span>|<span data-ttu-id="1c6e7-114">String</span><span class="sxs-lookup"><span data-stu-id="1c6e7-114">String</span></span>|<span data-ttu-id="1c6e7-115">Значение хэша файла.</span><span class="sxs-lookup"><span data-stu-id="1c6e7-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1c6e7-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c6e7-116">JSON representation</span></span>

<span data-ttu-id="1c6e7-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c6e7-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.fileHash"
}-->

```json
{
  "hashType": "@odata.type: microsoft.graph.fileHashType",
  "hashValue": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "fileHash resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
