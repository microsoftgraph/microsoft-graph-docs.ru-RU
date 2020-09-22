---
title: Тип ресурса mobileAppCategory
description: Содержит свойства для одной категории приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2a894f978b412c2916b9d036a1d4f708e231066b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094395"
---
# <a name="mobileappcategory-resource-type"></a>Тип ресурса mobileAppCategory

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для одной категории приложений Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppCategory](../api/intune-apps-mobileappcategory-list.md)|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список свойств и связей объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Получение объекта mobileAppCategory](../api/intune-apps-mobileappcategory-get.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Чтение свойств и связей объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Создание объекта mobileAppCategory](../api/intune-apps-mobileappcategory-create.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Создание объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Удаление объекта mobileAppCategory](../api/intune-apps-mobileappcategory-delete.md)|Нет|Удаляет объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Обновление объекта mobileAppCategory](../api/intune-apps-mobileappcategory-update.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|displayName|Строка|Имя категории приложений.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения mobileAppCategory.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```









