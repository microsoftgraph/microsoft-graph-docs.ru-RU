---
title: тип runState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1785f433c604c441072b953a3efae94978d449f4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612296"
---
# <a name="runstate-enum-type"></a>тип runState enum

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип выполнения сценария управления устройствами.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный результат.|
|success|1|Скрипт успешно работает.|
|сбой|2|Сценарий не удалось выполнить.|
|scriptError|3|Скрипт обнаружения попадает в ошибку.|
|ожидание|4 |Скрипт находится в ожидании выполнения.|
|notApplicable|5 |Скрипт для этого устройства не применяется.|




