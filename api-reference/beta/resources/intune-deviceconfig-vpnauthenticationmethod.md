---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dbb441bfc32e2de64f5950c033bdd24a3b05c59e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726404"
---
# <a name="vpnauthenticationmethod-enum-type"></a>тип перечисления Впнаусентикатионмесод

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Способ проверки подлинности VPN.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|certificate|нуль|Проверка подлинности с помощью сертификата.|
|усернамеандпассворд|1,1|Используйте имя пользователя и пароль для проверки подлинности.|
|шаредсекрет|2|Используйте общий секрет для проверки подлинности.  Поддерживается только для iOS IKEv2.|
|дериведкредентиал|4|Используйте производные учетные данные для проверки подлинности.|
|azureAD|4 |Используйте Azure AD для проверки подлинности.|





