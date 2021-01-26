---
title: Отчеты о действиях в Yammer
description: Вы можете понять уровень взаимодействия вашей организации с Yammer по уровню активности в организации и количеству уникальных пользователей, которые читают и читают сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: c0009949b5eb429f15155059768365b201078134
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982469"
---
# <a name="yammer-activity-reports"></a>Отчеты о действиях в Yammer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете понять уровень взаимодействия вашей организации с Yammer по уровню активности в организации и количеству уникальных пользователей, которые читают и читают сообщения в Yammer.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 - Yammer Activity.](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | Получение сведений о действиях в Yammer с разбивкой по пользователям. |
| [Получение количества действий](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений. |
| [Получение количества пользователей](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer. |


