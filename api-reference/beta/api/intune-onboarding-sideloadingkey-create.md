---
title: Создание sideLoadingKey
description: Создайте объект sideLoadingKey.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a55840adf84a5234a7ded834ca03ceb4a9c69498
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212908"
---
# <a name="create-sideloadingkey"></a>Создание sideLoadingKey

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте объект [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта sideLoadingKey в формате JSON.

В следующей таблице показаны свойства, необходимые при создании sideLoadingKey.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор ключа загрузки неопубликоваемого ключа.|
|value|String|Значение ключа загрузки стороны— это значение 5x5, разделяемое по hiphens.|
|displayName|String|Имя ключа загрузки стороны, отображаемое для администраторов ITPro.|
|description|Строка|Описание ключа загрузки неопубликоваемых приложений, отображаемое для администраторов ITPro.|
|totalActivation|Int32|Активация всего ключа загрузки неопубликоваемых ключей, отображаемая для ИТ-администраторов.|
|lastUpdatedDateTime|Строка|Дата последнего обновления ключа загрузки стороны, отображаемая для администраторов ITPro.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает код `201 Created` отклика и объект [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```




