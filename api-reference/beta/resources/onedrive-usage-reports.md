---
title: Отчеты об использовании OneDrive
description: Вы можете получить общее представление о значении, получаемом из OneDrive, с точки зрения общего количества файлов и хранилища, используемых во всех учетных записях OneDrive в организации. Вы также можете получить детализированные сведения для понимания того, каковы тенденции активных учетных записей OneDrive, с каким количеством файлов пользователи работали, какой объем хранилища используется. Он также предоставляет сведения об учетной записи OneDrive.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: e1c6128fab80fb0b7a0ec1391f4022bb625b2442
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2021
ms.locfileid: "49983211"
---
# <a name="onedrive-usage-reports"></a>Отчеты об использовании OneDrive

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить общее представление о значении, получаемом из OneDrive, с точки зрения общего количества файлов и хранилища, используемых во всех учетных записях OneDrive в организации. Вы также можете получить детализированные сведения для понимания того, каковы тенденции активных учетных записей OneDrive, с каким количеством файлов пользователи работали, какой объем хранилища используется. Он также предоставляет сведения об учетной записи OneDrive.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [отчетах Microsoft 365 об использовании OneDrive для бизнеса.](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | ---------------------------------------- | ---------------------------------------- |
| [Получение сведений об учетной записи](../api/reportroot-getonedriveusageaccountdetail.md) | Stream          | [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) | Получите сведения об использовании OneDrive с разбивкой по учетным записям. |
| [Получение количества учетных записей](../api/reportroot-getonedriveusageaccountcounts.md) | Stream          | [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) | Отслеживайте, как меняется количество активных сайтов OneDrive для бизнеса. Активным считается сайт, на котором пользователи просматривали, изменяли, добавляли, скачивали, синхронизировали файлы или делились ими. |
| [Получение количества файлов](../api/reportroot-getonedriveusagefilecounts.md) | Stream          | [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) | Получение общего количества файлов на всех сайтах и количества активных файлов. Файл считается активным, если он был сохранен, синхронизирован, изменен в указанный период или им поделились в указанный период. |
| [Получение занятого объема хранилища](../api/reportroot-getonedriveusagestorage.md) | Поток          | [siteUsageStorage](../resources/siteusagestorage.md) | Получение сведений о том, как меняется используемый объем хранилища в OneDrive для бизнеса. |


