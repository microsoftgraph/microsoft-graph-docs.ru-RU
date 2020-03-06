---
title: Отчеты об активности в группах Office 365
description: Эти отчеты позволяют получить представление об активности в группах Office 365 в организации и узнать, сколько групп Office 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 57749ca15e4eaf4aad14f3f914426d861ea45eeb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534179"
---
# <a name="office-365-groups-activity-reports"></a>Отчеты об активности в группах Office 365

Пространство имен: microsoft.graph

Эти отчеты позволяют получить представление об активности в группах Office 365 в организации и узнать, сколько групп Office 365 создается и используется.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип | Описание                              |
| :--------------------------------------- | :-------------- |  ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getoffice365groupsactivitydetail.md) | Stream          | Получите сведения об активности в группах Office 365. |
| [Получение количества действий](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | Узнайте, сколько различных действий было в группах. |
| [Получение количества групп](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Stream          | Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день. |
| [Получение занятого объема хранилища](../api/reportroot-getoffice365groupsactivitystorage.md) | Поток          | Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп. |
| [Получение количества файлов](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Поток          | Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны. |
