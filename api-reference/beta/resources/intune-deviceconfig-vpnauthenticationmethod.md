---
title: vpnAuthenticationMethod enum type
description: Метод проверки подлинности VPN.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22037a272e10c78c0d500bb20fb8955e20182170
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59146564"
---
# <a name="vpnauthenticationmethod-enum-type"></a>vpnAuthenticationMethod enum type

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Метод проверки подлинности VPN.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|certificate|0|Проверка подлинности с помощью сертификата.|
|usernameAndPassword|1|Используйте имя пользователя и пароль для проверки подлинности.|
|sharedSecret|2|Использование общего секрета для проверки подлинности.  Действительна только для iOS IKEv2.|
|derivedCredential|3|Использование производных учетных данных для проверки подлинности.|
|azureAD|4 |Используйте Azure AD для проверки подлинности.|



