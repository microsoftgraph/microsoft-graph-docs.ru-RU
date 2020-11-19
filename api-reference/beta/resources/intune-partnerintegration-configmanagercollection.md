---
title: Тип ресурса Конфигманажерколлектион
description: Определенная Конфигманажер коллекция устройств или пользователей.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bc7d7d371a0bbc07b29835c5ed2a4b23078cf04
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302314"
---
# <a name="configmanagercollection-resource-type"></a>Тип ресурса Конфигманажерколлектион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определенная Конфигманажер коллекция устройств или пользователей.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Конфигманажерколлектионс](../api/intune-partnerintegration-configmanagercollection-list.md)|Коллекция [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md)|Список свойств и связей объектов [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) .|
|[Получение Конфигманажерколлектион](../api/intune-partnerintegration-configmanagercollection-get.md)|[конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md)|Чтение свойств и связей объекта [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) .|
|[Создание Конфигманажерколлектион](../api/intune-partnerintegration-configmanagercollection-create.md)|[конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md)|Создание нового объекта [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) .|
|[Удаление Конфигманажерколлектион](../api/intune-partnerintegration-configmanagercollection-delete.md)|Нет|Удаляет объект [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md).|
|[Обновление Конфигманажерколлектион](../api/intune-partnerintegration-configmanagercollection-update.md)|[конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md)|Обновление свойств объекта [конфигманажерколлектион](../resources/intune-partnerintegration-configmanagercollection.md) .|
|[Функция Жетполицисуммари](../api/intune-partnerintegration-configmanagercollection-getpolicysummary.md)|[конфигманажерполицисуммари](../resources/intune-partnerintegration-configmanagerpolicysummary.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ для коллекции Конфигманажер.|
|displayName|String|DisplayName.|
|коллектионидентифиер|String|Идентификатор коллекции в SCCM.|
|хиерарчинаме|String|Хиерарчинаме.|
|хиерарчидентифиер|String|Идентификатор иерархии.|
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




