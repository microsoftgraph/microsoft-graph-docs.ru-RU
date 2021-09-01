---
title: Тип ресурса resourceOperation
description: Описывает ресурс resourceOperation (сущность) API microsoft Graph (REST), который поддерживает процессы intune, связанные с управлением доступом на основе ролей (RBAC).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6495d80c548f3847dd7ac88adcb3f92b14c04409
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58807644"
---
# <a name="resourceoperation-resource-type"></a>Тип ресурса resourceOperation

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

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
|[функция getScopesForUser](../api/intune-rbac-resourceoperation-getscopesforuser.md)|Коллекция строк|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ операции с ресурсом. Доступен только для чтения и создается автоматически.|
|resource|String|Категория ресурсов, к которой относится эта операция. Это свойство доступно только для чтения.|
|resourceName|String|Имя ресурса, с которым выполняется эта операция.|
|actionName|String|Тип действия, которое выполнит эта операция. Свойство actionName должно быть максимально краткое (максимум несколько слов).|
|description|Строка|Описание операции с ресурсом. Используется в тексте, который отображается над операцией при наведении указателя мыши на портале Azure.|
|enabledForScopeValidation|Логический|Определяет, проверяется ли разрешение для областей, определенных для назначения ролей. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
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
  "resource": "String",
  "resourceName": "String",
  "actionName": "String",
  "description": "String",
  "enabledForScopeValidation": true
}
```



