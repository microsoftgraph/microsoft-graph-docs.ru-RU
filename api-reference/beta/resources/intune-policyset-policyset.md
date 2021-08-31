---
title: Тип ресурса policySet
description: Класс, содержащий свойства, используемые для PolicySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: edac97723f19b494adcb38ed87b68695c31bd367
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793290"
---
# <a name="policyset-resource-type"></a>Тип ресурса policySet

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для PolicySet.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Списки политикSets](../api/intune-policyset-policyset-list.md)|[коллекция policySet](../resources/intune-policyset-policyset.md)|Список свойств и связей объектов [policySet.](../resources/intune-policyset-policyset.md)|
|[Get policySet](../api/intune-policyset-policyset-get.md)|[policySet](../resources/intune-policyset-policyset.md)|Чтение свойств и связей объекта [policySet.](../resources/intune-policyset-policyset.md)|
|[Создание policySet](../api/intune-policyset-policyset-create.md)|[policySet](../resources/intune-policyset-policyset.md)|Создание нового [объекта policySet.](../resources/intune-policyset-policyset.md)|
|[Удаление policySet](../api/intune-policyset-policyset-delete.md)|Нет|Удаляет набор [политик.](../resources/intune-policyset-policyset.md)|
|[Update policySet](../api/intune-policyset-policyset-update.md)|[policySet](../resources/intune-policyset-policyset.md)|Обновление свойств объекта [policySet.](../resources/intune-policyset-policyset.md)|
|[Действие обновления](../api/intune-policyset-policyset-update.md)|Нет|Н/Д|
|[действие getPolicySets](../api/intune-policyset-policyset-getpolicysets.md)|[коллекция policySet](../resources/intune-policyset-policyset.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша PolicySet.|
|createdDateTime|DateTimeOffset|Время создания PolicySet.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время в PolicySet.|
|displayName|Строка|DisplayName of the PolicySet.|
|description|Строка|Описание PolicySet.|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Проверка/присвоение состояния PolicySet. Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки, если таковое произошло. Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Коллекция String|Теги управляемого развертывания|
|roleScopeTags|Коллекция String|RoleScopeTags of the PolicySet|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|[коллекция policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Назначения PolicySet.|
|элементы|[коллекция policySetItem](../resources/intune-policyset-policysetitem.md)|Элементы PolicySet с максимальным количеством 100.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySet",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "roleScopeTags": [
    "String"
  ]
}
```



