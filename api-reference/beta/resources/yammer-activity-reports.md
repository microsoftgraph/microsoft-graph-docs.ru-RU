---
title: Отчеты о действиях в Yammer
description: Вы понимаете обязательства вашей организации с помощью Yammer с активности создается в организации и число уникальных пользователей, публиковать, такие как и читать сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 69c155df86cfe772e0c065bec0297a83fb7f3a8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912038"
---
# <a name="yammer-activity-reports"></a>Отчеты о действиях в Yammer

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается. Эти интерфейсы API в Китае Microsoft Graph обслуживается 21Vianet не поддерживаются.

Вы понимаете обязательства вашей организации с помощью Yammer с активности создается в организации и число уникальных пользователей, публиковать, такие как и читать сообщения в Yammer.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | Получение сведений о действиях в Yammer с разбивкой по пользователям. |
| [Получение количества действий](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений. |
| [Получение количества пользователей](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer. |
