---
title: Тип ресурса Метадатаактион
description: Представляет метаданные, которые необходимо записать или удалить из файла.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8652a33de04d0a28a34c3738dd1706d6aff5e5b9
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938907"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="f1843-103">Тип ресурса Метадатаактион</span><span class="sxs-lookup"><span data-stu-id="f1843-103">metadataAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1843-104">Представляет метаданные, которые необходимо записать или удалить из файла.</span><span class="sxs-lookup"><span data-stu-id="f1843-104">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="f1843-105">**метадатаактион** могут возвращаться с помощью API [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md), [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)и [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) .</span><span class="sxs-lookup"><span data-stu-id="f1843-105">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="f1843-106">Действие информирует приложение использования определенных пар "ключ-значение", которые следует добавить в файл, или конкретные ключи метаданных, которые следует удалить из файла.</span><span class="sxs-lookup"><span data-stu-id="f1843-106">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="f1843-107">Эти метаданные описывают файл или сведения, *помеченные как отмеченные*.</span><span class="sxs-lookup"><span data-stu-id="f1843-107">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="f1843-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1843-108">Properties</span></span>

| <span data-ttu-id="f1843-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1843-109">Property</span></span>         | <span data-ttu-id="f1843-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f1843-110">Type</span></span>                                       | <span data-ttu-id="f1843-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f1843-111">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="f1843-112">метадататоадд</span><span class="sxs-lookup"><span data-stu-id="f1843-112">metadataToAdd</span></span>    | <span data-ttu-id="f1843-113">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="f1843-113">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="f1843-114">Коллекция пар "ключ-значение", которые следует добавить в файл.</span><span class="sxs-lookup"><span data-stu-id="f1843-114">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="f1843-115">метадататоремове</span><span class="sxs-lookup"><span data-stu-id="f1843-115">metadataToRemove</span></span> | <span data-ttu-id="f1843-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f1843-116">String collection</span></span>                          | <span data-ttu-id="f1843-117">Коллекция строк, указывающая, какие ключи необходимо удалить из метаданных файла.</span><span class="sxs-lookup"><span data-stu-id="f1843-117">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f1843-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1843-118">JSON representation</span></span>

<span data-ttu-id="f1843-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1843-119">The following is a JSON representation of the resource.</span></span>

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