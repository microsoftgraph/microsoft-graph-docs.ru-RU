---
title: Тип ресурса fileHash
description: Содержит сведения о состоянии хэшей файлов (криптографии и зависящие от местонахождения).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 06097280b54e065842db7aa53ff060ce2ce5d5e1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986087"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="b5ca4-103">Тип ресурса fileHash</span><span class="sxs-lookup"><span data-stu-id="b5ca4-103">fileHash resource type</span></span>

<span data-ttu-id="b5ca4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5ca4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5ca4-105">Содержит сведения о состоянии хэшей файлов (криптографии и зависящие от местонахождения).</span><span class="sxs-lookup"><span data-stu-id="b5ca4-105">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="b5ca4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b5ca4-106">Properties</span></span>

| <span data-ttu-id="b5ca4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b5ca4-107">Property</span></span>     | <span data-ttu-id="b5ca4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b5ca4-108">Type</span></span>        | <span data-ttu-id="b5ca4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b5ca4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5ca4-110">хаштипе</span><span class="sxs-lookup"><span data-stu-id="b5ca4-110">hashType</span></span>|<span data-ttu-id="b5ca4-111">Перечисление [филехаштипе](filehashtypeenumtype.md)</span><span class="sxs-lookup"><span data-stu-id="b5ca4-111">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="b5ca4-112">Тип хэша файла.</span><span class="sxs-lookup"><span data-stu-id="b5ca4-112">File hash type.</span></span> <span data-ttu-id="b5ca4-113">Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="b5ca4-113">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="b5ca4-114">хашвалуе</span><span class="sxs-lookup"><span data-stu-id="b5ca4-114">hashValue</span></span>|<span data-ttu-id="b5ca4-115">String</span><span class="sxs-lookup"><span data-stu-id="b5ca4-115">String</span></span>|<span data-ttu-id="b5ca4-116">Значение хэша файла.</span><span class="sxs-lookup"><span data-stu-id="b5ca4-116">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5ca4-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b5ca4-117">JSON representation</span></span>

<span data-ttu-id="b5ca4-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b5ca4-118">The following is a JSON representation of the resource.</span></span>

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


