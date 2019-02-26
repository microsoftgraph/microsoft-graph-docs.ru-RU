---
title: Тип ресурса resourceOperation
description: Описывает ресурс resourceOperation (Entity) API Microsoft Graph (REST), который поддерживает рабочие процессы Intune, связанные с управлением доступом на основе ролей (RBAC).
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c203b47235d94a3742c5cb0cee401d824feafb46
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257864"
---
# <a name="resourceoperation-resource-type"></a>Тип ресурса resourceOperation

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Определяет операцию или действие, которые можно выполнять с ресурсом (или объектом) Intune.  Распространенные операции — чтение, удаление, обновление и создание.  Они обеспечивают основные возможности управления базовым ресурсом Intune.  В некоторых случаях ресурс Intune может включать операции, выполняемые в сочетании с другими ресурсами.  Например, операция Assign позволяет назначить ресурс MobileApp группе безопасности AAD.  Операции с ресурсами невозможно изменить для встроенных ролей. Это определяет операцию или действие, которые можно выполнить с ресурсом (или объектом) Intune.  Распространенные операции — получение, перечисление, обновление и создание.  Они обеспечивают основные возможности управления базовым ресурсом Intune.  В некоторых случаях ресурс Intune может включать операции, выполняемые в сочетании с другими ресурсами.  Например, операция Assign позволяет назначить ресурс MobileApp группе безопасности AAD.  Операции с ресурсами невозможно изменить для встроенных ролей.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов resourceOperation](../api/intune-rbac-resourceoperation-list.md)|Коллекция объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md)|Список свойств и связей объектов [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Получение объекта resourceOperation](../api/intune-rbac-resourceoperation-get.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md);|Чтение свойств и связей объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Создание объекта resourceOperation](../api/intune-rbac-resourceoperation-create.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md);|Создание объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Удаление объекта resourceOperation](../api/intune-rbac-resourceoperation-delete.md)|Нет|Удаление объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).|
|[Обновление объекта resourceOperation](../api/intune-rbac-resourceoperation-update.md)|[resourceOperation](../resources/intune-rbac-resourceoperation.md)|Обновление свойств объекта [resourceOperation](../resources/intune-rbac-resourceoperation.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ операции с ресурсом. Доступен только для чтения и создается автоматически.|
|resourceName|String|Имя ресурса, с которым выполняется эта операция.|
|actionName|String|Тип действия, которое выполнит эта операция. Свойство actionName должно быть максимально кратким (только несколько слов).|
|description|Строка|Описание операции с ресурсом. Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.|

## <a name="relationships"></a>Связи
None

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



