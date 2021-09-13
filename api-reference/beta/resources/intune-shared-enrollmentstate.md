---
title: тип enum enrollmentState
description: Пока не задокументировано.
author: rolyon
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f06cb39e94dd526368b237b04d0bfefd9d68d095
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046612"
---
# <a name="enrollmentstate-enum-type"></a>тип enum enrollmentState

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние регистрации устройства неизвестно|
|зарегистрированный|1|Устройство зачислилось.|
|pendingReset|2|Зарегистрирован, но он зарегистрирован через профиль регистрации, а зарегистрированный профиль отличается от назначенного профиля.|
|не удалось|3|Не зарегистрирован, и есть запись сбоя регистрации.|
|notContacted|4 |Устройство импортируется, но не регистрируется.|
|заблокировано|5 |Устройство зарегистрировано как без пользователя, но не может двигаться к регистрации пользователей, так как приложение не удалось установить.|



