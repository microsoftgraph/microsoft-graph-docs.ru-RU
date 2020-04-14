---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dd3cc6887f5434df00a2ed9a817c0ca79c8c880e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412453"
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



