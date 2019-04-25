---
title: Тип ресурса Теамстемплате
description: Описывает объект Теамстемплате.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583174"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="997d3-103">Тип ресурса Теамстемплате</span><span class="sxs-lookup"><span data-stu-id="997d3-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="997d3-104">Шаблон группы — это план для создания [команды](../resources/team.md) в Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="997d3-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="997d3-105">Шаблон определяет структуру, параметры и даже содержимое, которое должно быть подготовлено в новой команде, созданной с помощью шаблона.</span><span class="sxs-lookup"><span data-stu-id="997d3-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="997d3-106">Корпорация Майкрософт предоставляет набор базовых шаблонов и клиентов, которые могут сохранять собственные настраиваемые шаблоны.</span><span class="sxs-lookup"><span data-stu-id="997d3-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="997d3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="997d3-107">Properties</span></span>

| <span data-ttu-id="997d3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="997d3-108">Property</span></span>            | <span data-ttu-id="997d3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="997d3-109">Type</span></span>     | <span data-ttu-id="997d3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="997d3-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="997d3-111">id</span><span class="sxs-lookup"><span data-stu-id="997d3-111">id</span></span>                  | <span data-ttu-id="997d3-112">String</span><span class="sxs-lookup"><span data-stu-id="997d3-112">String</span></span>   | <span data-ttu-id="997d3-113">Уникальный идентификатор шаблона.</span><span class="sxs-lookup"><span data-stu-id="997d3-113">Unique identifier of the template.</span></span> <span data-ttu-id="997d3-114">Не может иметь значение null.</span><span class="sxs-lookup"><span data-stu-id="997d3-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="997d3-115">Описание в формате JSON</span><span class="sxs-lookup"><span data-stu-id="997d3-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="997d3-116">См. также</span><span class="sxs-lookup"><span data-stu-id="997d3-116">See also</span></span>

- [<span data-ttu-id="997d3-117">team</span><span class="sxs-lookup"><span data-stu-id="997d3-117">team</span></span>](team.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
