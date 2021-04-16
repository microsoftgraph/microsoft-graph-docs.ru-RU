---
title: тип enum enrollmentState
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d208f8a4d1097d6698be3175a0b5ae86cf1918d4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866799"
---
# <a name="enrollmentstate-enum-type"></a>тип enum enrollmentState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

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




