---
title: тип ресурса configManagerCollection
description: ConfigManager определяет коллекцию устройств или пользователей.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a3833f2ee3ae94807af402b1109954b8785ab5a826ee0762ea0a4f0e1208af3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226247"
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
|id|String|Ключ для коллекции ConfigManager.|
|displayName|Строка|The DisplayName.|
|collectionIdentifier|Строка|Идентификатор коллекции в SCCM.|
|hierarchyName|String|Имя иерархии.|
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




