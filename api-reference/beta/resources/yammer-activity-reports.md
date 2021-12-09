---
title: Отчеты о действиях в Yammer
description: Вы можете понять уровень взаимодействия вашей организации с Yammer по количеству активностей, генерируемых в организации, и количеству уникальных пользователей, которые вывешиют, любят и читают сообщения в Yammer.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 5d157217c94d35450929745a4f5bf0989bb2bf49
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390831"
---
# <a name="yammer-activity-reports"></a>Отчеты о действиях в Yammer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете понять уровень взаимодействия вашей организации с Yammer по количеству активностей, генерируемых в организации, и количеству уникальных пользователей, которые вывешиют, любят и читают сообщения в Yammer.

> **Примечание:** Подробные сведения о различных представлениях и именах [отчетов см. в Microsoft 365 отчеты - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Отчеты

| Функция                                                     | Тип возврата CSV | Тип возврата JSON | Описание                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Получение сведений о пользователях](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | Stream           | Получение сведений о действиях в Yammer с разбивкой по пользователям.                   |
| [Получение количества действий](../api/reportroot-getyammeractivitycounts.md) | Stream          | Stream           | Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений. |
| [Получение количества пользователей](../api/reportroot-getyammeractivityusercounts.md) | Stream          | Stream           | Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer. |


