---
title: Отчеты о работе со Skype для бизнеса
description: Вы можете получить подробные сведения об активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 7ab7955de5c5bf331d954a3dc553018a87dbac44
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997671"
---
# <a name="skype-for-business-activity-reports"></a>Отчеты о работе со Skype для бизнеса

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить подробные сведения об активности в Организации. Эти данные могут пригодиться при проведении анализа, планировании и принятии других бизнес-решений.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье Microsoft 365 Reports-Activity for Skype для бизнеса](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [скипефорбусинессактивитюсердетаил](../resources/skypeforbusinessactivityuserdetail.md) | Получите сведения о действиях пользователей в Skype для бизнеса. |
| [Получение количества действий](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | [скипефорбусинессактивитикаунтс](../resources/skypeforbusinessactivitycounts.md) | Отслеживайте, как меняется количество организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |
| [Получение количества пользователей](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | [скипефорбусинессактивитюсеркаунтс](../resources/skypeforbusinessactivityusercounts.md) | Отслеживайте, как меняется количество уникальных организаторов и участников конференций, проводимых в вашей организации через Skype для бизнеса. Отчет также включает количество одноранговых сеансов. |


