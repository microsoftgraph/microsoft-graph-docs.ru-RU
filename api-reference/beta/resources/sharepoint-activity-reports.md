---
title: Отчеты о действиях в SharePoint
description: Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию на использование SharePoint, изучив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: b787fe2828519c6c21fa0c0b605ba9045c31ae84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520726"
---
# <a name="sharepoint-activity-reports"></a>Отчеты о действиях в SharePoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию на использование SharePoint, изучив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getsharepointactivityuserdetail.md) | Stream          | [шарепоинтактивитюсердетаил](../resources/sharepointactivityuserdetail.md) | Получите сведения о действиях в SharePoint с разбивкой по пользователям. |
| [Получение количества файлов](../api/reportroot-getsharepointactivityfilecounts.md) | Stream          | [ситеактивитисуммари](../resources/siteactivitysummary.md) | Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint. |
| [Получение количества пользователей](../api/reportroot-getsharepointactivityusercounts.md) | Stream          | [шарепоинтактивитюсеркаунтс](../resources/sharepointactivityusercounts.md) | Получение сведений о том, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период. |
| [Получение страниц](../api/reportroot-getsharepointactivitypages.md) | Stream          | [шарепоинтактивитипажес](../resources/sharepointactivitypages.md) | Получите количество уникальных страниц, посещенных пользователями. |
