---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 89be71ded6aa970a5b1b598fe75488423b2b7de6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532203"
---
# <a name="deviceregistrationstate-enum-type"></a>тип перечисления deviceRegistrationState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние регистрации устройства.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нотрегистеред|нуль|Устройство не зарегистрировано.|
|охраняем|2 |Устройство зарегистрировано.|
|отозван|3 |Устройство заблокировано, очищено или снято.|
|кэйконфликт|4 |У устройства есть конфликт ключей.|
|аппровалпендинг|5 |Устройство ожидает утверждения.|
|цертификатересет|6 |Сертификат устройства сброшен.|
|нотрегистередпендинженроллмент|7 |Устройство не зарегистрировано и находится в состоянии ожидания регистрации.|
|unknown|8 |Состояние регистрации устройства неизвестно.|




