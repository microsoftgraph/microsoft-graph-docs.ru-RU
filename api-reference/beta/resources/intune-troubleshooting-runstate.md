---
title: тип runState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f25057c0fcd19b3a9ad121471876f7b6f1e5d15
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020177"
---
# <a name="runstate-enum-type"></a>тип runState enum

Пространство имен: microsoft.graph

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




