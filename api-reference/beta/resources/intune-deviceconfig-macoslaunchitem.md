---
title: Тип ресурса Макослаунчитем
description: Представляет приложение в списке элементов запуска macOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dbdec2156c135544a6ce36887fcd7c911217dff5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529682"
---
# <a name="macoslaunchitem-resource-type"></a>Тип ресурса Макослаунчитем

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет приложение в списке элементов запуска macOS

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|path|String|Путь к запускаемому элементу.|
|скрытых|Логический|Указывает, следует ли скрыть элемент в списке "пользователи и группы".|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```



