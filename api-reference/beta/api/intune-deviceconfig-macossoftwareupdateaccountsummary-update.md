---
title: Обновление macOSSoftwareUpdateAccountSummary
description: Обновление свойств объекта macOSSoftwareUpdateAccountSummary.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 356ac6f22ee82d2abb09768e12b822a8942db42a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59112750"
---
# <a name="update-macossoftwareupdateaccountsummary"></a>Обновление macOSSoftwareUpdateAccountSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
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
PATCH /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)

В следующей таблице показаны свойства, необходимые при создании [macOSSoftwareUpdateAccountSummary.](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Имя отчета|
|deviceId|String|ID устройства.|
|userId|String|Идентификатор пользователя.|
|deviceName|String|Имя устройства.|
|userPrincipalName|String|Имя основного пользователя|
|osVersion|String|Версия ОС.|
|successfulUpdateCount|Int32|Количество успешных обновлений на устройстве.|
|failedUpdateCount|Int32|Количество сбойных обновлений на устройстве.|
|totalUpdateCount|Int32|Количество обновлений на устройстве.|
|lastUpdatedDateTime|DateTimeOffset|Последняя дата обновления отчета для этого устройства.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект macOSSoftwareUpdateAccountSummary](../resources/intune-deviceconfig-macossoftwareupdateaccountsummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}
Content-type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateAccountSummary",
  "id": "64687d05-7d05-6468-057d-6864057d6864",
  "displayName": "Display Name value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "userPrincipalName": "User Principal Name value",
  "osVersion": "Os Version value",
  "successfulUpdateCount": 5,
  "failedUpdateCount": 1,
  "totalUpdateCount": 0,
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```



