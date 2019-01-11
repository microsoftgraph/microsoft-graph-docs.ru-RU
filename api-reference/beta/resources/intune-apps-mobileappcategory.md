---
title: Тип ресурса mobileAppCategory
description: Содержит свойства для одной категории приложений Intune.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2ceb0453ffdf7180d55ba9b76ad95f873389924e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857164"
---
# <a name="mobileappcategory-resource-type"></a>Тип ресурса mobileAppCategory

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|id|String|Ключ объекта.|
|displayName|String|Имя категории приложений.|
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





