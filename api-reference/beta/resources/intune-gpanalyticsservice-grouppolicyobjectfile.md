---
title: Тип ресурса Граупполициобжектфиле
description: Файл объекта групповой политики, переданный администратором.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b68282f9920e9111ab0b5d09f448abc6c688603e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727297"
---
# <a name="grouppolicyobjectfile-resource-type"></a>Тип ресурса Граупполициобжектфиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Файл объекта групповой политики, переданный администратором.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициобжектфилес](../api/intune-gpanalyticsservice-grouppolicyobjectfile-list.md)|Коллекция [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Список свойств и связей объектов [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .|
|[Получение Граупполициобжектфиле](../api/intune-gpanalyticsservice-grouppolicyobjectfile-get.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Чтение свойств и связей объекта [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .|
|[Создание Граупполициобжектфиле](../api/intune-gpanalyticsservice-grouppolicyobjectfile-create.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Создание нового объекта [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .|
|[Удаление Граупполициобжектфиле](../api/intune-gpanalyticsservice-grouppolicyobjectfile-delete.md)|Нет|Удаляет объект [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).|
|[Обновление Граупполициобжектфиле](../api/intune-gpanalyticsservice-grouppolicyobjectfile-update.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Обновление свойств объекта [граупполициобжектфиле](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Пока не задокументировано.|
|граупполициобжектид|Guid|GUID объекта групповой политики из XML-содержимого объекта групповой политики|
|аудистингуишеднаме|Строка|Различающееся имя подразделения.|
|createdDateTime|DateTimeOffset|Дата и время первой загрузки Граупполици.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения Граупполициобжектфиле.|
|content|String|Содержимое файла объекта групповой политики.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "String (identifier)",
  "groupPolicyObjectId": "Guid",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "content": "String"
}
```





