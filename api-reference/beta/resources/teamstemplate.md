---
title: Тип ресурса Теамстемплате
description: Описывает объект Теамстемплате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dde08e6c4ecde3b3a600958a5af5cd93b5fc600f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964391"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="1a416-103">Тип ресурса Теамстемплате</span><span class="sxs-lookup"><span data-stu-id="1a416-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a416-104">Шаблон группы — это план для создания [команды](../resources/team.md) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1a416-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="1a416-105">Шаблон определяет структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="1a416-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="1a416-106">Корпорация Майкрософт предоставляет набор базовых шаблонов и клиентов, которые могут сохранять собственные настраиваемые шаблоны.</span><span class="sxs-lookup"><span data-stu-id="1a416-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="1a416-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a416-107">Properties</span></span>

| <span data-ttu-id="1a416-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a416-108">Property</span></span>            | <span data-ttu-id="1a416-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1a416-109">Type</span></span>     | <span data-ttu-id="1a416-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a416-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="1a416-111">id</span><span class="sxs-lookup"><span data-stu-id="1a416-111">id</span></span>                  | <span data-ttu-id="1a416-112">String</span><span class="sxs-lookup"><span data-stu-id="1a416-112">String</span></span>   | <span data-ttu-id="1a416-113">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="1a416-113">Unique identifier of the template.</span></span> <span data-ttu-id="1a416-114">Не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="1a416-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1a416-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1a416-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="1a416-116">См. также</span><span class="sxs-lookup"><span data-stu-id="1a416-116">See also</span></span>

- [<span data-ttu-id="1a416-117">team</span><span class="sxs-lookup"><span data-stu-id="1a416-117">team</span></span>](team.md)

