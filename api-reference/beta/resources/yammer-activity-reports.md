---
title: Отчеты о действиях в Yammer
description: Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 8f1358c188b06953d7af180c2b7ad83b6183af35
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519059"
---
# <a name="yammer-activity-reports"></a>Отчеты о действиях в Yammer

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [яммерактивитюсердетаил](../resources/yammeractivityuserdetail.md) | Получение сведений о действиях в Yammer с разбивкой по пользователям. |
| [Получение количества действий](../api/reportroot-getyammeractivitycounts.md) | Stream          | [яммерактивитисуммари](../resources/yammeractivitysummary.md) | Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений. |
| [Получение количества пользователей](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [яммерактивитисуммари](../resources/yammeractivitysummary.md) | Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer. |
