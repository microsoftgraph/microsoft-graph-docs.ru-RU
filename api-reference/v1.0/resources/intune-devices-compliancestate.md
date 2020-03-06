---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3b0b20615dfdda489649182d0c0687e9a735b5f7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532226"
---
# <a name="compliancestate-enum-type"></a>тип перечисления Комплианцестате

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Найден.|
|совместимо|1 |Совместимо.|
|несоответствующих|2 |Устройство не совместимо и заблокировано из корпоративных ресурсов.|
|противоречивы|3 |Конфликт с другими правилами.|
|error|4 |Ошибка|
|инграцепериод|254|Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам|
|конфигманажер|255|Управление с помощью диспетчера конфигураций|




