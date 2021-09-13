---
title: Создание cloudPCConnectivityIssue
description: Создание нового объекта cloudPCConnectivityIssue.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 559b7746003009a7095944128d4560f169ca0ae4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59059142"
---
# <a name="create-cloudpcconnectivityissue"></a>Создание cloudPCConnectivityIssue

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта cloudPCConnectivityIssue.](../resources/intune-devices-cloudpcconnectivityissue.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cloudPCConnectivityIssues
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта cloudPCConnectivityIssue.

В следующей таблице показаны свойства, необходимые при создании cloudPCConnectivityIssue.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта событий событий для аналитики пользовательского интерфейса.|
|deviceId|String|Устройство Intune устройства, с которое связано подключение.|
|errorCode|String|Код ошибки проблемы подключения.|
|errorDateTime|DateTimeOffset|Время начала подключения. Время отображается в формате ISO 8601 и времени скоординированного универсального времени (UTC).|
|userId|String|Уникальный id пользователя, который инициализирует подключение.|
|errorDescription|String|Подробное описание того, что пошло не так.|
|recommendedAction|Строка|Рекомендуемое действие для устранения соответствующей ошибки.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "e8e2bf5f-bf5f-e8e2-5fbf-e2e85fbfe2e8",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```



