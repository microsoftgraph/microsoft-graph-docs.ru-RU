---
title: тип ресурса cartToClassAssociation
description: CartToClassAssociation для связывания тележек устройств с классами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 133c59057c4c5d59eb16af808e69ec4b8ae385bba91a3fa01f05857a1dabbf44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226436"
---
# <a name="carttoclassassociation-resource-type"></a>тип ресурса cartToClassAssociation

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

CartToClassAssociation для связывания тележек устройств с классами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Списки cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[коллекция cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Список свойств и связей объектов [cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)|
|[Get cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Чтение свойств и связей объекта [cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)|
|[Создание cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Создайте новый [объект cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)|
|[Удаление cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|Нет|Удаляет [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).|
|[Обновление cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Обновление свойств объекта [cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|version|Int32|Версия CartToClassAssociation.|
|displayName|Строка|Указанное администратором имя конфигурации устройства.|
|description|String|Администратор предоставил описание CartToClassAssociation.|
|deviceCartIds|Коллекция String|Идентификаторы тележек устройств, связанных с классами.|
|classroomIds|Коллекция String|Идентификаторы классов, связанных с тележками устройств.|

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




