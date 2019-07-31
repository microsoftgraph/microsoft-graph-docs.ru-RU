---
title: Отчеты об активности в группах Office 365
description: Вы можете получить представление об активности групп Office 365 в Организации и узнать, сколько групп Office 365 создается и используется.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 49ebf19b1c8cc00f6edfc62b1056412c45bbe2e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009547"
---
# <a name="office-365-groups-activity-reports"></a>Отчеты об активности в группах Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить представление об активности групп Office 365 в Организации и узнать, сколько групп Office 365 создается и используется.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getoffice365groupsactivitydetail.md) | Поток          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | Получите сведения об активности в группах Office 365. |
| [Получение количества действий](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | Узнайте, сколько различных действий было в группах. |
| [Получение количества групп](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Поток          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день. |
| [Получение занятого объема хранилища](../api/reportroot-getoffice365groupsactivitystorage.md) | Поток          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп. |
| [Получение количества файлов](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны. |
