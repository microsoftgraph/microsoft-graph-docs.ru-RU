---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 030a1184fe9577a1a965ea65a90ad03f136858cc
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697695"
---
# <a name="deviceregistrationstate-enum-type"></a>тип перечисления deviceRegistrationState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние регистрации устройства.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нотрегистеред|нуль|Устройство не зарегистрировано.|
|охраняем|2|Устройство зарегистрировано.|
|отозван|4|Устройство заблокировано, очищено или снято.|
|кэйконфликт|4 |У устройства есть конфликт ключей.|
|аппровалпендинг|5 |Устройство ожидает утверждения.|
|цертификатересет|6 |Сертификат устройства сброшен.|
|нотрегистередпендинженроллмент|7 |Устройство не зарегистрировано и находится в состоянии ожидания регистрации.|
|unknown|8 |Состояние регистрации устройства неизвестно.|





