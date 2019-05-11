---
title: Тип ресурса КарттоклассассоЦиатион
description: КарттоклассассоЦиатион для связывания корзин устройств с аудиториями.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ccd3acb7770a0f2e9821268ae64dd70d1e7fcd71
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947465"
---
# <a name="carttoclassassociation-resource-type"></a>Тип ресурса КарттоклассассоЦиатион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

КарттоклассассоЦиатион для связывания корзин устройств с аудиториями.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список свойства carttoclassassociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|Коллекция [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md)|Список свойств и связей объектов [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Получение КарттоклассассоЦиатион](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Чтение свойств и связей объекта [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Создание КарттоклассассоЦиатион](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Создание нового объекта [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Удаление КарттоклассассоЦиатион](../api/intune-deviceconfig-carttoclassassociation-delete.md)|Нет|Удаляет объект [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md).|
|[Обновление КарттоклассассоЦиатион](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Обновление свойств объекта [карттоклассассоЦиатион](../resources/intune-deviceconfig-carttoclassassociation.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|version|Int32|Версия КарттоклассассоЦиатион.|
|displayName|Строка|Указанное администратором имя конфигурации устройства.|
|description|String|Администратор предоставил описание КарттоклассассоЦиатион.|
|Девицекартидс|Коллекция строк|Идентификаторы корзин устройств, которые необходимо связать с классами.|
|Классрумидс|Коллекция строк|Идентификаторы аудиторий, которые необходимо связать с тележками устройств.|

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




