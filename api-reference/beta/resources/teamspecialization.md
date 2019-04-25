---
title: тип перечисления ТеамспеЦиализатион
description: Описывает особый вариант использования для команды.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553654"
---
# <a name="teamspecialization-enum-type"></a>тип перечисления ТеамспеЦиализатион

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Указывает, предназначена ли [команда](../resources/team.md) для определенного варианта использования. Каждая специализация [команды](../resources/team.md) имеет доступ к уникальным поведению и возможностям, предназначенным для своего случая использования. Значение по умолчанию: None.

## <a name="members"></a>Элементы

| Элемент             | Значение | Описание                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| Нет               | нуль     | Тип по умолчанию для команды, обеспечивающей стандартную работу группы.          |
| Едукатионстандард  | 1      | Группа, созданная пользователем для образования. Все команды, созданные пользователем для образования образования, имеют тип edu. |
| educationClass     | 2      | Командный интерфейс, оптимизированный для класса. Это позволяет Сегментация функций в O365. |
| Едукатионпрофессионаллеарнингкоммунити | 3  | Рабочая группа, оптимизированная для "переработано". Подробнее о том, как переадресовать [здесь](https://en.wikipedia.org/wiki/Professional_learning_community). |
| Едукатионстафф     | 4      |  Тип команды оптимизированный интерфейс для сотрудников Организации, где руководитель отдела, например участник, является администратором и преподавателями участниками команды, которая поставляется с специализированной записной книжкой. Более подробную информацию можно узнать в разделе [служебная записная книжКа OneNote для образовательных учреждений](https://www.onenote.com/staffnotebookedu). |
| unknownFutureValue | 7      | Значение Sentinel зарезервировано как заполнитель для расширения перечисления в будущем. |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
