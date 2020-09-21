---
title: Отчеты об активности в группах Microsoft 365
description: Отчеты об активности групп можно использовать для получения сведений о действиях в группах Microsoft 365 в Организации и о количестве создаваемых и используемых групп Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 52bb3cb71837f049cada3970bdd0faa710f38844
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965423"
---
# <a name="microsoft-365-groups-activity-reports"></a>Отчеты об активности в группах Microsoft 365

Пространство имен: microsoft.graph

Отчеты об активности групп можно использовать для получения сведений о действиях в группах Microsoft 365 в Организации и о количестве создаваемых и используемых групп Microsoft 365.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getoffice365groupsactivitydetail.md) | Поток          | Получение сведений о действиях в группах Microsoft 365, сгруппированных по группам. |
| [Получение количества действий](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | Узнайте, сколько различных действий было в группах. |
| [Получение количества групп](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Поток          | Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день. |
| [Получение занятого объема хранилища](../api/reportroot-getoffice365groupsactivitystorage.md) | Поток          | Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп. |
| [Получение количества файлов](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | Получите общее количество файлов и их количество, которое было активно на всех сайтах группы, связанных с группой Microsoft 365. |

