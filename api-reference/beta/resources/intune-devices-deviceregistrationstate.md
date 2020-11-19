---
title: тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: facd74e3ef2b2d4b6296e9b56fb99f6a2ed14fed
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267413"
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




