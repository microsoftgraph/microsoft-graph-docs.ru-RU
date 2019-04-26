---
title: Тип ресурса Теамстемплате
description: Описывает объект Теамстемплате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4e960e85e6e8b3017d8f4e0ab89bb85cb4c12f58
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345750"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="ed9d2-103">Тип ресурса Теамстемплате</span><span class="sxs-lookup"><span data-stu-id="ed9d2-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed9d2-104">Шаблон группы — это план для создания [команды](../resources/team.md) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ed9d2-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="ed9d2-105">Шаблон определяет структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="ed9d2-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="ed9d2-106">Корпорация Майкрософт предоставляет набор базовых шаблонов и клиентов, которые могут сохранять собственные настраиваемые шаблоны.</span><span class="sxs-lookup"><span data-stu-id="ed9d2-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="ed9d2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed9d2-107">Properties</span></span>

| <span data-ttu-id="ed9d2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed9d2-108">Property</span></span>            | <span data-ttu-id="ed9d2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ed9d2-109">Type</span></span>     | <span data-ttu-id="ed9d2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ed9d2-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="ed9d2-111">id</span><span class="sxs-lookup"><span data-stu-id="ed9d2-111">id</span></span>                  | <span data-ttu-id="ed9d2-112">String</span><span class="sxs-lookup"><span data-stu-id="ed9d2-112">String</span></span>   | <span data-ttu-id="ed9d2-113">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="ed9d2-113">Unique identifier of the template.</span></span> <span data-ttu-id="ed9d2-114">Не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="ed9d2-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ed9d2-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ed9d2-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="ed9d2-116">См. также</span><span class="sxs-lookup"><span data-stu-id="ed9d2-116">See also</span></span>

- [<span data-ttu-id="ed9d2-117">team</span><span class="sxs-lookup"><span data-stu-id="ed9d2-117">team</span></span>](team.md)

