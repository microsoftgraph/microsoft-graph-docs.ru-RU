---
title: тип ресурса configManagerCollection
description: ConfigManager определяет коллекцию устройств или пользователей.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 961f43556622fd92cb990777155c8ab3debcb7df
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786616"
---
# <a name="configmanagercollection-resource-type"></a>тип ресурса configManagerCollection

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

ConfigManager определяет коллекцию устройств или пользователей.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список configManagerCollections](../api/intune-partnerintegration-configmanagercollection-list.md)|[коллекция configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Список свойств и связей объектов [configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)|
|[Get configManagerCollection](../api/intune-partnerintegration-configmanagercollection-get.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Чтение свойств и связей объекта [configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)|
|[Создание configManagerCollection](../api/intune-partnerintegration-configmanagercollection-create.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Создайте новый [объект configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)|
|[Удаление configManagerCollection](../api/intune-partnerintegration-configmanagercollection-delete.md)|Нет|Удаляет [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md).|
|[Обновление configManagerCollection](../api/intune-partnerintegration-configmanagercollection-update.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Обновление свойств объекта [configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)|
|[функция getPolicySummary](../api/intune-partnerintegration-configmanagercollection-getpolicysummary.md)|[configManagerPolicySummary](../resources/intune-partnerintegration-configmanagerpolicysummary.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ для коллекции ConfigManager.|
|displayName|Строка|The DisplayName.|
|collectionIdentifier|Строка|Идентификатор коллекции в SCCM.|
|hierarchyName|Строка|Имя иерархии.|
|hierarchyIdentifier|Строка|Идентификатор иерархии.|
|createdDateTime|DateTimeOffset|Дата создания.|
|lastModifiedDateTime|DateTimeOffset|Дата последнего изменения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configManagerCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "id": "String (identifier)",
  "displayName": "String",
  "collectionIdentifier": "String",
  "hierarchyName": "String",
  "hierarchyIdentifier": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



