---
title: тип перечисления Граупполицимигратионреадинесс
description: Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efd579adb3c3408eda9b87ffb7f48e98c836065f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783174"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a>тип перечисления Граупполицимигратионреадинесс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Указывает, является ли файл объекта групповой политики охваченным и готовым к миграции в Intune.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|none|1,1|Нет покрытия Intune|
|части|2|Частичное покрытие Intune|
|complete|4|Выполнение действия в Intune|
|error|4 |Ошибка при анализе покрытия|
|нотаппликабле|5 |Нет параметров групповой политики в объекте групповой политики|



