---
title: Отчеты об использовании сайтов SharePoint
description: Вы можете получить высокоуровневое представление значения, получаемого из SharePoint, в терминах общего числа файлов, которые пользователи хранят на сайтах SharePoint, сколько файлов активно используется, а хранилище потребляется на всех этих сайтах. Затем вы можете детализировать отчет об использовании сайта SharePoint, чтобы выявить тенденции и получить сведения об использовании на уровне сайта.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: f9e12156fdb515210b82b31db0c04a3393821197
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895554"
---
# <a name="sharepoint-site-usage-reports"></a>Отчеты об использовании сайтов SharePoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить высокоуровневое представление значения, получаемого из SharePoint, в терминах общего числа файлов, которые пользователи хранят на сайтах SharePoint, сколько файлов активно используется, а хранилище потребляется на всех этих сайтах. Затем вы можете детализировать отчет об использовании сайта SharePoint, чтобы выявить тенденции и получить сведения об использовании на уровне сайта.

> **Примечание:** Сведения о различных представлениях и именах отчетов можно найти в [статье Microsoft 365 Reports-SharePoint site Usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о сайтах](../api/reportroot-getsharepointsiteusagedetail.md) | Stream          | [шарепоинтситеусажедетаил](../resources/sharepointsiteusagedetail.md) | Получите сведения об использовании сайтов SharePoint. |
| [Получение количества файлов](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream          | [шарепоинтситеусажефилекаунтс](../resources/sharepointsiteusagefilecounts.md) | Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период. |
| [Получение количества сайтов](../api/reportroot-getsharepointsiteusagesitecounts.md) | Stream          | [шарепоинтситеусажеситекаунтс](../resources/sharepointsiteusagesitecounts.md) | Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период. |
| [Получение занятого объема хранилища](../api/reportroot-getsharepointsiteusagestorage.md) | Поток          | [ситеусажестораже](../resources/siteusagestorage.md) | Отслеживайте динамику выделенного и использованного объема хранилища за отчетный период. |
| [Получение количества страниц](../api/reportroot-getsharepointsiteusagepages.md) | Stream          | [шарепоинтситеусажепажес](../resources/sharepointsiteusagepages.md) | Узнайте, сколько страниц было просмотрено на всех сайтах. |
