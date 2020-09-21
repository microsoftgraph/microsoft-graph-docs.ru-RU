---
title: тип перечисления Рунстате
description: Указывает тип состояния выполнения скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 36022987fb96671399523a5936c7799e97db33c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084046"
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
|success|1 |Сценарий успешно запущен.|
|сбой|2 |Не удалось выполнить скрипт.|
|скриптеррор|4|Ошибка при обращении к скрипту обнаружения.|
|закончен|4 |Сценарий находится в состоянии ожидания выполнения.|
|нотаппликабле|5 |Сценарий неприменим для этого устройства.|






