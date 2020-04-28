---
title: Тип ресурса Метадатаактион
description: Представляет метаданные, которые необходимо записать или удалить из файла.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 592bd308b3c28d36fedb405b0c7dd7f35cba3436
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522654"
---
# <a name="metadataaction-resource-type"></a><span data-ttu-id="e2bc9-103">Тип ресурса Метадатаактион</span><span class="sxs-lookup"><span data-stu-id="e2bc9-103">metadataAction resource type</span></span>

<span data-ttu-id="e2bc9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2bc9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2bc9-105">Представляет метаданные, которые необходимо записать или удалить из файла.</span><span class="sxs-lookup"><span data-stu-id="e2bc9-105">Represents the metadata to be written or removed from a file.</span></span> <span data-ttu-id="e2bc9-106">**метадатаактион** могут возвращаться с помощью API [евалуатеремовал](../api/informationprotectionlabel-evaluateremoval.md), [евалуатеаппликатион](../api/informationprotectionlabel-evaluateapplication.md)и [евалуатеклассификатионресултс](../api/informationprotectionlabel-evaluateclassificationresults.md) .</span><span class="sxs-lookup"><span data-stu-id="e2bc9-106">**metadataAction** may be returned by the [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md), [evaluateApplication](../api/informationprotectionlabel-evaluateapplication.md), and [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md) APIs.</span></span> <span data-ttu-id="e2bc9-107">Действие информирует приложение использования определенных пар "ключ-значение", которые следует добавить в файл, или конкретные ключи метаданных, которые следует удалить из файла.</span><span class="sxs-lookup"><span data-stu-id="e2bc9-107">The action informs the consuming application of the specific key/value pairs that should be added to the file or the specific metadata keys that should be removed from the file.</span></span> <span data-ttu-id="e2bc9-108">Эти метаданные описывают файл или сведения, *помеченные как отмеченные*.</span><span class="sxs-lookup"><span data-stu-id="e2bc9-108">This metadata is what describes the file or information as being *labeled*.</span></span>

## <a name="properties"></a><span data-ttu-id="e2bc9-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2bc9-109">Properties</span></span>

| <span data-ttu-id="e2bc9-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2bc9-110">Property</span></span>         | <span data-ttu-id="e2bc9-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e2bc9-111">Type</span></span>                                       | <span data-ttu-id="e2bc9-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e2bc9-112">Description</span></span>                                                                        |
| :--------------- | :----------------------------------------- | :--------------------------------------------------------------------------------- |
| <span data-ttu-id="e2bc9-113">метадататоадд</span><span class="sxs-lookup"><span data-stu-id="e2bc9-113">metadataToAdd</span></span>    | <span data-ttu-id="e2bc9-114">Коллекция [keyValuePair](keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="e2bc9-114">[keyValuePair](keyvaluepair.md) collection</span></span> | <span data-ttu-id="e2bc9-115">Коллекция пар "ключ-значение", которые следует добавить в файл.</span><span class="sxs-lookup"><span data-stu-id="e2bc9-115">A collection of key value pairs that should be added to the file.</span></span>                  |
| <span data-ttu-id="e2bc9-116">метадататоремове</span><span class="sxs-lookup"><span data-stu-id="e2bc9-116">metadataToRemove</span></span> | <span data-ttu-id="e2bc9-117">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="e2bc9-117">String collection</span></span>                          | <span data-ttu-id="e2bc9-118">Коллекция строк, указывающая, какие ключи необходимо удалить из метаданных файла.</span><span class="sxs-lookup"><span data-stu-id="e2bc9-118">A collection of strings that indicate which keys to remove from the file metadata.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2bc9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2bc9-119">JSON representation</span></span>

<span data-ttu-id="e2bc9-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2bc9-120">The following is a JSON representation of the resource.</span></span>

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