---
title: тип remediationState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: dad0c6030d4a0f06ac17da9f2060b099d71d4ea4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788936"
---
# <a name="remediationstate-enum-type"></a>тип remediationState enum

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает тип выполнения сценария управления устройствами.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Неизвестный результат.|
|пропущено|1|Выполнение сценария восстановления было пропущено|
|success|2|Успешно выполнен сценарий восстановления и исправлено состояние устройства|
|remediationFailed|3|Сценарий восстановления, выполненный успешно, но не исправленное состояние устройства|
|scriptError|4 |Выполнение сценария восстановления, встречаемая и ошибка или приумно|



