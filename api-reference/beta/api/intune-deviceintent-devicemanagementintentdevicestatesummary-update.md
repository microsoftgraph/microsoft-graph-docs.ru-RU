---
title: Обновление deviceManagementIntentDeviceStateSummary
description: Обновление свойств объекта deviceManagementIntentDeviceStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5cf6c13b3e1fc2a886109dfe0a8a111942ca817
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795993"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a>Обновление deviceManagementIntentDeviceStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceManagementIntentDeviceStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта deviceManagementIntentDeviceStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)

В следующей таблице показаны свойства, необходимые при создании [устройстваManagementIntentDeviceStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|The ID|
|conflictCount|Int32|Количество устройств в конфликте|
|errorCount|Int32|Количество устройств с ошибками.|
|failedCount|Int32|Число устройств со сбоями.|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|notApplicablePlatformCount|Int32|Количество не применимых устройств из-за несоответствия платформы и политики|
|successCount|Int32|Количество успешных устройств.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
Content-type: application/json
Content-length: 237

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "12230bf9-0bf9-1223-f90b-2312f90b2312",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```



