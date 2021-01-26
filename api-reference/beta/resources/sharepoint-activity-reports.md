---
title: Отчеты о действиях в SharePoint
description: Вы можете получить действия каждого пользователя с лицензией на использование SharePoint, изусмотрив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 2e7b834f9bd4e1a440f0fd5167679ce0074668cd
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983787"
---
# <a name="sharepoint-activity-reports"></a>Отчеты о действиях в SharePoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить действия каждого пользователя с лицензией на использование SharePoint, изусмотрив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 : действия в SharePoint.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возвращаемого JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getsharepointactivityuserdetail.md) | Stream          | [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) | Получите сведения о действиях в SharePoint с разбивкой по пользователям. |
| [Получение количества файлов](../api/reportroot-getsharepointactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint. |
| [Получение количества пользователей](../api/reportroot-getsharepointactivityusercounts.md) | Stream          | [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) | Получение сведений о том, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период. |
| [Получение страниц](../api/reportroot-getsharepointactivitypages.md) | Stream          | [sharePointActivityPages](../resources/sharepointactivitypages.md) | Получите количество уникальных страниц, посещенных пользователями. |


