---
title: тип ресурса windowsUpdateCatalogItem
description: Windows объект элемента каталога
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1c964c3ad3d0ec949cb2ab1eeed7aebe835e8939
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820417"
---
# <a name="windowsupdatecatalogitem-resource-type"></a>тип ресурса windowsUpdateCatalogItem

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Windows объект элемента каталога

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список windowsUpdateCatalogItems](../api/intune-softwareupdate-windowsupdatecatalogitem-list.md)|[коллекция windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|Список свойств и связей [объектов WindowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|
|[Get windowsUpdateCatalogItem](../api/intune-softwareupdate-windowsupdatecatalogitem-get.md)|[windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|Чтение свойств и связей [объекта WindowsUpdateCatalogItem.](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID элемента каталога.|
|displayName|String|Имя отображения элемента каталога.|
|releaseDateTime|DateTimeOffset|Дата выпуска элемента каталога|
|endOfSupportDate|DateTimeOffset|Последняя поддерживаемая дата элемента каталога|

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
  "releaseDateTime": "String (timestamp)",
  "endOfSupportDate": "String (timestamp)"
}
```



