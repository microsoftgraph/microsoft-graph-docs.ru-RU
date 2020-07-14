---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ef477b17b8ae7e8aedc3b95ce70b66115a3c8712
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123892"
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
|усернамеандпассворд|1 |Используйте имя пользователя и пароль для проверки подлинности.|
|шаредсекрет|2 |Используйте общий секрет для проверки подлинности.  Поддерживается только для iOS IKEv2.|
|дериведкредентиал|3 |Используйте производные учетные данные для проверки подлинности.|
|azureAD|4 |Используйте Azure AD для проверки подлинности.|



