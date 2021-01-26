---
title: Отчеты об использовании сайтов SharePoint
description: Вы можете получить общее представление о значении, которое вы получаете от SharePoint, с точки зрения общего количества файлов, которые пользователи хранят на сайтах SharePoint, количества активно используемых файлов и объема хранилища, используемого на всех этих сайтах. Затем вы можете детализировать отчет об использовании сайта SharePoint, чтобы выявить тенденции и получить сведения об использовании на уровне сайта.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: c61665eb86e9bf903c003f816f7edde949f5fcdc
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982490"
---
# <a name="sharepoint-site-usage-reports"></a>Отчеты об использовании сайтов SharePoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить общее представление о значении, получаемом из SharePoint, с точки зрения общего количества файлов, которые пользователи хранят на сайтах SharePoint, количества активно используемых файлов и объема хранилища, используемого на всех этих сайтах. Затем вы можете детализировать отчет об использовании сайта SharePoint, чтобы выявить тенденции и получить сведения об использовании на уровне сайта.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании сайта SharePoint.](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о сайтах](../api/reportroot-getsharepointsiteusagedetail.md) | Поток          | [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) | Получите сведения об использовании сайтов SharePoint. |
| [Получение количества файлов](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream          | [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) | Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период. |
| [Получение количества сайтов](../api/reportroot-getsharepointsiteusagesitecounts.md) | Поток          | [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) | Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период. |
| [Получение занятого объема хранилища](../api/reportroot-getsharepointsiteusagestorage.md) | Поток          | [siteUsageStorage](../resources/siteusagestorage.md) | Отслеживайте динамику выделенного и использованного объема хранилища за отчетный период. |
| [Получение количества страниц](../api/reportroot-getsharepointsiteusagepages.md) | Stream          | [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) | Узнайте, сколько страниц было просмотрено на всех сайтах. |


