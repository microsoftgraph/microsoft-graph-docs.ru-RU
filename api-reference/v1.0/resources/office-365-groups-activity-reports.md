---
title: Отчеты об активности в группах Microsoft 365
description: Отчеты об активности групп можно использовать для получения сведений о действиях в группах Microsoft 365 в Организации и о количестве создаваемых и используемых групп Microsoft 365.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 0cd0dfc07813714d376a38125835917c712e7ebe
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898158"
---
# <a name="microsoft-365-groups-activity-reports"></a>Отчеты об активности в группах Microsoft 365

Пространство имен: microsoft.graph

Отчеты об активности групп можно использовать для получения сведений о действиях в группах Microsoft 365 в Организации и о количестве создаваемых и используемых групп Microsoft 365.

> **Примечание:** Сведения о различных представлениях отчетов и их именах можно найти в [статье microsoft 365 Reports — microsoft 365 Groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | Получение сведений о действиях в группах Microsoft 365, сгруппированных по группам. |
| [Получение количества действий](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | Узнайте, сколько различных действий было в группах. |
| [Получение количества групп](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Поток          | Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день. |
| [Получение занятого объема хранилища](../api/reportroot-getoffice365groupsactivitystorage.md) | Поток          | Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп. |
| [Получение количества файлов](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | Получите общее количество файлов и их количество, которое было активно на всех сайтах группы, связанных с группой Microsoft 365. |
