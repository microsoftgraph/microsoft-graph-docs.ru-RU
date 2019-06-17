---
title: Тип ресурса Граупполицидефинитионфиле
description: Сущность представляет XML-файл ADMX (административный шаблон). ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a872671186e55524002b2d0a5f85b2ce1bbf2466
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975940"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>Тип ресурса Граупполицидефинитионфиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет XML-файл ADMX (административный шаблон). ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Граупполицидефинитионфиле](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[Граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Чтение свойств и связей объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|
|[Обновление Граупполицидефинитионфиле](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[Граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Обновление свойств объекта [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Локализованное понятное имя файла ADMX.|
|description|String|Локализованное описание параметров политики в файле ADMX. По умолчанию это значение пусто.|
|Лангуажекодес|Коллекция строк|Поддерживаемые коды языков для ADMX.|
|Таржетпрефикс|String|Задает логическое имя, которое ссылается на пространство имен в файле ADMX.|
|Атрибут|String|Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX.|
|Полицитипе|[Граупполицитипе](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Возможные значения: `admxBacked`, `admxIngested`.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```





