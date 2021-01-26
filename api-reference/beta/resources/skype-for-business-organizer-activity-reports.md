---
title: Отчеты об организации конференций Skype для бизнеса
description: Вы можете получить подробные сведения об организации конференций в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 6e52d37322bb5dbd67faac0b9b51f6e8afc3aeb2
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983064"
---
# <a name="skype-for-business-organizer-activity-reports"></a>Отчеты об организации конференций Skype для бизнеса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить подробные сведения об организации конференций в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание.** For details about different report views and names, see [Microsoft 365 reports - Skype for Business conference organizer activity](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254).

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение количества действий](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | Stream          | [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) | Отслеживайте динамику использования по количеству и типу проведенных и организованных конференций (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу). |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | Stream          | [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) | Отслеживайте динамику использования по количеству уникальных пользователей и типу проведенных и организованных конференций (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу). |
| [Получение количества минут](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | Поток          | [skypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) | Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт). |


