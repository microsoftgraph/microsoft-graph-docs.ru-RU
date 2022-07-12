---
title: Тип перечисления deviceRegistrationState
description: Состояние регистрации устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a104fb6f347d24dbb2e3d373a1046148486b387e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730639"
---
# <a name="deviceregistrationstate-enum-type"></a>Тип перечисления deviceRegistrationState

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние регистрации устройства.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notRegistered|0|Устройство не зарегистрировано.|
|Зарегистрированных|2|Устройство зарегистрировано.|
|Отозван|3|Устройство заблокировано, очищено или удалено.|
|keyConflict|4|У устройства есть конфликт ключей.|
|approvalPending|5|Устройство ожидает утверждения.|
|certificateReset|6 |Сертификат устройства был сброшен.|
|notRegisteredPendingEnrollment|7 |Устройство не зарегистрировано и ожидает регистрации.|
|unknown|8 |Состояние регистрации устройства неизвестно.|





