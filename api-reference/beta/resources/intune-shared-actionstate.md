---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 83370402104e4ebd42551262aaa98c109149e32e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067274"
---
# <a name="actionstate-enum-type"></a>тип перечисления actionState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние действия на устройстве

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|нуль|Недопустимое состояние действия|
|закончен|1 |Ожидается действие|
|закрыт|2 |Действие отменено.|
|ASP|4|Действие активно.|
|done|4 |Действие выполнено без ошибок.|
|сбоев|5 |Не удалось выполнить действие|
|notSupported|6 |Действие не поддерживается.|






