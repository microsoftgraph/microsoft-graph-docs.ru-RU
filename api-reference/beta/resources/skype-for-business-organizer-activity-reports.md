---
title: Отчеты об организации конференций Skype для бизнеса
description: Подробные сведения можно получить упорядоченный конференций действия внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 706e9d88e52756ac8df4db8fd5c738a50d545e37
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514056"
---
# <a name="skype-for-business-organizer-activity-reports"></a>Отчеты об организации конференций Skype для бизнеса

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подробные сведения можно получить упорядоченный конференций действия внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение количества действий](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | Stream          | [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) | Получение сведений о том, как меняется количество и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу). |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | Stream          | [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) | Получение сведений о том, как меняется количество уникальных пользователей и тип сеансов конференц-связи, проводимых и организуемых пользователями в организации. (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу). |
| [Получение количества минут](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | Поток          | [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) | Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт). |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-organizer-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
