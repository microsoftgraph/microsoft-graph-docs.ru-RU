---
title: тип ресурса groupPolicyDefinitionFile
description: Объект представляет XML-файл ADMX (Административный шаблон). Файл ADMX содержит коллекцию определений групповой политики и их расположения по категориям. Файл определения групповой политики также содержит языки, поддерживаемые языковыми файлами ADML (Административный шаблон).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70f502578f7291a3dab89d37b0aa4722ea8ff9a1
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292062"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>тип ресурса groupPolicyDefinitionFile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет XML-файл ADMX (Административный шаблон). Файл ADMX содержит коллекцию определений групповой политики и их расположения по категориям. Файл определения групповой политики также содержит языки, поддерживаемые языковыми файлами ADML (Административный шаблон).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Чтение свойств и связей объекта [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|
|[Update groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Обновление свойств объекта [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Локализованное удобное имя файла ADMX.|
|description|String|Локализованное описание параметров политики в файле ADMX. По умолчанию это значение пусто.|
|languageCodes|Коллекция строк|Поддерживаемые языковые коды для файла ADMX.|
|targetPrefix|String|Указывает логическое имя, которое ссылается на пространство имен в файле ADMX.|
|targetNamespace|String|Указывает URI, используемую для определения пространства имен в файле ADMX.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Возможные значения: `admxBacked`, `admxIngested`.|
|изменение|String|Версия изменения, связанная с файлом.|
|fileName|String|Имя файла файла ADMX без пути. Например: edge.admx|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определения|[коллекция groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определения групповой политики, связанные с файлом.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "revision": "String",
  "fileName": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




