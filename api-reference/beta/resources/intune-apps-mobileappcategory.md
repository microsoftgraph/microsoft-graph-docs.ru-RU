---
title: Тип ресурса mobileAppCategory
description: Содержит свойства для одной категории приложений Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 431de325915747bc31620d8ea77c697b71b5db9d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723036"
---
# <a name="mobileappcategory-resource-type"></a>Тип ресурса mobileAppCategory

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

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





