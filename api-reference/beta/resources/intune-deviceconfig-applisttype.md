---
title: тип списка appListType
description: Возможные значения списка приложений для соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7a5609bc6847c35bcc196e4df6a1ec94a3150e2907c530ac52e2acb44b362d79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213216"
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
|appsInListCompliant|1 |В списке представлены приложения, которые будут считаться совместимыми (только приложения в списке совместимы).|
|appsNotInListCompliant|2|В списке представлены приложения, которые будут считаться не соответствующими требованиям (все приложения совместимы, за исключением приложений в списке).|




