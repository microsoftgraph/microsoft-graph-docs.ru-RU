---
title: Обновление win32LobApp
description: Обновление свойств объекта win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e3311aa409752353b3be63915a938a620e3aca2
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793250"
---
# <a name="update-win32lobapp"></a>Обновление win32LobApp

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) .

## <a name="prerequisites"></a>Необходимые компоненты
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [win32LobApp](../resources/intune-apps-win32lobapp.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [win32LobApp](../resources/intune-apps-win32lobapp.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|displayName|Строка|Название приложения, которое предоставил или импортировал администратор. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|description|Строка|Описание приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publisher|String|Издатель приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|largeIcon|[mimeContent](../resources/intune-shared-mimecontent.md)|Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|createdDateTime|DateTimeOffset|Дата и время создания приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|isFeatured|Boolean|Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-shared-mobileapp.md).|
|privacyInformationUrl|String|URL-адрес заявления о конфиденциальности. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|informationUrl|String|URL-адрес страницы с дополнительными сведениями. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|owner|String|Владелец приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|developer|String|Разработчик приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|notes|String|Заметки для приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|uploadState|Int32|Состояние отправки. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|publishingState|[мобилеапппублишингстате](../resources/intune-apps-mobileapppublishingstate.md)|Состояние публикации для приложения. Приложение невозможно назначить, если оно не опубликовано. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md). Возможные значения: `notPublished`, `processing`, `published`.|
|isAssigned|Boolean|Значение, указывающее, назначено ли приложение по крайней мере одной группе. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|roleScopeTagIds|Коллекция String|Список идентификаторов тегов области для этого мобильного приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|депендентаппкаунт|Int32|Общее количество зависимостей для дочернего приложения. Наследуется от [mobileApp](../resources/intune-shared-mobileapp.md).|
|committedContentVersion|String|Внутренняя версия подтвержденного содержимого. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|fileName|String|Имя основного файла бизнес-приложения. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|size|Int64|Общий размер, включая все отправленные файлы. Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).|
|инсталлкоммандлине|String|Командная строка для установки приложения|
|унинсталлкоммандлине|String|Командная строка для удаления приложения|
|applicableArchitectures|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Архитектура Windows, которая поддерживается этим приложением. Возможные значения: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|Значение, которое представляет минимальную применимую версию операционной системы.|
|минимумфридискспацеинмб|Int32|Минимальное свободное место на диске, необходимое для установки этого приложения.|
|минимуммеморинмб|Int32|Значение минимальной физической памяти, необходимой для установки этого приложения.|
|минимумнумберофпроцессорс|Int32|Значение минимального числа процессоров, необходимое для установки этого приложения.|
|минимумкпуспидинмхз|Int32|Значение минимальной скорости ЦП, необходимое для установки этого приложения.|
|детектионрулес|Коллекция [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)|Правила обнаружения для определения бизнес-приложения Win32 (LoB).|
|рекуирементрулес|Коллекция [win32LobAppRequirement](../resources/intune-apps-win32lobapprequirement.md)|Правила требований для обнаружения бизнес-приложения Win32.|
|правила|Коллекция [win32LobAppRule](../resources/intune-apps-win32lobapprule.md)|Правила обнаружения и требований для этого приложения.|
|инсталлекспериенце|[win32LobAppInstallExperience](../resources/intune-apps-win32lobappinstallexperience.md)|Установка приложения.|
|ретурнкодес|Коллекция [win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)|Коды возврата для поведения после установки.|
|мсиинформатион|[win32LobAppMsiInformation](../resources/intune-apps-win32lobappmsiinformation.md)|Сведения о MSI, если это приложение Win32 является приложением MSI.|
|сетупфилепас|String|Относительный путь к файлу установки в зашифрованном пакете Win32LobApp.|
|installLanguage|String|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [win32LobApp](../resources/intune-apps-win32lobapp.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 3224

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```

### <a name="response"></a>Отклик
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3396

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1,
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  },
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRequirement",
      "operator": "equal",
      "detectionValue": "Detection Value value",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "installLanguage": "Install Language value"
}
```



