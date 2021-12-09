---
title: Отчеты о действиях в SharePoint
description: Вы можете получить действие каждого пользователя, лицензированного на использование SharePoint, изумив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b1fe7edaea8e7d2d6cc5a0da83dc7fd739a77d6e
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391083"
---
# <a name="sharepoint-activity-reports"></a>Отчеты о действиях в SharePoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить действие каждого пользователя, лицензированного на использование SharePoint, изумив их взаимодействие с файлами. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.

> **Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — SharePoint действий.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)

## <a name="reports"></a>Отчеты

| Функция                                                     | Тип возврата CSV | Тип возврата JSON | Описание                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Получение сведений о пользователях](../api/reportroot-getsharepointactivityuserdetail.md) | Stream          | Stream           | Получите сведения о действиях в SharePoint с разбивкой по пользователям.               |
| [Получение количества файлов](../api/reportroot-getsharepointactivityfilecounts.md) | Stream          | Stream           | Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint. |
| [Получение количества пользователей](../api/reportroot-getsharepointactivityusercounts.md) | Stream          | Stream           | Получение сведений о том, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период. |
| [Получение страниц](../api/reportroot-getsharepointactivitypages.md) | Stream          | Stream           | Получите количество уникальных страниц, посещенных пользователями.             |


