---
title: Тип перечисления appListType
description: Возможные значения списка приложений для соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b801765b4524a22a6525a41d6635daa382564e8e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66722770"
---
# <a name="applisttype-enum-type"></a>Тип перечисления appListType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения списка приложений для соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|0|Значение по умолчанию, без намерения.|
|appsInListCompliant|1|Список представляет приложения, которые будут считаться совместимыми (только приложения в списке соответствуют требованиям).|
|appsNotInListCompliant|2|Список представляет приложения, которые будут считаться несоответствующими (все приложения соответствуют требованиям, кроме приложений в списке).|





