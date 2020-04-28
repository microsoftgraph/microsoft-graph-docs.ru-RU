---
title: Обновление Енроллментрестриктионсконфигуратионполицисетитем
description: Обновление свойств объекта Енроллментрестриктионсконфигуратионполицисетитем.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c3b2338e2f4ea97a9f1e20daecde7e6aa8f1943
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424125"
---
# <a name="update-enrollmentrestrictionsconfigurationpolicysetitem"></a>Обновление Енроллментрестриктионсконфигуратионполицисетитем

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) .

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
PATCH /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Мобилеаппполицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Время создания Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|пайлоадид|String|Пайлоадид Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|itemType|String|Полицисеттипе Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|displayName|Строка|DisplayName объекта Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Состояние Полицисетитем. Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Код ошибки (при возникновении ошибки). Наследуется от [полицисетитем](../resources/intune-policyset-policysetitem.md). Возможные значения: `noError`, `unauthorized`, `notFound`, `deleted`.|
|гуидеддеплойменттагс|Коллекция объектов string|Теги управляемого развертывания, унаследованные от [полицисетитем](../resources/intune-policyset-policysetitem.md)|
|priority|Int32|Приоритет Енроллментрестриктионсконфигуратионполицисетитем.|
|limit|Int32|Ограничения для Енроллментрестриктионсконфигуратионполицисетитем.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [енроллментрестриктионсконфигуратионполицисетитем](../resources/intune-policyset-enrollmentrestrictionsconfigurationpolicysetitem.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8,
  "limit": 5
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "@odata.type": "#microsoft.graph.enrollmentRestrictionsConfigurationPolicySetItem",
  "id": "08c4f0b1-f0b1-08c4-b1f0-c408b1f0c408",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "validating",
  "errorCode": "unauthorized",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ],
  "priority": 8,
  "limit": 5
}
```



