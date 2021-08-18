---
title: тип enum wiFiSecurityType
description: Wi-Fi типы безопасности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b24b05396a5b436d2c029cfe3991ccbab8cfbce665088d2f67ca62629f7d85c8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251416"
---
# <a name="wifisecuritytype-enum-type"></a>тип enum wiFiSecurityType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Wi-Fi типы безопасности.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|open|0|Open (Без проверки подлинности).|
|wpaPersonal|1 |WPA-Personal.|
|wpaEnterprise|2|WPA-Enterprise. Для настройки корпоративных параметров необходимо использовать тип IOSEnterpriseWifiConfiguration.|
|wep|3 |Шифрование WEP.|
|wpa2Personal|4 |WPA2-Personal.|
|wpa2Enterprise|5 |WPA2-Enterprise. Для настройки корпоративных параметров необходимо использовать тип WindowsWifiEnterpriseEAPConfiguration.|




