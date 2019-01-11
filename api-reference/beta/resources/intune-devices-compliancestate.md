---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b3d496d6890d0da4d817ad9ba1f03e4b0825204d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861679"
---
# <a name="compliancestate-enum-type"></a>Тип перечисления complianceState

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

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





