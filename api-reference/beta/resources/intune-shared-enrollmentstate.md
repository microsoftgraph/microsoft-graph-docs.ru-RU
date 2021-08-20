---
title: тип enum enrollmentState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0817bb82e098d1fab93da3381c81faafc03b4cf0810e602934924305e0971edf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206111"
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
|зарегистрированный|1 |Устройство зачислилось.|
|pendingReset|2|Зарегистрирован, но он зарегистрирован через профиль регистрации, а зарегистрированный профиль отличается от назначенного профиля.|
|не удалось|3 |Не зарегистрирован, и есть запись сбоя регистрации.|
|notContacted|4 |Устройство импортируется, но не регистрируется.|
|заблокировано|5 |Устройство зарегистрировано как без пользователя, но не может двигаться к регистрации пользователей, так как приложение не удалось установить.|




