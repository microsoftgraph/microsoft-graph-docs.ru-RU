---
title: тип enum wiFiSecurityType
description: Wi-Fi типы безопасности.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 600173712b5e00f8af9a6e9a94dc4b2167d6130b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057378"
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



