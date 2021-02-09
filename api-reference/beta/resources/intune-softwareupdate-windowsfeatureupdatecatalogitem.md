---
title: Тип ресурса windowsFeatureUpdateCatalogItem
description: Сущность элемента каталога обновлений Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e02546a0d09690ecd720e565e9193aa2c8ec72f4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162468"
---
# <a name="windowsfeatureupdatecatalogitem-resource-type"></a>Тип ресурса windowsFeatureUpdateCatalogItem

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность элемента каталога обновлений Windows


Наследуется от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsFeatureUpdateCatalogItems](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-list.md)|[Коллекция windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|Список свойств и связей объектов [windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|
|[Get windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-get.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|Чтение свойств и связей объекта [windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|
|[Создание windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-create.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|Создание объекта [windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|
|[Удаление windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-delete.md)|Нет|Удаляет [windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|
|[Обновление windowsFeatureUpdateCatalogItem](../api/intune-softwareupdate-windowsfeatureupdatecatalogitem-update.md)|[windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|Обновление свойств объекта [windowsFeatureUpdateCatalogItem.](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|String|Отображаемого имени элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|Дата выпуска элемента каталога. Наследуется от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|version|String|Версия обновления функций|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFeatureUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "version": "String"
}
```




