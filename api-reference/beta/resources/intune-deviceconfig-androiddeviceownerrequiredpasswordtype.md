---
title: тип enum androidDeviceOwnerRequiredPasswordType
description: Политика владельца android-устройств требует типа пароля.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c3fb30d71826a273ebd1e128d292508f76bfe7a4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023621"
---
# <a name="androiddeviceownerrequiredpasswordtype-enum-type"></a>тип enum androidDeviceOwnerRequiredPasswordType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Политика владельца android-устройств требует типа пароля.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|deviceDefault|0|Значение устройства по умолчанию, без намерения.|
|обязательно|1|Должен быть набор паролей, но ограничений по типу нет.|
|числовая|2|По крайней мере числовая.|
|numericComplex|3|По крайней мере числовая без повторения или заказа последовательностей.|
|алфавитный|4 |По крайней мере алфавитный пароль.|
|alphanumeric|5 |По крайней мере, альфа-пароль|
|alphanumericWithSymbols|6 |По крайней мере, альфа-число с символами.|
|lowSecurityBiometric|7 |Требуется пароль с низкой безопасностью на основе биометрии.|
|customPassword|8 |Настраиваемый пароль, установленный администратором.|



