---
title: Отчеты о действиях в Yammer
description: Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: efdb4ba603be33f18cd66529edd724f6e1a3798d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35963833"
---
# <a name="yammer-activity-reports"></a>Отчеты о действиях в Yammer

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете оценить уровень задействования Организации в Yammer, указав количество действий, создаваемых в Организации, и количество уникальных пользователей, которые размещает, например, и прочитают сообщения в Yammer.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в Yammer](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getyammeractivityuserdetail.md) | Поток          | [Яммерактивитюсердетаил](../resources/yammeractivityuserdetail.md) | Получение сведений о действиях в Yammer с разбивкой по пользователям. |
| [Получение количества действий](../api/reportroot-getyammeractivitycounts.md) | Stream          | [Яммерактивитисуммари](../resources/yammeractivitysummary.md) | Отследите динамику использования Yammer в организации по количеству опубликованных, прочитанных и понравившихся сообщений. |
| [Получение количества пользователей](../api/reportroot-getyammeractivityusercounts.md) | Поток          | [Яммерактивитисуммари](../resources/yammeractivitysummary.md) | Отследите динамику по количеству уникальных пользователей, которые опубликовали, прочитали и оценили сообщения Yammer. |
