---
title: Отчеты о действиях в OneDrive
description: Можно получить активности каждый пользователь с лицензии на использование OneDrive, посмотрев их взаимодействие с файлами на OneDrive. Он также помогает понять уровень совместной работы более подробное с отображением число общих файлов.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8e02e93d2266f302fb3f90ab47fe4853e34adee5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947199"
---
# <a name="onedrive-activity-reports"></a>Отчеты о действиях в OneDrive

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Можно получить активности каждый пользователь с лицензии на использование OneDrive, посмотрев их взаимодействие с файлами на OneDrive. Он также помогает понять уровень совместной работы более подробное с отображением число общих файлов.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Центре администрирования Office 365 — действия в OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | Получите сведения о действиях в OneDrive с разбивкой по пользователям. |
| [Получение количества пользователей](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Получение тренда в отношении количества активных пользователей OneDrive. |
| [Получение количества файлов](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive. |
