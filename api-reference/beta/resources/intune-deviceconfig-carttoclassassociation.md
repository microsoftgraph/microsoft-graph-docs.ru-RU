---
title: Тип ресурса cartToClassAssociation
description: CartToClassAssociation для связывания устройства корзины с помощью аудиторий.
ms.openlocfilehash: f177771cf6147771fc051d05e6fbb49d95b9feeb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077883"
---
# <a name="carttoclassassociation-resource-type"></a>Тип ресурса cartToClassAssociation

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

CartToClassAssociation для связывания устройства корзины с помощью аудиторий.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) коллекции|Свойства списка и связей объектов [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Получение cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Чтение свойства и связи объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Создание cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Создание нового объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Удаление cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|Нет|Удаляет [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).|
|[Обновление cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Обновление свойства объекта [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|version|Int32|Версия CartToClassAssociation.|
|displayName|String|Указанное администратором имя конфигурации устройства.|
|описание|String|Admin, предоставляемые описание CartToClassAssociation.|
|deviceCartIds|Коллекция String|Идентификаторы корзины устройства необходимо сопоставить с классы.|
|classroomIds|Коллекция String|Идентификаторы аудиторий необходимо сопоставить с устройства корзины.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cartToClassAssociation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
  ]
}
```





