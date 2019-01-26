---
title: Отчеты об активных пользователях Office 365
description: Отчет активных пользователей Office 365 используется для получения числа лицензий продукта используются с пользователями в организации и детализации для получения сведений о том, какие пользователи используют какие продукты. В этом отчете может помочь администраторам определение использования продуктов или пользователей, которым могут понадобиться дополнительные учебные курсы или сведения.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 638550fbc44acd0154a2dab5c062e2061fa9c582
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571767"
---
# <a name="office-365-active-users-reports"></a>Отчеты об активных пользователях Office 365

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Отчет активных пользователей Office 365 используется для получения числа лицензий продукта используются с пользователями в организации и детализации для получения сведений о том, какие пользователи используют какие продукты. В этом отчете может помочь администраторам определение использования продуктов или пользователей, которым могут понадобиться дополнительные учебные курсы или сведения.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в [этой статье](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Отчеты
| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Получите сведения об активных пользователях Office 365. |
| [Получение количества пользователей](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | Узнайте, сколько активных пользователей в день было у каждого продукта в отчетный период. |
| [Получение количества пользователей по службам](../api/reportroot-getoffice365servicesusercounts.md) | Поток          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | Узнайте, сколько пользователей были активны и неактивны в каждой службе. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-active-users-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
