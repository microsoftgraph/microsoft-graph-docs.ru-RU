---
title: Тип ресурса Граупполициобжектфиле
description: Файл объекта групповой политики, переданный администратором.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f1778e05f9c6f28966a92c46094d8e773b9de48
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458464"
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
|id|String|Пока не задокументировано.|
|граупполициобжектид|GUID|GUID объекта групповой политики из XML-содержимого объекта групповой политики|
|аудистингуишеднаме|String|Различающееся имя подразделения.|
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



