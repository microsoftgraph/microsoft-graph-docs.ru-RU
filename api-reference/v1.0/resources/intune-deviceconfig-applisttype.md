---
title: тип списка appListType
description: Возможные значения списка приложений для соответствия требованиям.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a5410919bb33a4a77d4d774108157519fad9ae4d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60455923"
---
# <a name="applisttype-enum-type"></a>тип списка appListType

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Возможные значения списка приложений для соответствия требованиям.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|Нет|0|Значение по умолчанию, без намерения.|
|appsInListCompliant|1|В списке представлены приложения, которые будут считаться совместимыми (только приложения в списке совместимы).|
|appsNotInListCompliant|2|В списке представлены приложения, которые будут считаться не соответствующими требованиям (все приложения совместимы, за исключением приложений в списке).|



