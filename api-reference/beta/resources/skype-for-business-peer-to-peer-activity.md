---
title: Отчеты об активности в одноранговых сеансах Skype для бизнеса
description: Вы можете получить сведения об одноранговой активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 60f8e5c5878822eaae64d5f10d0ff52dd4bc004f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964993"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Отчеты об активности в одноранговых сеансах Skype для бизнеса

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения об одноранговой активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений для организации.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение количества действий](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | Stream          | [Скипефорбусинесспиртопирактивитикаунтс](../resources/skypeforbusinesspeertopeeractivitycounts.md) | Отслеживайте динамику использования по количеству и типу проведенных в организации сеансов (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов). |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Поток          | [Скипефорбусинесспиртопирактивитюсеркаунтс](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | Отслеживайте динамику использования по количеству уникальных пользователей и типу проведенных в организации одноранговых сеансов (обмен мгновенными сообщениями, аудио, видео, общий доступ к приложениям и передача файлов в одноранговых сеансах). |
| [Получение количества минут](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Поток          | [Скипефорбусинесспиртопирактивитиминутекаунтс](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | Отслеживайте динамику использования по продолжительности (в минутах) и типу проведенных в организации одноранговых сеансов (аудио и видео). |
