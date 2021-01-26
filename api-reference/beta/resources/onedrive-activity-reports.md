---
title: Отчеты о действиях в OneDrive
description: Вы можете получить действия каждого пользователя, у кого есть лицензия на использование OneDrive, изусмотрив их взаимодействие с файлами в OneDrive. Кроме того, это помогает понять, каков уровень совместной работы, показывая количество общих файлов.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7d0c069d2787b30f37e634757127b6141843a9ed
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983603"
---
# <a name="onedrive-activity-reports"></a>Отчеты о действиях в OneDrive

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить действия каждого пользователя, у кого есть лицензия на использование OneDrive, изусмотрив их взаимодействие с файлами в OneDrive. Кроме того, это помогает понять, каков уровень совместной работы, показывая количество общих файлов.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365: действия в OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | Получите сведения о действиях в OneDrive с разбивкой по пользователям. |
| [Получение количества пользователей](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Получение тренда в отношении количества активных пользователей OneDrive. |
| [Получение количества файлов](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive. |


