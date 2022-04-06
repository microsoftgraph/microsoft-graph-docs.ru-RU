---
title: Microsoft 365 отчеты об использовании браузера
description: Используйте отчеты Microsoft 365 браузера, чтобы получить сведения об использовании браузеров (Microsoft Edge, устаревшая версия Microsoft Edge и Internet Explorer) в организации.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: 8b0a0865ecd051d241f41844004ee247e0a57b17
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64590020"
---
# <a name="microsoft-365-browser-usage-reports"></a>Microsoft 365 отчеты об использовании браузера

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте отчеты Microsoft 365 браузера, чтобы получить сведения об использовании браузеров (Microsoft Edge, устаревшая версия Microsoft Edge и Internet Explorer) в организации.

> **Примечание:** Сведения о различных представлениях отчетов и [именах см. в Microsoft 365 Отчеты в центре администрирования — использование браузера Майкрософт](/microsoft-365/admin/activity-reports/browser-usage-report).

## <a name="reports"></a>Отчеты

| Функция                                 | Тип возврата CSV | Тип возврата JSON                         | Описание                              |
| :--------------------------------------- | --------------- | ---------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getbrowseruserdetail.md ) | Stream          | Stream | Подробные сведения об использовании браузера для каждого пользователя.  |
| [Получение количества пользователей](../api/reportroot-getbrowserusercounts.md ) | Stream          | Stream |Получите тенденцию в количестве активных пользователей для каждого браузера. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getbrowserdistributionusercounts.md) | Stream          | Stream | Получите количество пользователей в браузере за выбранный период. |
