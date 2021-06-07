---
title: тип enum deviceRegistrationState
description: Состояние регистрации устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 39a4c68f2a688564284fc6045f61b84e72b748ab
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751694"
---
# <a name="deviceregistrationstate-enum-type"></a>тип enum deviceRegistrationState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние регистрации устройств.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notRegistered|0|Устройство не зарегистрировано.|
|зарегистрирована|2|Устройство зарегистрировано.|
|отменено|3|Устройство было заблокировано, вытерто или отошедо.|
|keyConflict|4 |У устройства есть ключевой конфликт.|
|approvalPending|5 |Устройство находится на стадии утверждения.|
|certificateReset|6 |Сертификат устройства был сброшен.|
|notRegisteredPendingEnrollment|7 |Устройство не регистрируется и не ожидает регистрации.|
|unknown|8 |Состояние регистрации устройства неизвестно.|




