---
title: Отчеты об организации конференций Skype для бизнеса
description: Сведения об активности организованных конференций можно получить в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: f58c289f4fb99d8abd0b2506e0e3dc1776931870
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61241347"
---
# <a name="skype-for-business-organizer-activity-reports"></a>Отчеты об организации конференций Skype для бизнеса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Сведения об активности организованных конференций можно получить в организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание:** Подробные сведения о различных представлениях и именах отчетов [см. в Microsoft 365 отчетов - Skype для бизнеса деятельности организатора конференции.](https://support.office.com/client/Skype-for-Business-Online-conference-organized-activity-03a255d4-0e1d-4b24-b73d-7a62fae36254)

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение количества действий](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md) | Stream          | [SkypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) | Отслеживайте динамику использования по количеству и типу проведенных и организованных конференций (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу). |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md) | Stream          | [SkypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) | Отслеживайте динамику использования по количеству уникальных пользователей и типу проведенных и организованных конференций (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям, веб-конференции, конференции с телефонным подключением и присоединением обратным звонком через Майкрософт или стороннюю службу). |
| [Получение количества минут](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md) | Поток          | [SkypeForBusinessOrganizerActivityMinuteCounts](../resources/skypeforbusinessorganizeractivityminutecounts.md) | Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных и организованных конференций (аудио и видео, с телефонным подключением или с присоединением обратным звонком через Майкрософт). |


