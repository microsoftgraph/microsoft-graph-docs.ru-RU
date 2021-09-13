---
title: тип enum androidWorkProfileRequiredPasswordType
description: Рабочий профиль Android требуется тип пароля.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 630743d82742102687675f5f1c7de3b75443320b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111273"
---
# <a name="androidworkprofilerequiredpasswordtype-enum-type"></a>тип enum androidWorkProfileRequiredPasswordType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Рабочий профиль Android требуется тип пароля.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение устройства по умолчанию, без намерения.|
|lowSecurityBiometric|1|Требуется пароль с низкой безопасностью на основе биометрии.|
|обязательно|2|Обязательно.|
|atLeastNumeric|3|Требуется по крайней мере числовая пароль.|
|numericComplex|4 |Требуется числовый сложный пароль.|
|atLeastAlphabetic|5 |Требуется по крайней мере алфавитный пароль.|
|atLeastAlphanumeric|6 |Требуется, по крайней мере, альфа-числовая пароль.|
|alphanumericWithSymbols|7 |По крайней мере, альфа-число с паролем символов.|



