---
title: Тип ресурса teamsTemplate
description: Описание сущности teamsTemplate.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9bd5047950ed1ed3c57950d2c4b708a78b570649
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940087"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="1e0ab-103">Тип ресурса teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="1e0ab-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="1e0ab-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1e0ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e0ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1e0ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e0ab-106">Шаблон группы — это план для создания [группы](../resources/team.md) в группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1e0ab-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="1e0ab-107">Шаблон указывает структуры, параметры и даже контента, который следует предоставить в новые группы, созданные на основе шаблона.</span><span class="sxs-lookup"><span data-stu-id="1e0ab-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="1e0ab-108">Корпорация Майкрософт предоставляет набор базовых шаблонов и пользователи могут сохранять свои собственные пользовательские шаблоны.</span><span class="sxs-lookup"><span data-stu-id="1e0ab-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="1e0ab-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1e0ab-109">Properties</span></span>

| <span data-ttu-id="1e0ab-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1e0ab-110">Property</span></span>            | <span data-ttu-id="1e0ab-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1e0ab-111">Type</span></span>     | <span data-ttu-id="1e0ab-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1e0ab-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1e0ab-113">id</span><span class="sxs-lookup"><span data-stu-id="1e0ab-113">id</span></span>                  | <span data-ttu-id="1e0ab-114">Строка</span><span class="sxs-lookup"><span data-stu-id="1e0ab-114">String</span></span>   | <span data-ttu-id="1e0ab-115">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="1e0ab-115">Unique identifier of the template.</span></span> <span data-ttu-id="1e0ab-116">Не может быть null.</span><span class="sxs-lookup"><span data-stu-id="1e0ab-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1e0ab-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1e0ab-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="1e0ab-118">См. также</span><span class="sxs-lookup"><span data-stu-id="1e0ab-118">See also</span></span>

- [<span data-ttu-id="1e0ab-119">Группа</span><span class="sxs-lookup"><span data-stu-id="1e0ab-119">team</span></span>](team.md)

