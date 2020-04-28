---
title: Создание Граупполициуплоадеддефинитионфиле
description: Создание нового объекта Граупполициуплоадеддефинитионфиле.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 828464d5a0e620a713eac7187b6a8883ea7a2648
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43388652"
---
# <a name="create-grouppolicyuploadeddefinitionfile"></a>Создание Граупполициуплоадеддефинитионфиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyUploadedDefinitionFiles
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Граупполициуплоадеддефинитионфиле в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Граупполициуплоадеддефинитионфиле.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|Строка|Локализованное понятное имя файла ADMX. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|description|String|Локализованное описание параметров политики в файле ADMX. По умолчанию это значение пусто. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|лангуажекодес|Коллекция объектов string|Поддерживаемые коды языков для ADMX. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|таржетпрефикс|String|Задает логическое имя, которое ссылается на пространство имен в файле ADMX. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|Атрибут|String|Указывает универсальный код ресурса (URI), используемый для идентификации пространства имен в файле ADMX. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|полицитипе|[граупполицитипе](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md). Возможные значения: `admxBacked`, `admxIngested`.|
|последним|String|Версия редакции, связанная с файлом. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|id|Строка|Ключ объекта. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполицидефинитионфиле](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|
|fileName|String|Имя файла загруженного файла ADML.|
|status|[groupPolicyUploadedDefinitionFileStatus](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfilestatus.md)|Состояние отправки для отправленного ADMX файла. Возможные значения: `none`, `uploadInProgress`, `available`, `assigned`, `removalInProgress`, `uploadFailed`, `removalFailed`.|
|содержимое|Binary|Содержимое отправленного ADMX файла.|
|уплоаддатетиме|DateTimeOffset|Время отправки файла ADMX.|
|дефаултлангуажекоде|String|Язык по умолчанию для отправленного файла ADMX.|
|граупполициуплоадедлангуажефилес|Коллекция [граупполициуплоадедлангуажефиле](../resources/intune-grouppolicy-grouppolicyuploadedlanguagefile.md)|Список файлов ADML, связанных с отправленным ADMX файлом.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициуплоадеддефинитионфиле](../resources/intune-grouppolicy-grouppolicyuploadeddefinitionfile.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyUploadedDefinitionFiles
Content-type: application/json
Content-length: 922

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1035

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "0ce1a8cf-a8cf-0ce1-cfa8-e10ccfa8e10c",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "fileName": "File Name value",
  "status": "uploadInProgress",
  "content": "Y29udGVudA==",
  "uploadDateTime": "2016-12-31T23:58:46.5747426-08:00",
  "defaultLanguageCode": "Default Language Code value",
  "groupPolicyUploadedLanguageFiles": [
    {
      "@odata.type": "microsoft.graph.groupPolicyUploadedLanguageFile",
      "fileName": "File Name value",
      "languageCode": "Language Code value",
      "content": "Y29udGVudA==",
      "id": "Id value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```



