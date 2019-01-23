---
title: Тип перечисления androidDeviceOwnerRequiredPasswordType
description: Android политики устройства владельцем требуется тип пароль.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c405cf3a69597994d5539427698baa92cabd3904
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403541"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>Тип перечисления androidDeviceOwnerRequiredPasswordType

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Android политики устройства владельцем требуется тип пароль.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение по умолчанию устройства, без цели.|
|Обязательный|1|Необходимо задать пароль, но не существует ограничений на тип.|
|числовое|2|AT бы числовое.|
|numericComplex|3|AT бы числовое с последовательности не повторяющиеся или упорядоченном.|
|к буквам и цифрам|4|По крайней мере к буквам и цифрам пароль.|
|буквенно-цифровые;|5|По крайней мере буквенно-цифровой пароль|
|alphanumericWithSymbols|6|По крайней мере буквенно-цифровые символы.|




