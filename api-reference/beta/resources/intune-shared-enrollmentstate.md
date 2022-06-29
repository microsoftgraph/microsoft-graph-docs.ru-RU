---
title: Тип перечисления enrollmentState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: afe74408d7e372b6fd9c92a31afd988bc3457f72
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441134"
---
# <a name="enrollmentstate-enum-type"></a>Тип перечисления enrollmentState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Состояние регистрации устройства неизвестно|
|Зачислены|1|Устройство зарегистрировано.|
|pendingReset|2|Зарегистрирован, но зарегистрирован через профиль регистрации, и зарегистрированный профиль отличается от назначенного профиля.|
|Сбой при|3|Регистрация не зарегистрирована и имеется запись о сбое регистрации.|
|notContacted|4|Устройство импортируется, но не зарегистрировано.|
|Заблокирован|5|Устройство регистрируется как без пользователя, но не может перейти на регистрацию пользователей, так как не удалось установить приложение.|



