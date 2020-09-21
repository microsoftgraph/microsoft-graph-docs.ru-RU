---
title: Отчеты о действиях в OneDrive
description: Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на OneDrive, в отчетах действий с файлами в OneDrive. Эти отчеты позволят оценить уровень взаимодействия благодаря данным о количестве файлов, к которым предоставлен общий доступ.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: d06dc9aba906f9d8e423388a39faf3ccfe414bf1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965465"
---
# <a name="onedrive-activity-reports"></a>Отчеты о действиях в OneDrive

Пространство имен: microsoft.graph

Просматривайте сведения о действиях каждого пользователя, имеющего лицензию на OneDrive, в отчетах действий с файлами в OneDrive. Эти отчеты позволят оценить уровень взаимодействия благодаря данным о количестве файлов, к которым предоставлен общий доступ.

> **Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-Activity for OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getonedriveactivityuserdetail.md) | Stream      | Получите сведения о действиях в OneDrive с разбивкой по пользователям. |
| [Получение количества пользователей](../api/reportroot-getonedriveactivityusercounts.md) | Stream      | Получение тренда в отношении количества активных пользователей OneDrive. |
| [Получение количества файлов](../api/reportroot-getonedriveactivityfilecounts.md) | Stream      | Получение количества уникальных пользователей с лицензией, которые работали с файлами в любой учетной записи OneDrive. |


