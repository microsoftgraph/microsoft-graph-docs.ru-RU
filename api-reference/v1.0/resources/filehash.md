---
title: Тип ресурса fileHash
description: Содержит информацию о состояниях о хэши файлов (криптографии и расположение конфиденциальные).
ms.openlocfilehash: f7e1f5ceba700a30f1e68e0670ebcec40c3d6fd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025576"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="56c05-103">Тип ресурса fileHash</span><span class="sxs-lookup"><span data-stu-id="56c05-103">fileHash resource type</span></span>

<span data-ttu-id="56c05-104">Содержит информацию о состояниях о хэши файлов (криптографии и расположение конфиденциальные).</span><span class="sxs-lookup"><span data-stu-id="56c05-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="56c05-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="56c05-105">Properties</span></span>

| <span data-ttu-id="56c05-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="56c05-106">Property</span></span>     | <span data-ttu-id="56c05-107">Тип</span><span class="sxs-lookup"><span data-stu-id="56c05-107">Type</span></span>        | <span data-ttu-id="56c05-108">Описание</span><span class="sxs-lookup"><span data-stu-id="56c05-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="56c05-109">hashType</span><span class="sxs-lookup"><span data-stu-id="56c05-109">hashType</span></span>|<span data-ttu-id="56c05-110">fileHashType</span><span class="sxs-lookup"><span data-stu-id="56c05-110">fileHashType</span></span>|<span data-ttu-id="56c05-111">Тип файла хэш-функции.</span><span class="sxs-lookup"><span data-stu-id="56c05-111">File hash type.</span></span> <span data-ttu-id="56c05-112">Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="56c05-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="56c05-113">hashValue</span><span class="sxs-lookup"><span data-stu-id="56c05-113">hashValue</span></span>|<span data-ttu-id="56c05-114">String</span><span class="sxs-lookup"><span data-stu-id="56c05-114">String</span></span>|<span data-ttu-id="56c05-115">Значение хэш файла.</span><span class="sxs-lookup"><span data-stu-id="56c05-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56c05-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="56c05-116">JSON representation</span></span>

<span data-ttu-id="56c05-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="56c05-117">The following is a JSON representation of the resource.</span></span>

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