---
title: тип ресурса educationFileResource
description: Подкласс educationResource, который представляет объект файла, связанный с назначением или отправкой.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 814ea6119210184356c561ac4f6a3dee5d3eac10
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912617"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="66044-103">тип ресурса educationFileResource</span><span class="sxs-lookup"><span data-stu-id="66044-103">educationFileResource resource type</span></span>

<span data-ttu-id="66044-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66044-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="66044-105">Подкласс [educationResource,](educationresource.md) который представляет объект файла, связанный с назначением или отправкой.</span><span class="sxs-lookup"><span data-stu-id="66044-105">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>

<span data-ttu-id="66044-106">В этом случае файл не является одним из специальных файлов (Word, Excel и т. д.), а является файлом, который не имеет специальной обработки в системе.</span><span class="sxs-lookup"><span data-stu-id="66044-106">In this case, the file isn't one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="66044-107">Файловый ресурс должен храниться в **ресурсеFolder,** связанном с назначением или отправкой этого ресурса.</span><span class="sxs-lookup"><span data-stu-id="66044-107">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="66044-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="66044-108">Properties</span></span>
| <span data-ttu-id="66044-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="66044-109">Property</span></span>     | <span data-ttu-id="66044-110">Тип</span><span class="sxs-lookup"><span data-stu-id="66044-110">Type</span></span>   |<span data-ttu-id="66044-111">Описание</span><span class="sxs-lookup"><span data-stu-id="66044-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66044-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="66044-112">fileUrl</span></span>|<span data-ttu-id="66044-113">String</span><span class="sxs-lookup"><span data-stu-id="66044-113">String</span></span>|<span data-ttu-id="66044-114">Расположение на диске файлового ресурса.</span><span class="sxs-lookup"><span data-stu-id="66044-114">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="66044-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="66044-115">JSON representation</span></span>

<span data-ttu-id="66044-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66044-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


