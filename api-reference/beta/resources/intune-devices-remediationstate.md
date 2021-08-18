---
title: тип remediationState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7a47a880dbf067c455ca108fd8f80636810a6d31bc196b3c3198a87b089f6959
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164211"
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
|пропущено|1 |Выполнение сценария восстановления было пропущено|
|success|2|Успешно выполнен сценарий восстановления и исправлено состояние устройства|
|remediationFailed|3 |Сценарий восстановления, выполненный успешно, но не исправленное состояние устройства|
|scriptError|4 |Выполнение сценария восстановления, встречаемая и ошибка или приумно|




