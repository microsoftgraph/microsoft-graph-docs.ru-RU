---
title: тип списка appListType
description: Возможные значения списка приложений для соответствия требованиям.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eab8857585226f84fcba2014cb72827ef5e0fd6f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069364"
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



