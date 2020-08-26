---
title: Тип ресурса Теамстемплате
description: Описывает объект Теамстемплате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c32c8cfa770bd7633915e0e8f9b6d371458d4173
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873452"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="bb5d8-103">Тип ресурса Теамстемплате</span><span class="sxs-lookup"><span data-stu-id="bb5d8-103">teamsTemplate resource type</span></span>

<span data-ttu-id="bb5d8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb5d8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb5d8-105">Шаблон группы — это план для создания [команды](../resources/team.md) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="bb5d8-105">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="bb5d8-106">Шаблон определяет структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="bb5d8-106">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="bb5d8-107">Корпорация Майкрософт предоставляет набор базовых шаблонов и клиентов, которые могут сохранять собственные настраиваемые шаблоны.</span><span class="sxs-lookup"><span data-stu-id="bb5d8-107">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="bb5d8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb5d8-108">Properties</span></span>

| <span data-ttu-id="bb5d8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb5d8-109">Property</span></span>            | <span data-ttu-id="bb5d8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bb5d8-110">Type</span></span>     | <span data-ttu-id="bb5d8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bb5d8-111">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="bb5d8-112">id</span><span class="sxs-lookup"><span data-stu-id="bb5d8-112">id</span></span>                  | <span data-ttu-id="bb5d8-113">Строка</span><span class="sxs-lookup"><span data-stu-id="bb5d8-113">String</span></span>   | <span data-ttu-id="bb5d8-114">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="bb5d8-114">Unique identifier of the template.</span></span> <span data-ttu-id="bb5d8-115">Не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="bb5d8-115">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bb5d8-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bb5d8-116">JSON representation</span></span>

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

## <a name="see-also"></a><span data-ttu-id="bb5d8-117">См. также</span><span class="sxs-lookup"><span data-stu-id="bb5d8-117">See also</span></span>

- [<span data-ttu-id="bb5d8-118">team</span><span class="sxs-lookup"><span data-stu-id="bb5d8-118">team</span></span>](team.md)

