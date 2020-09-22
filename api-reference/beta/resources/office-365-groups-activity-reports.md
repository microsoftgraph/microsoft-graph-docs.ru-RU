---
title: Отчеты об активности в группах Microsoft 365
description: Вы можете получить подробные сведения о действиях в группах Microsoft 365 в Организации и узнать, сколько групп Microsoft 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: fbe657da65955410a7ea38e3aafdef9d1d853e09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021240"
---
# <a name="microsoft-365-groups-activity-reports"></a>Отчеты об активности в группах Microsoft 365

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить подробные сведения о действиях в группах Microsoft 365 в Организации и узнать, сколько групп Microsoft 365 создается и используется.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getoffice365groupsactivitydetail.md) | Поток          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | Получение сведений о действиях в группах Microsoft 365, сгруппированных по группам. |
| [Получение количества действий](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | Узнайте, сколько различных действий было в группах. |
| [Получение количества групп](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Поток          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день. |
| [Получение занятого объема хранилища](../api/reportroot-getoffice365groupsactivitystorage.md) | Поток          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп. |
| [Получение количества файлов](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Получите общее количество файлов и их количество, которое было активно на всех сайтах группы, связанных с группой Microsoft 365. |


