---
title: Создание deviceManagementIntentDeviceSettingStateSummary
description: Создайте новый объект deviceManagementIntentDeviceSettingStateSummary.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1cca0fac75efad84fe2c77321cf1adad2679d39
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59018357"
---
# <a name="create-devicemanagementintentdevicesettingstatesummary"></a>Создание deviceManagementIntentDeviceSettingStateSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект deviceManagementIntentDeviceSettingStateSummary.](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В корпусе запроса поставляем представление JSON для объекта deviceManagementIntentDeviceSettingStateSummary.

В следующей таблице показаны свойства, необходимые при создании устройстваManagementIntentDeviceSettingStateSummary.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|The ID|
|settingName|String|Имя параметра|
|compliantCount|Int32|Количество устройств, соответствующих требованиям.|
|conflictCount|Int32|Количество устройств в конфликте|
|errorCount|Int32|Количество устройств с ошибками.|
|nonCompliantCount|Int32|Число устройств, не совместимых с соответствием требованиям|
|notApplicableCount|Int32|Количество неприменимых устройств.|
|исправленоКоунт|Int32|Количество исправленных устройств.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код ответа и `201 Created` [объект deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "d3d3a75f-a75f-d3d3-5fa7-d3d35fa7d3d3",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```



