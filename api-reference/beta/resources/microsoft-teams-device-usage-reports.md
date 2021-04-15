---
title: Отчеты об использовании устройств Microsoft Teams
description: 'Используйте отчеты об использовании устройств Microsoft Teams, чтобы получить сведения об использовании устройств Microsoft Teams в вашей организации. '
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: conceptualPageType
ms.openlocfilehash: b9a4d2ab3034281970a3e342aa0a2d78e53678e5
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766114"
---
# <a name="microsoft-teams-device-usage-reports"></a>Отчеты об использовании устройств Microsoft Teams

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используйте отчеты об использовании устройств Microsoft Teams, чтобы получить сведения об использовании устройств Microsoft Teams в вашей организации. 

## <a name="methods"></a>Методы

| Метод                                                       | Возвращаемый тип                                                  | Описание                                                  |
| :----------------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getteamsdeviceusageuserdetail.md) | [teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md) | Получение сведений об использовании устройств Microsoft Teams отдельными пользователями.      |
| [Получение количества пользователей](../api/reportroot-getteamsdeviceusageusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Получите количество ежедневных уникальных пользователей Microsoft Teams, лицензированных по типу устройства. |
| [Общее количество пользователей](../api/reportroot-getteamsdeviceusagetotalusercounts.md) | [teamsDeviceUsageUserCounts](../resources/teamsdeviceusageusercounts.md) | Получите число ежедневных уникальных пользователей Microsoft Teams, лицензированных или не лицензированных по типу устройства. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getteamsdeviceusagedistributionusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Получите количество уникальных лицензированных пользователей Microsoft Teams по типу устройства за выбранный период времени. |
| [Общее количество пользователей в распределении](../api/reportroot-getteamsdeviceusagedistributiontotalusercounts.md) | [teamsDeviceUsagedistributionUserCounts](../resources/teamsdeviceusagedistributionusercounts.md) | Получите число уникальных пользователей Microsoft Teams, лицензированных или не лицензированных по типу устройства за выбранный период времени. |


