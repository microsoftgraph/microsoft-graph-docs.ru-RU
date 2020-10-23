---
title: Тип ресурса Мобилеконтаинедапп
description: Абстрактный класс, представляющий вложенное приложение в mobileApp, работающее в виде пакета.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ebe9834cc527fe79b4fcd920927dfb70fa42db5
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48719752"
---
# <a name="mobilecontainedapp-resource-type"></a>Тип ресурса Мобилеконтаинедапп

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Абстрактный класс, представляющий вложенное приложение в mobileApp, работающее в виде пакета.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Мобилеконтаинедаппс](../api/intune-apps-mobilecontainedapp-list.md)|Коллекция [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md)|Список свойств и связей объектов [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md) .|
|[Получение Мобилеконтаинедапп](../api/intune-apps-mobilecontainedapp-get.md)|[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md);|Чтение свойств и связей объекта [мобилеконтаинедапп](../resources/intune-apps-mobilecontainedapp.md) .|

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





