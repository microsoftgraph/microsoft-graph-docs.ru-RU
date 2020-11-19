---
title: Тип ресурса Граупполицидефинитионфиле
description: Сущность представляет XML-файл ADMX (административный шаблон). ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 89db03a54e2bbed52a4bc24266136cf9af272215
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259762"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>Тип ресурса Граупполицидефинитионфиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет XML-файл ADMX (административный шаблон). ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Граупполицидефинитионфиле](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Чтение свойств и связей объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|
|[Обновление Граупполицидефинитионфиле](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Обновление свойств объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Локализованное понятное имя файла ADMX.|
|description|String|Локализованное описание параметров политики в файле ADMX. По умолчанию это значение пусто.|
|лангуажекодес|Коллекция строк|Поддерживаемые коды языков для ADMX.|
|таржетпрефикс|String|Задает логическое имя, которое ссылается на пространство имен в файле ADMX.|
|Атрибут|String|Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.|
|полицитипе|[граупполицитипе](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Возможные значения: `admxBacked`, `admxIngested`.|
|последним|String|Версия редакции, связанная с файлом.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определения|Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определения групповой политики, связанные с файлом.|

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




