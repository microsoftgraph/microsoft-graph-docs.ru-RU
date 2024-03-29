---
title: Отчеты об использовании сайтов SharePoint
description: Эти отчеты позволяют получить общее представление об отдаче от SharePoint на основе общего количества хранимых на сайтах SharePoint файлов, количества активно используемых файлов и объема хранилища, занятого всеми этими сайтами. После этого вы можете посмотреть развернутые отчеты, чтобы выявить тенденции и особенности для каждого сайта.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 82ed0294ded68727fb373378871c07d08be74629
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545352"
---
# <a name="sharepoint-site-usage-reports"></a>Отчеты об использовании сайтов SharePoint

Пространство имен: microsoft.graph

Эти отчеты позволяют получить общее представление об отдаче от SharePoint на основе общего количества хранимых на сайтах SharePoint файлов, количества активно используемых файлов и объема хранилища, занятого всеми этими сайтами. После этого вы можете посмотреть развернутые отчеты, чтобы выявить тенденции и особенности для каждого сайта.

> **Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов - SharePoint использования сайта.](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)

## <a name="reports"></a>Отчеты

| Функция                                                     | Возвращаемый тип | Описание                                                  |
| :----------------------------------------------------------- | :---------- | :----------------------------------------------------------- |
| [Получение сведений о сайтах](../api/reportroot-getsharepointsiteusagedetail.md) | Поток      | Получите сведения об использовании сайтов SharePoint.                     |
| [Получение количества файлов](../api/reportroot-getsharepointsiteusagefilecounts.md) | Поток      | Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период. |
| [Получение количества сайтов](../api/reportroot-getsharepointsiteusagesitecounts.md) | Поток      | Получите тенденцию общего и активного количества сайтов в отчетный период. |
| [Получение занятого объема хранилища](../api/reportroot-getsharepointsiteusagestorage.md) | Поток      | Отслеживайте динамику выделенного и использованного объема хранилища за отчетный период. |
| [Получение количества страниц](../api/reportroot-getsharepointsiteusagepages.md) | Поток      | Узнайте, сколько страниц было просмотрено на всех сайтах.             |

