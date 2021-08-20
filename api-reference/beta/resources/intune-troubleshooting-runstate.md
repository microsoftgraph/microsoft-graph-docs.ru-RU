---
title: тип runState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e89cce46a1738664f83c64b2ec96ad6cc3f20a6b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259471"
---
# <a name="runstate-enum-type"></a>тип runState enum

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип выполнения сценария управления устройствами.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный результат.|
|success|1 |Скрипт успешно работает.|
|сбой|2|Сценарий не удалось выполнить.|
|scriptError|3 |Скрипт обнаружения попадает в ошибку.|
|ожидание|4 |Скрипт находится в ожидании выполнения.|
|notApplicable|5 |Скрипт для этого устройства не применяется.|




