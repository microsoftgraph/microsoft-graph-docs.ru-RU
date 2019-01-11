---
title: Тип ресурса mobileContainedApp
description: Абстрактный класс, представляющий автономные приложения в mobileApp, работающие в качестве пакета.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b81ee4ca194d1d01e3d834b3287f6b400e712a27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826287"
---
# <a name="mobilecontainedapp-resource-type"></a>Тип ресурса mobileContainedApp

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Абстрактный класс, представляющий автономные приложения в mobileApp, работающие в качестве пакета.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список mobileContainedApps](../api/intune-apps-mobilecontainedapp-list.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) коллекции|Свойства списка и связей объектов [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .|
|[Получение mobileContainedApp](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md);|Чтение свойства и связи объекта [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```





