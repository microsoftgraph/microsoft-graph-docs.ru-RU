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
# <a name="teamspecialization-enum-type"></a>Тип перечисления teamSpecialization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, будет ли [группы](../resources/team.md) для конкретного варианта использования. Специализация каждой [группы](../resources/team.md) имеет доступ к уникальное поведение и каждый раз, нацелено на пример его использования. Значение по умолчанию — «none».

## <a name="members"></a>Элементы

| Элемент             | Значение | Описание                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| none               | (0)     | Тип для группы, которая предоставляет опыт стандартной рабочей группы по умолчанию.          |
| unknownFutureValue | 7     | Sentinel значение зарезервировано для выполнения будущее расширение перечисления. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamspecialization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
