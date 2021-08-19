---
title: vpnAuthenticationMethod enum type
description: Метод проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0fca9d52b09bdb19f85aa6fa06c166195263af39fbf143e956207f7a5e0a7b30
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226345"
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
|usernameAndPassword|1 |Используйте имя пользователя и пароль для проверки подлинности.|
|sharedSecret|2|Использование общего секрета для проверки подлинности.  Действительна только для iOS IKEv2.|
|derivedCredential|3 |Использование производных учетных данных для проверки подлинности.|
|azureAD|4 |Используйте Azure AD для проверки подлинности.|




