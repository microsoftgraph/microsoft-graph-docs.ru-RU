---
title: Тип перечисления appListType
description: Возможные значения список соответствия требованиям приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1439ab860ab6a1fbf9ff4deb30320bb57fba338
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967240"
---
# <a name="applisttype-enum-type"></a>Тип перечисления appListType

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Возможные значения список соответствия требованиям приложения.
## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Значение по умолчанию, без цели.|
|appsInListCompliant|1|Список представляет приложений, которые будут считаться спецификации (только для приложений в списке совместимых).|
|appsNotInListCompliant|2|Представляет список приложений, которые будут считаться несовместимой (все приложения совместимых за исключением приложений в списке).|



