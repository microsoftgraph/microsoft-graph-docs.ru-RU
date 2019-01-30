---
title: Тип перечисления teamSpecialization
description: Описание варианта использования специальных для команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640324"
---
# <a name="teamspecialization-enum-type"></a>Тип перечисления teamSpecialization

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, будет ли [группы](../resources/team.md) для конкретного варианта использования. Специализация каждой [группы](../resources/team.md) имеет доступ к уникальное поведение и каждый раз, нацелено на пример его использования. Значение по умолчанию — «none».

## <a name="members"></a>Элементы

| Элемент             | Значение | Описание                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| none               | 0     | Тип для группы, которая предоставляет опыт стандартной рабочей группы по умолчанию.          |
| educationStandard  | 1     | Рабочая группа, созданные для образовательных заведений пользователя. Тип Edu — все группы, созданные пользователем образования. |
| educationClass     | 2     | Блог группы интерфейс, оптимизированный для класса. Это позволяет сегментации функций через O365. |
| educationProfessionalLearningCommunity | 3 | Опыт рабочей группы, оптимизированная для PLC. Дополнительные сведения о PLC [здесь](https://en.wikipedia.org/wiki/Professional_learning_community). |
| educationStaff     | 4     |  Тип группы для оптимизированный интерфейс для персонала в организации, где — это ведущий персонала, как участник, администрирования и преподавателей, входят в группы, которое поставляется с специализированных записной книжки. Дополнительные сведения см в [записной книжке OneNote персонала для образовательных учреждений](https://www.onenote.com/staffnotebookedu). |
| unknownFutureValue | 7     | Sentinel значение зарезервировано для выполнения будущее расширение перечисления. |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
