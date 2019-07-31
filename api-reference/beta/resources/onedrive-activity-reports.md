---
title: Отчеты о действиях в OneDrive
description: Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive. Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 710b2ed88deeec26846bb5afe7503808d8c470c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009442"
---
# <a name="onedrive-activity-reports"></a>Отчеты о действиях в OneDrive

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить сведения о действиях каждого пользователя, имеющего лицензию, для использования OneDrive, изучив их взаимодействие с файлами в OneDrive. Кроме того, вы можете ознакомиться с уровнем совместной работы, в котором показано количество файлов, к которым предоставлен общий доступ.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getonedriveactivityuserdetail.md) | Поток          | [Онедривеактивитюсердетаил](../resources/onedriveactivityuserdetail.md) | Получите сведения о действиях в OneDrive с разбивкой по пользователям. |
| [Получение количества пользователей](../api/reportroot-getonedriveactivityusercounts.md) | Поток          | [Ситеактивитисуммари](../resources/siteactivitysummary.md) | Получение тренда в отношении количества активных пользователей OneDrive. |
| [Получение количества файлов](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [Ситеактивитисуммари](../resources/siteactivitysummary.md) | Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive. |
