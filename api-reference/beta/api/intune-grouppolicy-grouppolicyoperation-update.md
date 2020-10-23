---
title: Обновление Граупполициоператион
description: Обновление свойств объекта Граупполициоператион.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f3b6ddd3657e9689e8950ab21207040dfceda16e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724173"
---
# <a name="update-grouppolicyoperation"></a>Обновление Граупполициоператион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) .

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
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|оператионтипе|[groupPolicyOperationType](../resources/intune-grouppolicy-grouppolicyoperationtype.md)|Тип операции с групповой политикой. Возможные значения: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|оператионстатус|[groupPolicyOperationStatus](../resources/intune-grouppolicy-grouppolicyoperationstatus.md)|Состояние операции групповой политики. Возможные значения: `unknown`, `inProgress`, `success`, `failed`.|
|статусдетаилс|Строка|Сведения о состоянии операции групповой политики.|
|id|Строка|Ключ объекта.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполициоператион](../resources/intune-grouppolicy-grouppolicyoperation.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/microsoft.graph.groupPolicyUploadedDefinitionFile/groupPolicyOperations/{groupPolicyOperationId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "upload",
  "operationStatus": "inProgress",
  "statusDetails": "Status Details value",
  "id": "4d18865b-865b-4d18-5b86-184d5b86184d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





