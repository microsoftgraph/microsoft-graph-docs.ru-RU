---
title: тип enum androidRequiredPasswordType
description: Тип пароля, требуемого для Android.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2e4931cef836f446613c54b3c9eb3eaf9506de24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59101683"
---
# <a name="androidrequiredpasswordtype-enum-type"></a>тип enum androidRequiredPasswordType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Тип пароля, требуемого для Android.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение устройства по умолчанию, без намерения.|
|алфавитный|1|Требуется алфавитный пароль.|
|alphanumeric|2|Необходимый альфа-пароль.|
|alphanumericWithSymbols|3|Альфа-число с паролем символов.|
|lowSecurityBiometric|4 |Требуется пароль с низкой безопасностью на основе биометрии.|
|числовая|5 |Необходимый числовой пароль.|
|numericComplex|6 |Требуется числовый сложный пароль.|
|любой|7 |Требуется пароль или шаблон, и любой из них является приемлемым.|



