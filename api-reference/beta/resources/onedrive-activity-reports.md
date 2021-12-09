---
title: Отчеты о действиях в OneDrive
description: Вы можете получить действие каждого пользователя, лицензированного на использование OneDrive, OneDrive их взаимодействия с файлами в OneDrive. Это также помогает вам понять уровень совместной работы, показывая количество общих файлов.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 188cb9ff8fc6750a1beb4177a82e3c1135da20bb
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61390796"
---
# <a name="onedrive-activity-reports"></a>Отчеты о действиях в OneDrive

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить действие каждого пользователя, лицензированного на использование OneDrive, OneDrive их взаимодействия с файлами в OneDrive. Это также помогает вам понять уровень совместной работы, показывая количество общих файлов.

> **Примечание:** Подробные сведения о различных представлениях и именах [отчетов см. в Microsoft 365 отчетов — OneDrive для бизнеса действий.](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)

## <a name="reports"></a>Отчеты

| Функция                                                     | Тип возврата CSV | Тип возврата JSON | Описание                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Получение сведений о пользователях](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | Stream           | Получите сведения о действиях в OneDrive с разбивкой по пользователям.                 |
| [Получение количества пользователей](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | Stream           | Получение тренда в отношении количества активных пользователей OneDrive.        |
| [Получение количества файлов](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | Stream           | Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive. |


