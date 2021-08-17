---
title: тип ресурса windowsUpdateCatalogItem
description: Windows объект элемента каталога
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a5c02bc7678b2487dda1ae61e07fc7d59de2cb829a026c0f8b3a385e3a68e383
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54165646"
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
|displayName|Строка|Имя отображения элемента каталога.|
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




