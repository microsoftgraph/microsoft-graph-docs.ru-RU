---
title: Отчеты об использовании сайтов SharePoint
description: Можно получить высокоуровневое представление значение, которое вы получаете из SharePoint с точки зрения общее число файлов, которые пользователи хранят на сайтах SharePoint, сколько файлов используется и хранения данных, использования по всем сайтам. Затем можно перейти в отчет об использовании сайта SharePoint для понимания тенденции и на уровне сведений о среде для всех сайтов.
localization_priority: Normal
ms.openlocfilehash: 287abafdf279b2a249481ebc4445bfcd980ebc76
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856143"
---
# <a name="sharepoint-site-usage-reports"></a>Отчеты об использовании сайтов SharePoint

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Можно получить высокоуровневое представление значение, которое вы получаете из SharePoint с точки зрения общее число файлов, которые пользователи хранят на сайтах SharePoint, сколько файлов используется и хранения данных, использования по всем сайтам. Затем можно перейти в отчет об использовании сайта SharePoint для понимания тенденции и на уровне сведений о среде для всех сайтов.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о сайтах](../api/reportroot-getsharepointsiteusagedetail.md) | Поток          | [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) | Получите сведения об использовании сайтов SharePoint. |
| [Получение количества файлов](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream          | [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) | Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период. |
| [Получение количества сайтов](../api/reportroot-getsharepointsiteusagesitecounts.md) | Поток          | [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) | Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период. |
| [Получение занятого объема хранилища](../api/reportroot-getsharepointsiteusagestorage.md) | Stream          | [siteUsageStorage](../resources/siteusagestorage.md) | Отслеживайте динамику выделенного и использованного объема хранилища за отчетный период. |
| [Получение количества страниц](../api/reportroot-getsharepointsiteusagepages.md) | Stream          | [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) | Узнайте, сколько страниц было просмотрено на всех сайтах. |
