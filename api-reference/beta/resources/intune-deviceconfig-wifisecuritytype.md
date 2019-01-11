---
title: Тип перечисления wiFiSecurityType
description: Типы безопасности Wi-Fi.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 90290b9b47154b95aca81d931fa66e7984688db1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839923"
---
# <a name="wifisecuritytype-enum-type"></a>Тип перечисления wiFiSecurityType

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Типы безопасности Wi-Fi.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Откройте|0|Откройте (без проверки подлинности).|
|wpaPersonal|1|WPA-Personal.|
|wpaEnterprise|2|WPA-предприятие. Необходимо использовать тип IOSEnterpriseWifiConfiguration позволяет настроить параметры enterprise.|
|WEP|3|Шифрования WEP.|
|wpa2Personal|4|WPA2-личное.|
|wpa2Enterprise|5|WPA2-предприятие. Необходимо использовать тип WindowsWifiEnterpriseEAPConfiguration позволяет настроить параметры enterprise.|





