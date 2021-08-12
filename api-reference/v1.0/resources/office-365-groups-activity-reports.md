---
title: Microsoft 365 отчеты о деятельности групп
description: Вы можете использовать отчеты о действиях Groups, чтобы получить представление о деятельности Microsoft 365 групп в организации и узнать, сколько Microsoft 365 групп создается и используется.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 814b66d419fea4d06cbf16158298fac81c644ba794f3c0f85a8c32e2996d776f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174922"
---
# <a name="microsoft-365-groups-activity-reports"></a>Microsoft 365 отчеты о деятельности групп

Пространство имен: microsoft.graph

Вы можете использовать отчеты о действиях Groups, чтобы получить представление о деятельности Microsoft 365 групп в организации и узнать, сколько Microsoft 365 групп создается и используется.

> **Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов — Microsoft 365 групп.](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getoffice365groupsactivitydetail.md) | Поток          | Сведения о Microsoft 365 групп по группам. |
| [Получение количества действий](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | Узнайте, сколько различных действий было в группах. |
| [Получение количества групп](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Поток          | Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день. |
| [Получение занятого объема хранилища](../api/reportroot-getoffice365groupsactivitystorage.md) | Поток          | Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп. |
| [Получение количества файлов](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | Получите общее количество файлов и их количество на всех сайтах группы, связанных с Microsoft 365 группой. |

