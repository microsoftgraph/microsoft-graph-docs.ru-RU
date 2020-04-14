---
title: тип перечисления Комплианцестате
description: Состояние соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c088f3a0fc3a4bd4b01f29da5f228920f00a398f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465145"
---
# <a name="compliancestate-enum-type"></a>тип перечисления Комплианцестате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Найден.|
|совместимо|1,1|Совместимо.|
|несоответствующих|2|Устройство не совместимо и заблокировано из корпоративных ресурсов.|
|противоречивы|4|Конфликт с другими правилами.|
|error|4 |Ошибка|
|инграцепериод|254|Устройство не соответствует требованиям, но имеет доступ к корпоративным ресурсам|
|конфигманажер|255|Управление с помощью диспетчера конфигураций|



