---
title: тип enum deviceRegistrationState
description: Состояние регистрации устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7197e541b46cc3f63340ee804f126a14d862283c616a1baf980c81725e6b5a87
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54197984"
---
# <a name="deviceregistrationstate-enum-type"></a>тип enum deviceRegistrationState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние регистрации устройств.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notRegistered|0|Устройство не зарегистрировано.|
|зарегистрирована|2|Устройство зарегистрировано.|
|отменено|3 |Устройство было заблокировано, вытерто или отошедо.|
|keyConflict|4 |У устройства есть ключевой конфликт.|
|approvalPending|5 |Устройство находится на стадии утверждения.|
|certificateReset|6 |Сертификат устройства был сброшен.|
|notRegisteredPendingEnrollment|7 |Устройство не регистрируется и не ожидает регистрации.|
|unknown|8 |Состояние регистрации устройства неизвестно.|




