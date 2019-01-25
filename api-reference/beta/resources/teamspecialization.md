---
title: Тип перечисления teamSpecialization
description: Описание варианта использования специальных для команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9e19c6b2242256f0d1b7a23c89aa07787bfc1913
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522653"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="a4441-103">Тип перечисления teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="a4441-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4441-104">Указывает, будет ли [группы](../resources/team.md) для конкретного варианта использования.</span><span class="sxs-lookup"><span data-stu-id="a4441-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="a4441-105">Специализация каждой [группы](../resources/team.md) имеет доступ к уникальное поведение и каждый раз, нацелено на пример его использования.</span><span class="sxs-lookup"><span data-stu-id="a4441-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="a4441-106">Значение по умолчанию — «none».</span><span class="sxs-lookup"><span data-stu-id="a4441-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="a4441-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="a4441-107">Members</span></span>

| <span data-ttu-id="a4441-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="a4441-108">Member</span></span>             | <span data-ttu-id="a4441-109">Значение</span><span class="sxs-lookup"><span data-stu-id="a4441-109">Value</span></span> | <span data-ttu-id="a4441-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a4441-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="a4441-111">none</span><span class="sxs-lookup"><span data-stu-id="a4441-111">none</span></span>               | <span data-ttu-id="a4441-112">(0)</span><span class="sxs-lookup"><span data-stu-id="a4441-112">0</span></span>     | <span data-ttu-id="a4441-113">Тип для группы, которая предоставляет опыт стандартной рабочей группы по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a4441-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="a4441-114">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="a4441-114">unknownFutureValue</span></span> | <span data-ttu-id="a4441-115">7</span><span class="sxs-lookup"><span data-stu-id="a4441-115">7</span></span>     | <span data-ttu-id="a4441-116">Sentinel значение зарезервировано для выполнения будущее расширение перечисления.</span><span class="sxs-lookup"><span data-stu-id="a4441-116">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamspecialization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
