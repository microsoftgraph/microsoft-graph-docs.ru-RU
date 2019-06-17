---
title: тип перечисления Впнаусентикатионмесод
description: Способ проверки подлинности VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 343b8e3809a3f61926521a43d873161b2d5eee5f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994316"
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





