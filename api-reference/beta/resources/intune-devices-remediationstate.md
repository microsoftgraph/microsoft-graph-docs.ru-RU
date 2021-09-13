---
title: тип remediationState enum
description: Указывает тип выполнения сценария управления устройствами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4e8925becd230f10904e15a9f105f475474b123d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137730"
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



