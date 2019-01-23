---
title: Тип ресурса groupPolicyDefinitionFile
description: Объект представляет ADMX (административных шаблонов) XML-файла. Файл ADMX содержит коллекцию определений групповой политики и их расположение по пути к категории. Файл определения групповой политике также содержит языки, поддерживаемые согласно языковых файлов языка зависимые ADML (административный шаблон).
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431711"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>Тип ресурса groupPolicyDefinitionFile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет ADMX (административных шаблонов) XML-файла. Файл ADMX содержит коллекцию определений групповой политики и их расположение по пути к категории. Файл определения групповой политике также содержит языки, поддерживаемые согласно языковых файлов языка зависимые ADML (административный шаблон).

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Чтение свойства и связи объекта [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|
|[Обновление groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Обновление свойства объекта [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Локализованные понятное имя файла ADMX.|
|description|String|Локализованное описание параметров политики в ADMX-файле. Значение по умолчанию будет пустым.|
|languageCodes|Коллекция String|Коды поддерживаемых языков для файлов ADMX.|
|targetPrefix|String|Задает логическое имя, которое относится к области имен файлах.|
|targetNamespace|String|Указывает URI, используемый для идентификации пространства имен в файле ADMX.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Возможные значения: `admxBacked`, `admxIngested`.|
|id|String|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|определения|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) коллекции|Определения групповой политики, связанные с этим файлом.|

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




