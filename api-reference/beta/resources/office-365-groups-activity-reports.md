---
title: Отчеты об активности в группах Office 365
description: Можно воспользоваться сведениями в действие группы Office 365 в вашей организации и видеть, сколько групп Office 365 создаются и используются.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 8db142bcc7ae283df41dd6809ab97e81c996c10a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971188"
---
# <a name="office-365-groups-activity-reports"></a>Отчеты об активности в группах Office 365

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Можно воспользоваться сведениями в действие группы Office 365 в вашей организации и видеть, сколько групп Office 365 создаются и используются.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о группах](../api/reportroot-getoffice365groupsactivitydetail.md) | Поток          | [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) | Получите сведения об активности в группах Office 365. |
| [Получение количества действий](../api/reportroot-getoffice365groupsactivitycounts.md) | Stream          | [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) | Узнайте, сколько различных действий было в группах. |
| [Получение количества групп](../api/reportroot-getoffice365groupsactivitygroupcounts.md) | Поток          | [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) | Узнайте, сколько всего групп в организации и сколько из них были активны на основе цепочек сообщений, публикаций в Yammer и действий с файлами SharePoint за день. |
| [Получение занятого объема хранилища](../api/reportroot-getoffice365groupsactivitystorage.md) | Stream          | [office365GroupsActivityStorage](../resources/office365groupsactivitystorage.md) | Узнайте, сколько места в хранилище занято всеми почтовыми ящиками и сайтами групп. |
| [Получение количества файлов](../api/reportroot-getoffice365groupsactivityfilecounts.md) | Stream          | [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) | Узнайте, сколько всего файлов на всех связанных с группой Office 365 сайтах и сколько из них были активны. |
