---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fef95d2d5744d0cdc6b92328b15a44f8b21c6cb0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523550"
---
# <a name="runstate-enum-type"></a>тип перечисления Рунстате

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип состояния выполнения скрипта управления устройствами.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Неизвестный результат.|
|success|1 |Сценарий успешно запущен.|
|сбой|2 |Не удалось выполнить скрипт.|
|скриптеррор|3 |Ошибка при обращении к скрипту обнаружения.|
|закончен|4 |Сценарий находится в состоянии ожидания выполнения.|
|нотаппликабле|5 |Сценарий неприменим для этого устройства.|



