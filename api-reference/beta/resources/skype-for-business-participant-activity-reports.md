---
title: Отчеты об участии в конференциях Skype для бизнеса
description: Вы можете получить сведения о действиях по конференц-связи в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0701a31db5a1c57e67efba477a5f2d0c6d47b5e9
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897990"
---
# <a name="skype-for-business-participant-activity-reports"></a>Отчеты об участии в конференциях Skype для бизнеса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения о действиях по конференц-связи в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports: действие участника конференции в Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение количества действий](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md) | Stream          | [скипефорбусинесспартиЦипантактивитикаунтс](../resources/skypeforbusinessparticipantactivitycounts.md) | Отслеживайте динамику использования по количеству и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу). |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md) | Stream          | [скипефорбусинесспартиЦипантактивитюсеркаунтс](../resources/skypeforbusinessparticipantactivityusercounts.md) | Отслеживайте динамику использования по количеству уникальных пользователей и типу конференций, в которых участвовали сотрудники организации (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через стороннюю службу). |
| [Получение количества минут](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md) | Поток          | [скипефорбусинесспартиЦипантактивитиминутекаунтс](../resources/skypeforbusinessparticipantactivityminutecounts.md) | Отслеживайте динамику использования по продолжительности (в минутах) и типу конференций, в которых участвовали сотрудники организации (аудио и видео). |
