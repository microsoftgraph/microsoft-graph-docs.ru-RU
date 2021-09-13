---
title: тип ресурса groupPolicyConfiguration
description: Объект конфигурации групповой политики содержит настроенные значения для одного или более определений групповой политики.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e46f23dc14427b9f4c7feb55f9538b010574b508
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063897"
---
# <a name="grouppolicyconfiguration-resource-type"></a>тип ресурса groupPolicyConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект конфигурации групповой политики содержит настроенные значения для одного или более определений групповой политики.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[коллекция groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Список свойств и связей объектов [groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[Get groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Чтение свойств и связей объекта [groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[Создание groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Создайте новый [объект groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[Удаление groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|Нет|Удаляет [группуPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[Update groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Обновление свойств объекта [groupPolicyConfiguration.](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|
|[Действие assign](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[коллекция groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Пока не задокументировано.|
|[updateDefinitionValues action](../api/intune-grouppolicy-grouppolicyconfiguration-updatedefinitionvalues.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Дата и время создания объекта.|
|displayName|String|Пользователь предоставил имя объекта ресурса.|
|description|String|Пользователь предоставил описание объекта ресурса.|
|roleScopeTagIds|Коллекция String|Список тегов области для конфигурации.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|definitionValues|[коллекция groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Список значений определения групповой политики включенной или отключенной для конфигурации.|
|assignments|[коллекция groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|Список групповых назначений для конфигурации.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



