---
title: тип ресурса groupPolicyUploadedDefinitionFile
description: Объект представляет XML-файл ADMX (Административный шаблон), загруженный администратором. Файл ADMX содержит коллекцию определений групповой политики и их расположения по категориям. Файл определения групповой политики также содержит языки, поддерживаемые языковыми файлами ADML (Административный шаблон).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 75598441e686607d4d1162d1b16c600983ccbeaa
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291894"
---
# <a name="grouppolicyuploadeddefinitionfile-resource-type"></a>тип ресурса groupPolicyUploadedDefinitionFile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект представляет XML-файл ADMX (Административный шаблон), загруженный администратором. Файл ADMX содержит коллекцию определений групповой политики и их расположения по категориям. Файл определения групповой политики также содержит языки, поддерживаемые языковыми файлами ADML (Административный шаблон).


Наследует от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[List groupPolicyUploadedDefinitionFiles](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-list.md)|[коллекция groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Список свойств и связей [объектов groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .|
|[Get groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-get.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Чтение свойств и связей объекта [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .|
|[Создание groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-create.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Создайте новый [объект GroupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .|
|[Удаление groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-delete.md)|Нет|Удаляет [группуPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md).|
|[Update groupPolicyUploadedDefinitionFile](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-update.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Обновление свойств объекта [groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .|
|[действие addLanguageFiles](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-addlanguagefiles.md)|Нет|Н/Д|
|[removeLanguageFiles action](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-removelanguagefiles.md)|Нет|Н/Д|
|[updateLanguageFiles action](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-updatelanguagefiles.md)|Нет|Н/Д|
|[uploadNewVersion action](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-uploadnewversion.md)|Нет|Н/Д|
|[удаление действия](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-remove.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Локализованное удобное имя файла ADMX. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|description|String|Локализованное описание параметров политики в файле ADMX. По умолчанию это значение пусто. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|languageCodes|Коллекция объектов string|Поддерживаемые языковые коды для файла ADMX. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetPrefix|String|Указывает логическое имя, которое ссылается на пространство имен в файле ADMX. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|targetNamespace|String|Указывает URI, используемую для определения пространства имен в файле ADMX. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Наследуется [от groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md). Возможные значения: `admxBacked`, `admxIngested`.|
|изменение|String|Версия изменения, связанная с файлом. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|fileName|String|Имя файла файла ADMX без пути. Например: edge.admx Inherited from [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|status|[groupPolicyUploadedDefinitionFileStatus](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|Состояние загрузки загруженного файла ADMX. Возможные значения: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|содержимое|Binary|Содержимое загруженного файла ADMX.|
|uploadDateTime|DateTimeOffset|Время загрузки загруженного файла ADMX.|
|defaultLanguageCode|String|Язык по умолчанию загруженного файла ADMX.|
|groupPolicyUploadedLanguageFiles|[коллекция groupPolicyUploadedLanguageFile](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)|Список ADML-файлов, связанных с загруженным ADMX-файлом.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определения|[коллекция groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определения групповой политики, связанные с файлом. Унаследованный от [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|groupPolicyOperations|[коллекция groupPolicyOperation](../resources/intune-grouppolicy-grouppolicyoperation.md)|Список операций в загруженных файлах ADMX.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
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
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "content": "binary",
  "uploadDateTime": "String (timestamp)",
  "defaultLanguageCode": "String",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "String",
      "languageCode": "String",
      "content": "binary",
      "id": "String",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```




