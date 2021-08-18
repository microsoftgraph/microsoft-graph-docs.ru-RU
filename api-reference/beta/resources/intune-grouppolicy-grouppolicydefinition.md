---
title: тип ресурса groupPolicyDefinition
description: Объект описывает всю информацию о единой групповой политике.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ab46b69ca78f6b7eac9707fc0f6b20bb973c3a48
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265384"
---
# <a name="grouppolicydefinition-resource-type"></a>тип ресурса groupPolicyDefinition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект описывает всю информацию о единой групповой политике.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Чтение свойств и связей объекта [groupPolicyDefinition.](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|[Update groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Обновление свойств объекта [groupPolicyDefinition.](../resources/intune-grouppolicy-grouppolicydefinition.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Определяет тип групп, к которые можно применить политику. Возможные значения: `user`, `machine`.|
|displayName|Строка|Имя локализованной политики.|
|explainText|String|Локализованный текст объяснения или справки, связанные с политикой. По умолчанию это значение пусто.|
|categoryPath|String|Путь к локализованным полным категориям для политики.|
|supportedOn|Строка|Локализованная строка, используемая для указания того, на какую операционную систему или версию приложения влияет политика.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Возможные значения: `admxBacked`, `admxIngested`.|
|hasRelatedDefinitions|Логический|Означает, есть ли связанные определения с этим определением или нет.|
|groupPolicyCategoryId|Guid|ID категории родительской категории|
|version|String|Настройка версии определения|
|id|Строка|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Файл групповой политики, связанный с определением.|
|category|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Категория групповой политики, связанная с определением.|
|презентации|[коллекция groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|Презентации групповой политики, связанные с определением.|
|previousVersionDefinition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение предыдущей версии этого определения|
|nextVersionDefinition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определение следующей версии этого определения|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "Guid",
  "version": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




