---
title: Тип ресурса Граупполициуплоадеддефинитионфиле
description: Сущность представляет XML-файл ADMX (административный шаблон), переданный администратором. ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2399555f5c7e63b595ef211089ddcc16cae7f8e3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298227"
---
# <a name="grouppolicyuploadeddefinitionfile-resource-type"></a>Тип ресурса Граупполициуплоадеддефинитионфиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность представляет XML-файл ADMX (административный шаблон), переданный администратором. ADMX-файл содержит коллекцию определений групповой политики и их расположение по пути к категории. В файле определения групповой политики также содержатся языки, поддерживаемые в зависимости от языковых файлов ADML (административного шаблона).


Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Граупполициуплоадеддефинитионфилес](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-list.md)|Коллекция [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Список свойств и связей объектов [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .|
|[Получение Граупполициуплоадеддефинитионфиле](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-get.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Чтение свойств и связей объекта [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .|
|[Создание Граупполициуплоадеддефинитионфиле](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-create.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Создание нового объекта [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .|
|[Удаление Граупполициуплоадеддефинитионфиле](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-delete.md)|Нет|Удаляет объект [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md).|
|[Обновление Граупполициуплоадеддефинитионфиле](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-update.md)|[groupPolicyUploadedDefinitionFile](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md)|Обновление свойств объекта [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .|
|[действие Аддлангуажефилес](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-addlanguagefiles.md)|Нет|Н/Д|
|[действие Ремовелангуажефилес](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-removelanguagefiles.md)|Нет|Н/Д|
|[действие Упдателангуажефилес](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-updatelanguagefiles.md)|Нет|Н/Д|
|[действие Уплоадневверсион](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-uploadnewversion.md)|Нет|Н/Д|
|[удалить действие](../api/intune-grouppolicy-grouppolicyuploadeddefinitionfile-remove.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Локализованное понятное имя файла ADMX. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|description|String|Локализованное описание параметров политики в файле ADMX. По умолчанию это значение пусто. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|лангуажекодес|Коллекция строк|Поддерживаемые коды языков для ADMX. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|таржетпрефикс|String|Задает логическое имя, которое ссылается на пространство имен в файле ADMX. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|Атрибут|String|Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|полицитипе|[граупполицитипе](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md). Возможные значения: `admxBacked`, `admxIngested`.|
|последним|String|Версия редакции, связанная с файлом. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|id|String|Ключ объекта. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|fileName|String|Имя файла загруженного файла ADML.|
|status|[groupPolicyUploadedDefinitionFileStatus](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|Состояние отправки для отправленного ADMX файла. Возможные значения: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|содержимое|Binary|Содержимое отправленного ADMX файла.|
|уплоаддатетиме|DateTimeOffset|Время отправки файла ADMX.|
|дефаултлангуажекоде|String|Язык по умолчанию для отправленного файла ADMX.|
|граупполициуплоадедлангуажефилес|Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)|Список файлов ADML, связанных с отправленным ADMX файлом.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|определения|Коллекция [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|Определения групповой политики, связанные с файлом. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|граупполициоператионс|Коллекция [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md)|Список операций для отправленного ADMX файл.|

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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "fileName": "String",
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




