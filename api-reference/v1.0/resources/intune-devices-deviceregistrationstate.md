---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 678db76ca3218515306e847abf38c8dcac9d3b20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091154"
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
|отозван|4|Устройство заблокировано, очищено или снято.|
|кэйконфликт|4 |У устройства есть конфликт ключей.|
|аппровалпендинг|5 |Устройство ожидает утверждения.|
|цертификатересет|6 |Сертификат устройства сброшен.|
|нотрегистередпендинженроллмент|7 |Устройство не зарегистрировано и находится в состоянии ожидания регистрации.|
|unknown|8 |Состояние регистрации устройства неизвестно.|









