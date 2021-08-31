---
title: тип ресурса groupPolicyDefinitionFile
description: Объект представляет XML-файл ADMX (Административный шаблон). Файл ADMX содержит коллекцию определений групповой политики и их расположения по категориям. Файл определения групповой политики также содержит языки, поддерживаемые языковыми файлами ADML (Административный шаблон).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 887c1b3b8b744e45b265fedff2bd2b5fd767fe4b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796196"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>тип ресурса groupPolicyDefinitionFile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет XML-файл ADMX (Административный шаблон). Файл ADMX содержит коллекцию определений групповой политики и их расположения по категориям. Файл определения групповой политики также содержит языки, поддерживаемые языковыми файлами ADML (Административный шаблон).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Чтение свойств и связей объекта [groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|[Update groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Обновление свойств объекта [groupPolicyDefinitionFile.](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Локализованное удобное имя файла ADMX.|
|description|Строка|Локализованное описание параметров политики в файле ADMX. По умолчанию это значение пусто.|
|languageCodes|Коллекция String|Поддерживаемые языковые коды для файла ADMX.|
|targetPrefix|Строка|Указывает логическое имя, которое ссылается на пространство имен в файле ADMX.|
|targetNamespace|Строка|Указывает URI, используемую для определения пространства имен в файле ADMX.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Возможные значения: `admxBacked`, `admxIngested`.|
|изменение|Строка|Версия изменения, связанная с файлом.|
|id|Строка|Ключ объекта.|
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



