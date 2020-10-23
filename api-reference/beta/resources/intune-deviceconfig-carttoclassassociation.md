---
title: Тип ресурса КарттоклассассоЦиатион
description: КарттоклассассоЦиатион для связывания корзин устройств с аудиториями.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 987eb9ad94ca84b9af3c9b7991e0f18068b6fcb4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729821"
---
# <a name="carttoclassassociation-resource-type"></a>Тип ресурса КарттоклассассоЦиатион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|id|Строка|Ключ объекта.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|
|version|Int32|Версия КарттоклассассоЦиатион.|
|displayName|Строка|Указанное администратором имя конфигурации устройства.|
|description|Строка|Администратор предоставил описание КарттоклассассоЦиатион.|
|девицекартидс|Коллекция строк|Идентификаторы корзин устройств, которые необходимо связать с классами.|
|классрумидс|Коллекция строк|Идентификаторы аудиторий, которые необходимо связать с тележками устройств.|

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





