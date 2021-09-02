---
title: тип enum enrollmentState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b58391b7942bfdc32af6fce25a5e23b7a5f5bccc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787787"
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



