---
title: Тип перечисления wiFiSecurityType
description: Типы безопасности Wi-Fi.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 73724041c223d50d0030bf27b780d6b694792a16
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422133"
---
# <a name="wifisecuritytype-enum-type"></a>Тип перечисления wiFiSecurityType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




