---
title: Тип ресурса КарттоклассассоЦиатион
description: КарттоклассассоЦиатион для связывания корзин устройств с аудиториями.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 228a3bfc873fdaf1fbd77e51a79ca184c2416d7c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156597"
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
|displayName|String|Указанное администратором имя конфигурации устройства.|
|description|String|Администратор предоставил описание КарттоклассассоЦиатион.|
|Девицекартидс|Коллекция строк|Идентификаторы корзин устройств, которые необходимо связать с классами.|
|Классрумидс|Коллекция строк|Идентификаторы аудиторий, которые необходимо связать с тележками устройств.|

## <a name="relationships"></a>Отношения
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




