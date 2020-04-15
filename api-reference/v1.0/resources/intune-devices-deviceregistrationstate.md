---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b1974d8124c834185617332096d6b44429c7900a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472425"
---
# <a name="deviceregistrationstate-enum-type"></a>тип перечисления deviceRegistrationState

Пространство имен: microsoft.graph

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







