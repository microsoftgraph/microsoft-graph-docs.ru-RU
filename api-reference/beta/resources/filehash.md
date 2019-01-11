---
title: Тип ресурса fileHash
description: Содержит информацию о состояниях о хэши файлов (криптографии и расположение конфиденциальные).
localization_priority: Normal
ms.openlocfilehash: f5d865a7ded230ca611b8628c3648ec1e331c67d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815647"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="4acc6-103">Тип ресурса fileHash</span><span class="sxs-lookup"><span data-stu-id="4acc6-103">fileHash resource type</span></span>

<span data-ttu-id="4acc6-104">Содержит информацию о состояниях о хэши файлов (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="4acc6-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="4acc6-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="4acc6-105">Properties</span></span>

| <span data-ttu-id="4acc6-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="4acc6-106">Property</span></span>     | <span data-ttu-id="4acc6-107">Тип</span><span class="sxs-lookup"><span data-stu-id="4acc6-107">Type</span></span>        | <span data-ttu-id="4acc6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="4acc6-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4acc6-109">hashType</span><span class="sxs-lookup"><span data-stu-id="4acc6-109">hashType</span></span>|<span data-ttu-id="4acc6-110">Перечисление [fileHashType](filehashtypeenumtype.md)</span><span class="sxs-lookup"><span data-stu-id="4acc6-110">[fileHashType](filehashtypeenumtype.md) enum</span></span>|<span data-ttu-id="4acc6-111">Тип файла хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="4acc6-111">File hash type.</span></span> <span data-ttu-id="4acc6-112">Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="4acc6-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="4acc6-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="4acc6-113">hashValue</span></span>|<span data-ttu-id="4acc6-114">Строка</span><span class="sxs-lookup"><span data-stu-id="4acc6-114">String</span></span>|<span data-ttu-id="4acc6-115">Значение хэш файла.</span><span class="sxs-lookup"><span data-stu-id="4acc6-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4acc6-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4acc6-116">JSON representation</span></span>

<span data-ttu-id="4acc6-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4acc6-117">The following is a JSON representation of the resource.</span></span>

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
