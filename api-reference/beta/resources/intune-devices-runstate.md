---
title: тип runState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 179ac69eab19f17bea478e50fa3591d19645a17d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033534"
---
# <a name="runstate-enum-type"></a>тип runState enum

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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



