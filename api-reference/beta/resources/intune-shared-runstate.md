---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ec8d3f9333393b946539d639c9cc9eeb30c6b027
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725157"
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





