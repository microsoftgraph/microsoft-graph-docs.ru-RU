---
title: Создание deviceManagementScript
description: Создание нового объекта deviceManagementScript.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a46e5eed8a4b5c678c9510d7471e3b7dc450ccb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959280"
---
# <a name="create-devicemanagementscript"></a>Создание deviceManagementScript

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

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
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта deviceManagementScript в формате JSON.

В следующей таблице приведены свойства, необходимые при создании deviceManagementScript.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сценария управления устройствами.|
|displayName|Строка|Имя скрипта управления устройствами.|
|description|String|НеОбязательное описание скрипта управления устройствами.|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|Интервал для запуска скрипта. Если не определен, сценарий будет выполняться один раз|
|Скриптконтент|Binary|Содержимое скрипта.|
|createdDateTime|DateTimeOffset|Дата и время создания сценария управления устройствами.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения скрипта управления устройствами.|
|runAsAccount|[Рунасаккаунттипе](../resources/intune-shared-runasaccounttype.md)|Указывает тип контекста выполнения. Возможные значения: `system`, `user`.|
|Свойства enforcesignaturecheck|Boolean|Указывает, нужно ли проверять подпись скрипта.|
|fileName|String|Имя файла сценария.|
|roleScopeTagIds|Коллекция строк|Список идентификаторов тегов области для этого экземпляра Повершеллскрипт.|
|runAs32Bit|Boolean|Значение, указывающее, должен ли скрипт PowerShell выполняться как 32 бит|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [deviceManagementScript](../resources/intune-devices-devicemanagementscript.md) в тексте отклика.

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
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
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




