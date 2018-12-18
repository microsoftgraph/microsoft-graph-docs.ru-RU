---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
author: tfitzmac
ms.openlocfilehash: 3045685518f1c7718f9a5f46cd10e0add6fe05b3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330277"
---
# <a name="compliancestate-enum-type"></a>Тип перечисления complianceState

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Состояние соответствия требованиям.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестно.|
|спецификации|1|Спецификации.|
|несовместимый|2|Устройство не соответствует спецификации и запретом корпоративным ресурсам.|
|конфликта|3|Конфликт с другими правилами.|
|error|4|Ошибка|
|inGracePeriod|254|Устройство, не соответствует спецификации, но по-прежнему имеет доступ к корпоративным ресурсам|
|configManager|255|Управляет диспетчер конфигурации|



