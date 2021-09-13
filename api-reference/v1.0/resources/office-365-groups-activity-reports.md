---
title: Microsoft 365 отчеты о деятельности групп
description: Вы можете использовать отчеты о действиях Groups, чтобы получить представление о деятельности Microsoft 365 групп в организации и узнать, сколько Microsoft 365 групп создается и используется.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 487b8a6693a077f59fd3202c563a56fc8ffce0dc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084246"
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

