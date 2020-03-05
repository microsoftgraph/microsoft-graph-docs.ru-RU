---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4f4716f65c5405cf324d758ffd3c8bcf38d61b5e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523774"
---
# <a name="actionstate-enum-type"></a>тип перечисления actionState

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние действия на устройстве

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нет|нуль|Недопустимое состояние действия|
|закончен|1 |Ожидается действие|
|закрыт|2 |Действие отменено.|
|ASP|3 |Действие активно.|
|done|4 |Действие выполнено без ошибок.|
|сбоев|5 |Не удалось выполнить действие|
|notSupported|6 |Действие не поддерживается.|



