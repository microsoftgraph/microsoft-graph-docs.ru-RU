---
title: Тип перечисления complianceState
description: Состояние соответствия требованиям.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a4f4c359665eb1a0087f64802b5e7c829002fd6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940199"
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



