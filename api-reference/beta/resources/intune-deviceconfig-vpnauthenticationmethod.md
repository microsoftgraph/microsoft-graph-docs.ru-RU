---
title: vpnAuthenticationMethod enum type
description: Метод проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 83d1789f02c8cc961bd4d1c784ad70f47c6b7f85
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58789935"
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



