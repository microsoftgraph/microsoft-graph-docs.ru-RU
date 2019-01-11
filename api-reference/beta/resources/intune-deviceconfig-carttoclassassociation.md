---
title: Тип ресурса cartToClassAssociation
description: CartToClassAssociation для связывания устройства корзины с помощью аудиторий.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 02a7d04b40d4d984f98f04eb653ee45ed436d099
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868035"
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
|id|Строка|Ключ объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|version|Int32|Версия CartToClassAssociation.|
|displayName|Строка|Указанное администратором имя конфигурации устройства.|
|описание|Строка|Admin, предоставляемые описание CartToClassAssociation.|
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





