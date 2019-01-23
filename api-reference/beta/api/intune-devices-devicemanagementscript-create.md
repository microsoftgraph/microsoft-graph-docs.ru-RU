---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be0ffb8b912b25684ba0ed3dc383a995fb872f3b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409274"
---
# <a name="create-devicemanagementscript"></a>Создание deviceManagementScript

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .

## <a name="prerequisites"></a>Предварительные требования
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Authorization|Требуется Bearer &lt;маркер&gt;
|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите представление JSON для объекта deviceManagementScript.

В следующей таблице показаны свойства, которые необходимы для создания deviceManagementScript.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для сценарий управления устройства.|
|displayName|String|Имя скрипта управления устройства.|
|description|String|Необязательное описание сценарий управления устройства.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Интервал для запуска сценария. Если не определена сценарий будет выполняться один раз|
|scriptContent|Binary|Содержимое сценария.|
|createdDateTime|DateTimeOffset|Дата и время создания сценарий управления устройства.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения сценарий управления устройства.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения скрипта управления устройства выполняется в. Возможные значения: `system`, `user`.|
|enforceSignatureCheck|Логический|Указывает, должно быть извлеченных подписи скрипта.|
|fileName|String|Имя файла сценария.|
|roleScopeTagIds|Коллекция String|Список идентификаторов тег области для этого экземпляра PowerShellScript.|
|runAs32Bit|Логический|Значение, указывающее ли сценарий PowerShell должна запускаться в 32-разрядная версия|



## <a name="response"></a>Отклик
Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в теле ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts
Content-type: application/json
Content-length: 443

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 615

{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "59ea4525-4525-59ea-2545-ea592545ea59",
  "displayName": "Display Name value",
  "description": "Description value",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "c2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "fileName": "File Name value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "runAs32Bit": true
}
```




