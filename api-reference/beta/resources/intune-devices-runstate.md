---
title: тип runState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fee3d6eef67b4af198e0a038875ece20fc640fc3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817077"
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



