---
title: Отчеты об использовании устройств с Yammer
description: Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a68b1decf0690a07db07c880cec25a1bf2c01cfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991960"
---
# <a name="yammer-device-usage-reports"></a>Отчеты об использовании устройств с Yammer

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается. Эти интерфейсы API в Китае Microsoft Graph обслуживается 21Vianet не поддерживаются.

Отчеты об использовании устройств с Yammer содержат сведения о том, какие устройства с Yammer есть у пользователей. Вы можете просматривать сведения о количестве пользователей за указанный период с разбивкой по типам устройств и по пользователям.

> **Примечание.** Подробные сведения о различных представлениях и названиях отчетов см. в статье [Отчеты в Office 365: использование устройств с Yammer](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Отчеты

| Функция                                 | Возвращаемый тип CSV | Возвращаемый тип JSON                         | Описание                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Получение сведений о пользователях](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream          | [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) | Получение сведений об использовании устройств с Yammer с разбивкой по пользователям. |
| [Получение количества пользователей с разбивкой по устройствам](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream          | [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) | Получение сведений о количестве пользователей с разбивкой по типам устройств.  |
| [Получение количества пользователей](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) | Получение сведений о количестве пользователей в день с разбивкой по типам устройств. |
