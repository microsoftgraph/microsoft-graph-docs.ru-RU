---
title: Отчеты об использовании сайтов SharePoint
description: Вы можете получить представление на высоком уровне о значении, которое вы получаете от SharePoint с точки зрения общего количества файлов, которые пользователи хранят на SharePoint сайтах, сколько файлов активно используется, и хранения, потребляемого на всех этих сайтах. Затем вы можете детализировать отчет об использовании сайта SharePoint, чтобы выявить тенденции и получить сведения об использовании на уровне сайта для всех сайтов.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 7d54fc29b73edac1039f041d4a3dd1a2a2bcafb8
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2021
ms.locfileid: "61545376"
---
# <a name="sharepoint-site-usage-reports"></a>Отчеты об использовании сайтов SharePoint

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете получить представление на высоком уровне о значении, которое вы получаете от SharePoint с точки зрения общего количества файлов, которые пользователи хранят на SharePoint сайтах, сколько файлов активно используется, и хранения, потребляемого на всех этих сайтах. Затем вы можете детализировать отчет об использовании сайта SharePoint, чтобы выявить тенденции и получить сведения об использовании на уровне сайта для всех сайтов.

> **Примечание:** Подробные сведения о различных представлениях отчетов и [именах см. в Microsoft 365 отчетов - SharePoint использования сайта.](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)

## <a name="reports"></a>Отчеты

| Функция                                                     | Тип возврата CSV | Тип возврата JSON | Описание                                                  |
| :----------------------------------------------------------- | :-------------- | :--------------- | ------------------------------------------------------------ |
| [Получение сведений о сайтах](../api/reportroot-getsharepointsiteusagedetail.md) | Поток          | Поток           | Получите сведения об использовании сайтов SharePoint.                     |
| [Получение количества файлов](../api/reportroot-getsharepointsiteusagefilecounts.md) | Stream          | Поток           | Узнайте, сколько всего файлов на всех сайтах и сколько из них активны. Файл (пользователь или система) считается активным, если он был сохранен, синхронизирован, изменен или отправлен в указанный период. |
| [Получение количества сайтов](../api/reportroot-getsharepointsiteusagesitecounts.md) | Поток          | Stream           | Получите тенденцию общего и активного количества сайтов в отчетный период. |
| [Получение занятого объема хранилища](../api/reportroot-getsharepointsiteusagestorage.md) | Поток          | Поток           | Отслеживайте динамику выделенного и использованного объема хранилища за отчетный период. |
| [Получение количества страниц](../api/reportroot-getsharepointsiteusagepages.md) | Stream          | Поток           | Узнайте, сколько страниц было просмотрено на всех сайтах.             |


