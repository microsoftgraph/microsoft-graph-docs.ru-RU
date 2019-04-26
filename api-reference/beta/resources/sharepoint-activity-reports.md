---
title: Отчеты о действиях в SharePoint
description: Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию на использование SharePoint, изучив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: cfe8c698533b46d4edbbb724dc5fb993cc85cfdb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343172"
---
# <a name="sharepoint-activity-reports"></a>Отчеты о действиях в SharePoint

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию на использование SharePoint, изучив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: действия в SharePoint](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getsharepointactivityuserdetail.md) | Stream          | [Шарепоинтактивитюсердетаил](../resources/sharepointactivityuserdetail.md) | Получите сведения о действиях в SharePoint с разбивкой по пользователям. |
| [Получение количества файлов](../api/reportroot-getsharepointactivityfilecounts.md) | Stream          | [Ситеактивитисуммари](../resources/siteactivitysummary.md) | Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint. |
| [Получение количества пользователей](../api/reportroot-getsharepointactivityusercounts.md) | Stream          | [Шарепоинтактивитюсеркаунтс](../resources/sharepointactivityusercounts.md) | Получение сведений о том, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период. |
| [Получение страниц](../api/reportroot-getsharepointactivitypages.md) | Stream          | [Шарепоинтактивитипажес](../resources/sharepointactivitypages.md) | Получите количество уникальных страниц, посещенных пользователями. |
