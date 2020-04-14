---
title: тип перечисления actionState
description: Состояние действия на устройстве
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c213567b46c7aea2f91deae8bc8a27d4b0382c7d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453182"
---
# <a name="actionstate-enum-type"></a>тип перечисления actionState

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Состояние действия на устройстве

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|нет|нуль|Недопустимое состояние действия|
|закончен|1,1|Ожидается действие|
|закрыт|2|Действие отменено.|
|ASP|4|Действие активно.|
|done|4 |Действие выполнено без ошибок.|
|сбоев|5 |Не удалось выполнить действие|
|notSupported|6 |Действие не поддерживается.|



