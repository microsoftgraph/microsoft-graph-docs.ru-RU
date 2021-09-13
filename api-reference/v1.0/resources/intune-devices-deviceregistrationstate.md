---
title: тип enum deviceRegistrationState
description: Состояние регистрации устройств.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 88f541d86a2c46b290f2c421e17a02c5c2b31b0f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59089496"
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




