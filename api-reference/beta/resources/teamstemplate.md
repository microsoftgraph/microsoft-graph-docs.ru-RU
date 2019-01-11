---
title: Тип ресурса teamsTemplate
description: Описание сущности teamsTemplate.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 6e847c7ef0b13dd9c4281c17939164128be8b6a5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818874"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="35bfa-103">Тип ресурса teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="35bfa-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="35bfa-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35bfa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35bfa-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35bfa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="35bfa-106">Шаблон группы — это план для создания [группы](../resources/team.md) в группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="35bfa-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="35bfa-107">Шаблон указывает структуры, параметры и даже контента, который следует предоставить в новые группы, созданные на основе шаблона.</span><span class="sxs-lookup"><span data-stu-id="35bfa-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="35bfa-108">Корпорация Майкрософт предоставляет набор базовых шаблонов и пользователи могут сохранять свои собственные пользовательские шаблоны.</span><span class="sxs-lookup"><span data-stu-id="35bfa-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="35bfa-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="35bfa-109">Properties</span></span>

| <span data-ttu-id="35bfa-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="35bfa-110">Property</span></span>            | <span data-ttu-id="35bfa-111">Тип</span><span class="sxs-lookup"><span data-stu-id="35bfa-111">Type</span></span>     | <span data-ttu-id="35bfa-112">Описание</span><span class="sxs-lookup"><span data-stu-id="35bfa-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="35bfa-113">id</span><span class="sxs-lookup"><span data-stu-id="35bfa-113">id</span></span>                  | <span data-ttu-id="35bfa-114">Строка</span><span class="sxs-lookup"><span data-stu-id="35bfa-114">String</span></span>   | <span data-ttu-id="35bfa-115">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="35bfa-115">Unique identifier of the template.</span></span> <span data-ttu-id="35bfa-116">Не может быть null.</span><span class="sxs-lookup"><span data-stu-id="35bfa-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35bfa-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35bfa-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="35bfa-118">См. также</span><span class="sxs-lookup"><span data-stu-id="35bfa-118">See also</span></span>

- [<span data-ttu-id="35bfa-119">Группа</span><span class="sxs-lookup"><span data-stu-id="35bfa-119">team</span></span>](team.md)

