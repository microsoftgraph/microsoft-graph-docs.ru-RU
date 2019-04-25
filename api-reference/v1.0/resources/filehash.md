---
title: Тип ресурса fileHash
description: Содержит сведения о состоянии хэшей файлов (криптографии и зависящие от местонахождения).
localization_priority: Normal
ms.openlocfilehash: 9d72812d1ad43999ea3ed5b28251d629b9380d47
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564773"
---
# <a name="filehash-resource-type"></a><span data-ttu-id="8d870-103">Тип ресурса fileHash</span><span class="sxs-lookup"><span data-stu-id="8d870-103">fileHash resource type</span></span>

<span data-ttu-id="8d870-104">Содержит сведения о состоянии хэшей файлов (криптографии и зависящие от местонахождения).</span><span class="sxs-lookup"><span data-stu-id="8d870-104">Contains stateful information about file hashes (cryptographic and location-sensitive).</span></span>

## <a name="properties"></a><span data-ttu-id="8d870-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d870-105">Properties</span></span>

| <span data-ttu-id="8d870-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d870-106">Property</span></span>     | <span data-ttu-id="8d870-107">Тип</span><span class="sxs-lookup"><span data-stu-id="8d870-107">Type</span></span>        | <span data-ttu-id="8d870-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8d870-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8d870-109">Хаштипе</span><span class="sxs-lookup"><span data-stu-id="8d870-109">hashType</span></span>|<span data-ttu-id="8d870-110">fileHashType</span><span class="sxs-lookup"><span data-stu-id="8d870-110">fileHashType</span></span>|<span data-ttu-id="8d870-111">Тип хэша файла.</span><span class="sxs-lookup"><span data-stu-id="8d870-111">File hash type.</span></span> <span data-ttu-id="8d870-112">Возможные значения: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span><span class="sxs-lookup"><span data-stu-id="8d870-112">Possible values are: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash`, `ctph`, `peSha1`, `peSha256`.</span></span>|
|<span data-ttu-id="8d870-113">Хашвалуе</span><span class="sxs-lookup"><span data-stu-id="8d870-113">hashValue</span></span>|<span data-ttu-id="8d870-114">String</span><span class="sxs-lookup"><span data-stu-id="8d870-114">String</span></span>|<span data-ttu-id="8d870-115">Значение хэша файла.</span><span class="sxs-lookup"><span data-stu-id="8d870-115">Value of the file hash.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8d870-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d870-116">JSON representation</span></span>

<span data-ttu-id="8d870-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d870-117">The following is a JSON representation of the resource.</span></span>

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
