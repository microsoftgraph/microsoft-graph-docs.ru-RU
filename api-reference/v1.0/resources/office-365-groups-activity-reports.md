---
title: Отчеты об активности групп Microsoft 365
description: Вы можете использовать отчеты о действиях в группах, чтобы получить представление об активности групп Microsoft 365 в организации и узнать, сколько групп Microsoft 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7470eff43c2c77a63206cf24e0484360bf3371b6
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49980999"
---
# <a name="microsoft-365-groups-activity-reports"></a>Отчеты об активности групп Microsoft 365

Пространство имен: microsoft.graph

Вы можете использовать отчеты о действиях в группах, чтобы получить представление об активности групп Microsoft 365 в организации и узнать, сколько групп Microsoft 365 создается и используется.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 — группы Microsoft 365.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getoffice365groupsactivitydetail.md) | Поток          | Получите сведения об активности групп Microsoft 365 по группам. |
| [Получение количества действий](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | Узнайте, сколько различных действий было в группах. |
| [Получение количества групп](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Поток          | Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день. |
| [Получение занятого объема хранилища](../api/reportroot-getoffice365groupsactivitystorage.md) | Поток          | Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп. |
| [Получение количества файлов](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | Получите общее количество файлов и их количество на всех сайтах групп, связанных с группой Microsoft 365. |

