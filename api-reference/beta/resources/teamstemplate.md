---
title: Тип ресурса teamsTemplate
description: Описание сущности teamsTemplate.
author: nkramer
ms.openlocfilehash: b4e32448f864048fdcb54dc001b21b262df2bba3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327715"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="1df0b-103">Тип ресурса teamsTemplate</span><span class="sxs-lookup"><span data-stu-id="1df0b-103">teamsTemplate resource type</span></span>

> <span data-ttu-id="1df0b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1df0b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1df0b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1df0b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1df0b-106">Шаблон группы — это план для создания [группы](../resources/team.md) в группами Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1df0b-106">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="1df0b-107">Шаблон указывает структуры, параметры и даже контента, который следует предоставить в новые группы, созданные на основе шаблона.</span><span class="sxs-lookup"><span data-stu-id="1df0b-107">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="1df0b-108">Корпорация Майкрософт предоставляет набор базовых шаблонов и пользователи могут сохранять свои собственные пользовательские шаблоны.</span><span class="sxs-lookup"><span data-stu-id="1df0b-108">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="1df0b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="1df0b-109">Properties</span></span>

| <span data-ttu-id="1df0b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="1df0b-110">Property</span></span>            | <span data-ttu-id="1df0b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="1df0b-111">Type</span></span>     | <span data-ttu-id="1df0b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1df0b-112">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1df0b-113">id</span><span class="sxs-lookup"><span data-stu-id="1df0b-113">id</span></span>                  | <span data-ttu-id="1df0b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="1df0b-114">String</span></span>   | <span data-ttu-id="1df0b-115">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="1df0b-115">Unique identifier of the template.</span></span> <span data-ttu-id="1df0b-116">Не может быть null.</span><span class="sxs-lookup"><span data-stu-id="1df0b-116">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1df0b-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1df0b-117">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="1df0b-118">См. также</span><span class="sxs-lookup"><span data-stu-id="1df0b-118">See also</span></span>

- [<span data-ttu-id="1df0b-119">Группа</span><span class="sxs-lookup"><span data-stu-id="1df0b-119">team</span></span>](team.md)

