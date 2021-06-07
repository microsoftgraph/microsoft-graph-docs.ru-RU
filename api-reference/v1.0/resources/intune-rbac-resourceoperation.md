---
title: Тип ресурса resourceOperation
description: Описывает ресурс resourceOperation (сущность) API microsoft Graph (REST), который поддерживает процессы intune, связанные с управлением доступом на основе ролей (RBAC).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d7e66c7cdbf7431d640d676c20bc074670cbd0a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751568"
---
# <a name="resourceoperation-resource-type"></a>Тип ресурса resourceOperation

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Описывает ресурс resourceOperation (сущность) API microsoft Graph (REST), который поддерживает процессы intune, связанные с управлением доступом на основе ролей (RBAC).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов resourceOperation](../api/intune-rbac-resourceoperation-list.md)|Коллекция объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Список свойств и связей объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Получение объекта resourceOperation](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Чтение свойств и связей объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Создание объекта resourceOperation](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Удаление объекта resourceOperation](../api/intune-rbac-resourceoperation-delete.md)|Нет|Удаление объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Обновление объекта resourceOperation](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Обновление свойств объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ операции с ресурсом. Доступен только для чтения и создается автоматически.|
|resourceName|String|Имя ресурса, с которым выполняется эта операция.|
|actionName|String|Тип действия, которое выполнит эта операция. Свойство actionName должно быть максимально краткое (максимум несколько слов).|
|description|String|Описание операции с ресурсом. Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "String (identifier)",
  "resourceName": "String",
  "actionName": "String",
  "description": "String"
}
```




