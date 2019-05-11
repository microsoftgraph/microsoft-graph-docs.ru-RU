---
title: Создание Виндовсоффицеклиентконфигуратион
description: Создайте новую политику, не являющуюся политикой безопасности, с целевыми группами.
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 87b30f78cd2c5bf8c97b3b08f2db490152767c0d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934000"
---
# <a name="create-windowsofficeclientconfiguration"></a>Создание Виндовсоффицеклиентконфигуратион

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новую политику, не являющуюся политикой безопасности, с целевыми группами.

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта [Виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор политики конфигурации клиента Office. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Усерпреференцепайлоад|Stream|Строка JSON параметров настройки в двоичном формате. Эти значения могут быть переопределены пользователем. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Полиципайлоад|Stream|Строка JSON параметров политики в двоичном формате эти значения не могут быть изменены пользователем. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|description|String|Администратор предоставил описание политики конфигурации клиента Office. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|displayName|Строка|Предоставленное администратором имя политики конфигурации клиента Office. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|assignments|Коллекция [оффицеклиентконфигуратионассигнмент](../resources/intune-cirrus-officeclientconfigurationassignment.md)|Список назначений групп для политики.. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|priority|Int32|Значение Priority должно быть уникальным для каждой политики в клиенте и использоваться для разрешения конфликтов, низкие значения имеют высокий приоритет. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|lastModifiedDateTime|DateTime|Метка даты и времени последнего изменения политики. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Усерчеккинсуммари|[officeUserCheckinSummary](../resources/intune-cirrus-officeusercheckinsummary.md)|Сводка по возврату пользователя для политики. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|
|Чеккинстатусес|Коллекция [оффицеклиентчеккинстатус](../resources/intune-cirrus-officeclientcheckinstatus.md)|Список состояния возврата клиента Office. Наследуется от [officeClientConfiguration](../resources/intune-cirrus-officeclientconfiguration.md)|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [виндовсоффицеклиентконфигуратион](../resources/intune-cirrus-windowsofficeclientconfiguration.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations
Content-type: application/json
Content-length: 1020

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1069

{
  "@odata.type": "#microsoft.graph.windowsOfficeClientConfiguration",
  "id": "13a5ac73-ac73-13a5-73ac-a51373aca513",
  "userPreferencePayload": "<Unknown Primitive Type Edm.Stream>",
  "policyPayload": "<Unknown Primitive Type Edm.Stream>",
  "description": "Description value",
  "displayName": "Display Name value",
  "priority": 8,
  "userCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  },
  "checkinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "userId": "User Id value",
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ]
    }
  ]
}
```



