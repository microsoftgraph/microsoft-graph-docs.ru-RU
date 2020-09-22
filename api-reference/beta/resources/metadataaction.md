---
title: Тип ресурса Метадатаактион
description: Представляет метаданные, которые необходимо записать или удалить из файла.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55ddd644428662f6a646fd9c003761ab6f7c1e9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021387"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="24ce0-103">Тип ресурса Метадатаактион</span><span class="sxs-lookup"><span data-stu-id="24ce0-103">metadataAction resource type</span></span>

<span data-ttu-id="24ce0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24ce0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24ce0-105">Представляет метаданные, которые необходимо записать или удалить из файла.</span><span class="sxs-lookup"><span data-stu-id="24ce0-105">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="24ce0-106">**метадатаактион** могут возвращаться с помощью API [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md), [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)и [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) .</span><span class="sxs-lookup"><span data-stu-id="24ce0-106">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="24ce0-107">Действие информирует приложение использования определенных пар "ключ-значение", которые следует добавить в файл, или конкретные ключи метаданных, которые следует удалить из файла.</span><span class="sxs-lookup"><span data-stu-id="24ce0-107">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="24ce0-108">Эти метаданные описывают файл или сведения, *помеченные как отмеченные*.</span><span class="sxs-lookup"><span data-stu-id="24ce0-108">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="24ce0-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="24ce0-109">Properties</span></span>

| <span data-ttu-id="24ce0-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="24ce0-110">Property</span></span>         | <span data-ttu-id="24ce0-111">Тип</span><span class="sxs-lookup"><span data-stu-id="24ce0-111">Type</span></span>                                       | <span data-ttu-id="24ce0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="24ce0-112">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="24ce0-113">метадататоадд</span><span class="sxs-lookup"><span data-stu-id="24ce0-113">metadataToAdd</span></span>    | <span data-ttu-id="24ce0-114">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="24ce0-114">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="24ce0-115">Коллекция пар "ключ-значение", которые следует добавить в файл.</span><span class="sxs-lookup"><span data-stu-id="24ce0-115">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="24ce0-116">метадататоремове</span><span class="sxs-lookup"><span data-stu-id="24ce0-116">metadataToRemove</span></span> | <span data-ttu-id="24ce0-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="24ce0-117">String collection</span></span>                          | <span data-ttu-id="24ce0-118">Коллекция строк, указывающая, какие ключи необходимо удалить из метаданных файла.</span><span class="sxs-lookup"><span data-stu-id="24ce0-118">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24ce0-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24ce0-119">JSON representation</span></span>

<span data-ttu-id="24ce0-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24ce0-120">The following is a JSON representation of the resource.</span></span>

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

