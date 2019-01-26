---
title: Отчеты об использовании OneDrive
description: Можно получить высокоуровневое представление значение, которое вы получаете из службы OneDrive в виде общее число файлов и хранения данных, используемых во всех учетных записей OneDrive в вашей организации. Вы также можете получить детализированные сведения для понимания того, каковы тенденции активных учетных записей OneDrive, с каким количеством файлов пользователи работали, какой объем хранилища используется. Он также дает на OneDrive сведения учетной записи.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1f899c3a60e1c0d66dd3b7e075bf0daf13de0b43
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574161"
---
# <a name="onedrive-usage-reports"></a>Отчеты об использовании OneDrive

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Можно получить высокоуровневое представление значение, которое вы получаете из службы OneDrive в виде общее число файлов и хранения данных, используемых во всех учетных записей OneDrive в вашей организации. Вы также можете получить детализированные сведения для понимания того, каковы тенденции активных учетных записей OneDrive, с каким количеством файлов пользователи работали, какой объем хранилища используется. Он также дает на OneDrive сведения учетной записи.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование OneDrive для бизнеса](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [Получение сведений об учетной записи](../api/reportroot-getonedriveusageaccountdetail.md) | Stream          | [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) | Получите сведения об использовании OneDrive с разбивкой по учетным записям. |
| [Получение количества учетных записей](../api/reportroot-getonedriveusageaccountcounts.md) | Stream          | [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) | Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, синхронизировали файлы или делились ими. |
| [Получение количества файлов](../api/reportroot-getonedriveusagefilecounts.md) | Stream          | [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) | Получение общего количества файлов на всех сайтах и количества активных файлов. Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период. |
| [Получение хранилища](../api/reportroot-getonedriveusagestorage.md) | Stream          | [siteUsageStorage](../resources/siteusagestorage.md) | Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onedrive-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
