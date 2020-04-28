---
title: Отчеты об участии в конференциях Skype для бизнеса
description: Вы можете получить сведения о действиях по конференц-связи в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 9ef31521125a7b4a8443002847ccf27cd8f265a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520473"
---
# <a name="skype-for-business-participant-activity-reports"></a>Отчеты об участии в конференциях Skype для бизнеса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения о действиях по конференц-связи в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение количества действий](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Stream          | [скипефорбусинесспартиЦипантактивитикаунтс](../resources/skypeforbusinessparticipantactivitycounts.md) | Отслеживайте динамику использования по количеству и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу). |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Stream          | [скипефорбусинесспартиЦипантактивитюсеркаунтс](../resources/skypeforbusinessparticipantactivityusercounts.md) | Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу). |
| [Получение количества минут](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Поток          | [скипефорбусинесспартиЦипантактивитиминутекаунтс](../resources/skypeforbusinessparticipantactivityminutecounts.md) | Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации (аудио и видео). |
