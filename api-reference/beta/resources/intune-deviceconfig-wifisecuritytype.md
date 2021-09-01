---
title: тип enum wiFiSecurityType
description: Wi-Fi типы безопасности.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a259b72691654ac979f65cbe4f445578743a491c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58797882"
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
|wpaPersonal|1|WPA-Personal.|
|wpaEnterprise|2|WPA-Enterprise. Для настройки корпоративных параметров необходимо использовать тип IOSEnterpriseWifiConfiguration.|
|wep|3|Шифрование WEP.|
|wpa2Personal|4 |WPA2-Personal.|
|wpa2Enterprise|5 |WPA2-Enterprise. Для настройки корпоративных параметров необходимо использовать тип WindowsWifiEnterpriseEAPConfiguration.|



