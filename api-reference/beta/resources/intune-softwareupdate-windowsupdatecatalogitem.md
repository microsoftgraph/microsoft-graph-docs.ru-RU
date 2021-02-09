---
title: Тип ресурса windowsUpdateCatalogItem
description: Сущность элемента каталога обновлений Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5de85dde2c9f2b5bc68e9644b96852bdbe880de
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162447"
---
# <a name="windowsupdatecatalogitem-resource-type"></a>Тип ресурса windowsUpdateCatalogItem

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность элемента каталога обновлений Windows

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsUpdateCatalogItems](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|[Коллекция windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|Список свойств и связей объектов [windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|[Get windowsUpdateCatalogItem](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|Чтение свойств и связей объекта [windowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД элемента каталога.|
|displayName|String|Отображаемого имени элемента каталога.|
|releaseDateTime|DateTimeOffset|Дата выпуска элемента каталога|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)"
}
```




