---
title: Тип ресурса mobileAppCategory
description: Содержит свойства для одной категории приложений Intune.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5cc3d55a717691fc3162bf0ca6f0a633b0e5a95
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327530"
---
# <a name="mobileappcategory-resource-type"></a>Тип ресурса mobileAppCategory

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для одной категории приложений Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов mobileAppCategory](../api/intune-apps-mobileappcategory-list.md)|Коллекция [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Список свойств и связей объектов [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Получение объекта mobileAppCategory](../api/intune-apps-mobileappcategory-get.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md);|Чтение свойств и связей объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Создание объекта mobileAppCategory](../api/intune-apps-mobileappcategory-create.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md);|Создание объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Удаление объекта mobileAppCategory](../api/intune-apps-mobileappcategory-delete.md)|Нет|Удаляет объект [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Обновление объекта mobileAppCategory](../api/intune-apps-mobileappcategory-update.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Обновление свойств объекта [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|Строка|Имя категории приложений.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения mobileAppCategory.|

## <a name="relationships"></a>Отношения
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



