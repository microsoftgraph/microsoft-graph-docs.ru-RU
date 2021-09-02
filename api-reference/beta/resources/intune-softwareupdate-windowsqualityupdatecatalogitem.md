---
title: тип ресурса windowsQualityUpdateCatalogItem
description: Windows объект элемента каталога
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25f4838145c47ef23ce2ee50300452fbf0e9333f
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58821909"
---
# <a name="windowsqualityupdatecatalogitem-resource-type"></a>тип ресурса windowsQualityUpdateCatalogItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows объект элемента каталога


Наследует [от windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsQualityUpdateCatalogItems](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-list.md)|[коллекция windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Список свойств и связей [объектов WindowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Get windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-get.md)|[WindowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Чтение свойств и связей [объекта WindowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Создание windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-create.md)|[WindowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Создайте [новый объект WindowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|
|[Удаление windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-delete.md)|Нет|Удаляет [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).|
|[Обновление windowsQualityUpdateCatalogItem](../api/intune-softwareupdate-windowsqualityupdatecatalogitem-update.md)|[WindowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|Обновление свойств объекта [windowsQualityUpdateCatalogItem.](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|displayName|String|Имя отображения элемента каталога. Унаследованный от [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|Дата выпуска элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|endOfSupportDate|DateTimeOffset|Последняя поддерживаемая дата для элемента каталога, наследуемого [из windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|kbArticleId|String|ID статьи базы знаний|
|classification|[windowsQualityUpdateClassification](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|Классификация обновления качества. Возможные значения: `all`, `security`, `nonSecurity`.|
|isExpeditable|Логический|Флаг, указывающий, имеет ли обновление право на ускорение|

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
  "endOfSupportDate": "String (timestamp)",
  "kbArticleId": "String",
  "classification": "String",
  "isExpeditable": true
}
```



