---
title: тип перечисления Ремедиатионстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc2be0c860ba142f59bba05a2a0c5ae0105c0ab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528517"
---
# <a name="remediationstate-enum-type"></a>тип перечисления Ремедиатионстате

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип состояния выполнения скрипта управления устройствами.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Неизвестный результат.|
|пропущенных|1 |Выполнение скрипта исправления пропущено|
|success|2 |Сценарий исправления успешно выполнен и исправлено состояние устройства|
|ремедиатионфаилед|3 |Сценарий исправления успешно выполнен, но ему не удалось исправить состояние устройства|
|скриптеррор|4 |Произошла ошибка или истекло время ожидания выполнения скрипта исправления|



