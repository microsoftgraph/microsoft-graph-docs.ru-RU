---
title: Тип ресурса Теамстемплате
description: Описывает объект Теамстемплате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 5fc40b9c2a5789c5bcd7ab5794e41c715223eff3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046393"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="2f082-103">Тип ресурса Теамстемплате</span><span class="sxs-lookup"><span data-stu-id="2f082-103">teamsTemplate resource type</span></span>

<span data-ttu-id="2f082-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f082-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f082-105">Шаблон группы — это план для создания [команды](../resources/team.md) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2f082-105">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="2f082-106">Шаблон определяет структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="2f082-106">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="2f082-107">Корпорация Майкрософт предоставляет набор базовых шаблонов и клиентов, которые могут сохранять собственные настраиваемые шаблоны.</span><span class="sxs-lookup"><span data-stu-id="2f082-107">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="2f082-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f082-108">Properties</span></span>

| <span data-ttu-id="2f082-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f082-109">Property</span></span>            | <span data-ttu-id="2f082-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2f082-110">Type</span></span>     | <span data-ttu-id="2f082-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2f082-111">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="2f082-112">id</span><span class="sxs-lookup"><span data-stu-id="2f082-112">id</span></span>                  | <span data-ttu-id="2f082-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2f082-113">String</span></span>   | <span data-ttu-id="2f082-114">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="2f082-114">Unique identifier of the template.</span></span> <span data-ttu-id="2f082-115">Не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="2f082-115">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2f082-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="2f082-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

## <a name="see-also"></a><span data-ttu-id="2f082-117">См. также</span><span class="sxs-lookup"><span data-stu-id="2f082-117">See also</span></span>

- [<span data-ttu-id="2f082-118">team</span><span class="sxs-lookup"><span data-stu-id="2f082-118">team</span></span>](team.md)



