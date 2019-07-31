---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 20374a3008e84b00ce7622019f4a3b8306a07318
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969522"
---
# <a name="vpnauthenticationmethod-enum-type"></a>тип перечисления Впнаусентикатионмесод

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Способ проверки подлинности VPN.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|certificate|нуль|Проверка подлинности с помощью сертификата.|
|Усернамеандпассворд|1,1|Используйте имя пользователя и пароль для проверки подлинности.|
|Шаредсекрет|2|Используйте общий секрет для проверки подлинности.  Поддерживается только для iOS IKEv2.|
|Дериведкредентиал|4|Используйте производные учетные данные для проверки подлинности.  Поддерживается только для iOS.|





