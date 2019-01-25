---
title: Отчеты об использовании устройств Microsoft Teams
description: 'Использование отчетов об использовании устройства группами Майкрософт для получения понять использование устройства группами Майкрософт в вашей организации. '
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: f9240f6cb310ada94f1a6694efb0da6cd691dc13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519908"
---
# <a name="microsoft-teams-device-usage-reports"></a>Отчеты об использовании устройств Microsoft Teams

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Использование отчетов об использовании устройства группами Майкрософт для получения понять использование устройства группами Майкрософт в вашей организации. 

## <a name="methods"></a>Методы

| Метод                                   | Возвращаемый тип                              | Описание                              |
| :--------------------------------------- | :--------------------------------------- | :--------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | Получение сведений об использовании устройств Microsoft Teams отдельными пользователями. |
| [Получение количества пользователей](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Получение сведений о количестве уникальных пользователей в день по типам устройств. |
| [Получение распределенного количества пользователей](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Получение количества уникальных пользователей по типам устройств за выбранный период времени. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/microsoft-teams-device-usage-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
