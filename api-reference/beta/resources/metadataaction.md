---
title: тип ресурса metadataAction
description: Представляет метаданные, которые будут написаны или удалены из файла.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 23305d8a3e1e89d198b4700e794dd264eabf003b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960399"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="18304-103">тип ресурса metadataAction</span><span class="sxs-lookup"><span data-stu-id="18304-103">metadataAction resource type</span></span>

<span data-ttu-id="18304-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18304-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18304-105">Представляет метаданные, которые будут написаны или удалены из файла.</span><span class="sxs-lookup"><span data-stu-id="18304-105">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="18304-106">**MetadataAction** может быть возвращено с помощью API [evaluateRemoval,](../api/informationprotectionlabel-evaluateremoval.md) [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)и [evaluateClassificationResults.](../api/informationprotectionlabel-evaluateclassificationresults.md)</span><span class="sxs-lookup"><span data-stu-id="18304-106">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="18304-107">Действие информирует о потребляемом приложении определенных пар ключей и значений, которые необходимо добавить в файл, или о конкретных ключах метаданных, которые должны быть удалены из файла.</span><span class="sxs-lookup"><span data-stu-id="18304-107">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="18304-108">Эти метаданные описывают файл или сведения как *помеченные.*</span><span class="sxs-lookup"><span data-stu-id="18304-108">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="18304-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="18304-109">Properties</span></span>

| <span data-ttu-id="18304-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="18304-110">Property</span></span>         | <span data-ttu-id="18304-111">Тип</span><span class="sxs-lookup"><span data-stu-id="18304-111">Type</span></span>                                       | <span data-ttu-id="18304-112">Описание</span><span class="sxs-lookup"><span data-stu-id="18304-112">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="18304-113">metadataToAdd</span><span class="sxs-lookup"><span data-stu-id="18304-113">metadataToAdd</span></span>    | <span data-ttu-id="18304-114">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="18304-114">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="18304-115">Коллекция пар ключевых значений, которые необходимо добавить в файл.</span><span class="sxs-lookup"><span data-stu-id="18304-115">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="18304-116">metadataToRemove</span><span class="sxs-lookup"><span data-stu-id="18304-116">metadataToRemove</span></span> | <span data-ttu-id="18304-117">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="18304-117">String collection</span></span>                          | <span data-ttu-id="18304-118">Коллекция строк, которые указывают, какие ключи следует удалить из метаданных файла.</span><span class="sxs-lookup"><span data-stu-id="18304-118">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="18304-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18304-119">JSON representation</span></span>

<span data-ttu-id="18304-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18304-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  "metadataToAdd": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "metadataToRemove": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

