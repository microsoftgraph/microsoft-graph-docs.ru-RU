---
title: Отчеты о действиях в SharePoint
description: Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на SharePoint, в отчетах о действиях с файлами в SharePoint. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 4c67655dce0bbbe834051a536cb6917111c53fe0729f5430e0558886529edd7a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54231476"
---
# <a name="sharepoint-activity-reports"></a>Отчеты о действиях в SharePoint

Пространство имен: microsoft.graph

Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на SharePoint, в отчетах о действиях с файлами в SharePoint. Кроме того, вы можете отслеживать уровень взаимодействия, просматривая количество файлов, которыми поделились.

> **Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — SharePoint действий.](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getsharepointactivityuserdetail.md) | Stream      | Получите сведения о действиях в SharePoint с разбивкой по пользователям. |
| [Получение количества файлов](../api/reportroot-getsharepointactivityfilecounts.md) | Stream      | Получите количество уникальных пользователей с лицензиями, которые работали с файлами, хранящимися на сайтах SharePoint. |
| [Получение количества пользователей](../api/reportroot-getsharepointactivityusercounts.md) | Stream      | Получение сведений о том, как меняется количество активных пользователей. Пользователь считается активным, если он выполнил действие с файлом (сохранение, синхронизация, изменение или предоставление общего доступа) или посетил страницу в указанный период. |
| [Получение страниц](../api/reportroot-getsharepointactivitypages.md) | Stream      | Получите количество уникальных страниц, посещенных пользователями. |

