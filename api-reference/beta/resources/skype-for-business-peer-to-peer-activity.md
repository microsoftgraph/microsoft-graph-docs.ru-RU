---
title: Отчеты об активности в одноранговых сеансах Skype для бизнеса
description: Вы можете получить сведения об одноранговой активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 76411b36259ade242be327525bbc1d65c7edd021
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997601"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Отчеты об активности в одноранговых сеансах Skype для бизнеса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения об одноранговой активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти [в статье Microsoft 365 Reports-Peer-to-Peer Activity (Microsoft](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение количества действий](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | Stream          | [скипефорбусинесспиртопирактивитикаунтс](../resources/skypeforbusinesspeertopeeractivitycounts.md) | Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов). |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Stream          | [скипефорбусинесспиртопирактивитюсеркаунтс](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | Отслеживайте динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов в одноранговых сеансах). |
| [Получение количества минут](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Поток          | [скипефорбусинесспиртопирактивитиминутекаунтс](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов (аудио и видео). |


