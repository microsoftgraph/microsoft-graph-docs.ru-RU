---
title: Отчеты об участии в конференциях Skype для бизнеса
description: Подробные сведения можно получить в действии конференц-связи внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 61c47820febba8f49b98ca19c82d12770da95ce2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516842"
---
# <a name="skype-for-business-participant-activity-reports"></a>Отчеты об участии в конференциях Skype для бизнеса

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Подробные сведения можно получить в действии конференц-связи внутри организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение количества действий](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Stream          | [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) | Отследите динамику использования по количеству и типу сеансов конференц-связи, в которых участвовали сотрудники организации. Такие типы включают обмен мгновенными сообщениями, общий доступ к приложениям, аудио, видео, а также веб-конференции, конференции с возможностью присоединения по прямому или обратному звонку (сторонняя служба). |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Stream          | [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) | Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу). |
| [Получение количества минут](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Поток          | [skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md) | Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации (аудио и видео). |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/skype-for-business-participant-activity-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
