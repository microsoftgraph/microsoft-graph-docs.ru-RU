---
title: Тип ресурса Теамстемплате
description: Описывает объект Теамстемплате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 77101c756e09b4ce2356da2384f2c50b119ae856
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519836"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="7a2db-103">Тип ресурса Теамстемплате</span><span class="sxs-lookup"><span data-stu-id="7a2db-103">teamsTemplate resource type</span></span>

<span data-ttu-id="7a2db-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7a2db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a2db-105">Шаблон группы — это план для создания [команды](../resources/team.md) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7a2db-105">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="7a2db-106">Шаблон определяет структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="7a2db-106">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="7a2db-107">Корпорация Майкрософт предоставляет набор базовых шаблонов и клиентов, которые могут сохранять собственные настраиваемые шаблоны.</span><span class="sxs-lookup"><span data-stu-id="7a2db-107">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="7a2db-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a2db-108">Properties</span></span>

| <span data-ttu-id="7a2db-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a2db-109">Property</span></span>            | <span data-ttu-id="7a2db-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7a2db-110">Type</span></span>     | <span data-ttu-id="7a2db-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7a2db-111">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="7a2db-112">id</span><span class="sxs-lookup"><span data-stu-id="7a2db-112">id</span></span>                  | <span data-ttu-id="7a2db-113">String</span><span class="sxs-lookup"><span data-stu-id="7a2db-113">String</span></span>   | <span data-ttu-id="7a2db-114">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="7a2db-114">Unique identifier of the template.</span></span> <span data-ttu-id="7a2db-115">Не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="7a2db-115">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a2db-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7a2db-116">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="7a2db-117">См. также</span><span class="sxs-lookup"><span data-stu-id="7a2db-117">See also</span></span>

- [<span data-ttu-id="7a2db-118">team</span><span class="sxs-lookup"><span data-stu-id="7a2db-118">team</span></span>](team.md)

