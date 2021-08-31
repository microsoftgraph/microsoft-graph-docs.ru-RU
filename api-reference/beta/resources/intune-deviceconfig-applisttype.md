---
title: тип списка appListType
description: Возможные значения списка приложений для соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 01dfc746757f3709137f4d8909b2a98500f4888f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800739"
---
# <a name="applisttype-enum-type"></a>тип списка appListType

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения списка приложений для соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Значение по умолчанию, без намерения.|
|appsInListCompliant|1|В списке представлены приложения, которые будут считаться совместимыми (только приложения в списке совместимы).|
|appsNotInListCompliant|2|В списке представлены приложения, которые будут считаться не соответствующими требованиям (все приложения совместимы, за исключением приложений в списке).|



