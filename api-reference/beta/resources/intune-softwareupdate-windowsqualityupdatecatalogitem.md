---
title: Тип ресурса windowsQualityUpdateCatalogItem
description: Сущность элемента каталога обновлений Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76813f404004445595b7439019bc33a73cda719f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162462"
---
# <a name="windowsqualityupdatecatalogitem-resource-type"></a>Тип ресурса windowsQualityUpdateCatalogItem

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность элемента каталога обновлений Windows


Наследуется от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsQualityUpdateCatalogItems](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-list.md)|[Коллекция windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Список свойств и связей объектов [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Get windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-get.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Чтение свойств и связей объекта [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Создание windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-create.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Создание объекта [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Удаление windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-delete.md)|Нет|Удаляет [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Обновление windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-update.md)|[windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Обновление свойств объекта [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|String|Отображаемого имени элемента каталога. Наследуется [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|Дата выпуска элемента каталога. Наследуется от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|kbArticleId|String|ИД статьи базы знаний|
|classification|[windowsQualityUpdateClassification](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|Классификация обновления качества. Возможные значения: `all`, `security`, `nonSecurity`.|
|isExpeditable|Boolean|Флаг, указывающий, является ли обновление квалификатором для ускорения|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsQualityUpdateCatalogItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "String (identifier)",
  "displayName": "String",
  "releaseDateTime": "String (timestamp)",
  "kbArticleId": "String",
  "classification": "String",
  "isExpeditable": true
}
```




