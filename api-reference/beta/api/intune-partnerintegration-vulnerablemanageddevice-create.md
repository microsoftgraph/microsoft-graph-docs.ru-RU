---
title: Создание Вулнераблеманажеддевице
description: Создание нового объекта Вулнераблеманажеддевице.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d9bab17be811156f9aa0efcae52f024388f260d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270416"
---
# <a name="create-vulnerablemanageddevice"></a>Создание Вулнераблеманажеддевице

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementApps.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Вулнераблеманажеддевице в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Вулнераблеманажеддевице.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ сущности и идентификатор устройства AAD.|
|манажеддевицеид|String|Идентификатор управляемого устройства Intune.|
|displayName|String|Имя устройства.|
|lastSyncDateTime|DateTimeOffset|Дата последней синхронизации.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
Content-type: application/json
Content-length: 214

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 263

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "id": "e59891d4-91d4-e598-d491-98e5d49198e5",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```




