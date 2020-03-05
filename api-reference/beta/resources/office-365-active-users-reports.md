---
title: Отчеты об активных пользователях Office 365
description: Вы можете использовать отчет об активных пользователях Office 365, чтобы узнать, сколько лицензий используется сотрудниками вашей организации, а также подробно раскрывающийся список для получения сведений о том, какие пользователи используют продукты. Этот отчет поможет администраторам выяснить, какие продукты используются редко, или определить пользователей, которым могут понадобиться дополнительное обучение и сведения.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: conceptualPageType
ms.openlocfilehash: 5937a855328224a319cdd148da936517b63171c5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522507"
---
# <a name="office-365-active-users-reports"></a>Отчеты об активных пользователях Office 365

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Вы можете использовать отчет об активных пользователях Office 365, чтобы узнать, сколько лицензий используется сотрудниками вашей организации, а также подробно раскрывающийся список для получения сведений о том, какие пользователи используют продукты. Этот отчет поможет администраторам выяснить, какие продукты используются редко, или определить пользователей, которым могут понадобиться дополнительное обучение и сведения.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Отчеты
| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Получите сведения об активных пользователях Office 365. |
| [Получение количества пользователей](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | Узнайте, сколько активных пользователей в день было у каждого продукта в отчетный период. |
| [Получение количества пользователей по службам](../api/reportroot-getoffice365servicesusercounts.md) | Поток          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | Узнайте, сколько пользователей были активны и неактивны в каждой службе. |
