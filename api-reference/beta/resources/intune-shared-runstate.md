---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 37905590f5ca61db53f98ff047ef699549f269ae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473510"
---
# <a name="runstate-enum-type"></a>тип перечисления Рунстате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип состояния выполнения скрипта управления устройствами.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|нуль|Неизвестный результат.|
|success|1,1|Сценарий успешно запущен.|
|сбой|2|Не удалось выполнить скрипт.|
|скриптеррор|4|Ошибка при обращении к скрипту обнаружения.|
|закончен|4 |Сценарий находится в состоянии ожидания выполнения.|
|нотаппликабле|5 |Сценарий неприменим для этого устройства.|



