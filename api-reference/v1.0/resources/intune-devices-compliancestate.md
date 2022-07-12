---
title: Тип перечисления complianceState
description: Состояние соответствия.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 20d0c049a8274bbedf4c618c54cdf003b9fbfb63
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736078"
---
# <a name="compliancestate-enum-type"></a>Тип перечисления complianceState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние соответствия.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестно.|
|Совместимый|1|Совместимый.|
|Несовместимые|2|Устройство не соответствует требованиям и заблокировано корпоративными ресурсами.|
|Конфликта|3|Конфликт с другими правилами.|
|error|4|Ошибка|
|inGracePeriod|254|Устройство не соответствует требованиям, но по-прежнему имеет доступ к корпоративным ресурсам|
|configManager|255|Управляется диспетчером конфигураций|





