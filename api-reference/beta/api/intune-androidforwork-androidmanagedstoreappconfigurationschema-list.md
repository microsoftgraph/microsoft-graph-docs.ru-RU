---
title: Список Андроидманажедстореаппконфигуратионсчемас
description: Список свойств и связей объектов Андроидманажедстореаппконфигуратионсчема.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 141c14087405b8c3c009a7fc3d245f2b7db8ca1b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/10/2019
ms.locfileid: "39922715"
---
# <a name="list-androidmanagedstoreappconfigurationschemas"></a>Список Андроидманажедстореаппконфигуратионсчемас

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [андроидманажедстореаппконфигуратионсчема](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1871

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
      "id": "db86c34a-c34a-db86-4ac3-86db4ac386db",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
          "index": 5,
          "parentIndex": 11,
          "schemaItemKey": "Schema Item Key value",
          "displayName": "Display Name value",
          "description": "Description value",
          "defaultBoolValue": true,
          "defaultIntValue": 15,
          "defaultStringValue": "Default String Value value",
          "defaultStringArrayValue": [
            "Default String Array Value value"
          ],
          "dataType": "integer",
          "selections": [
            {
              "@odata.type": "microsoft.graph.keyValuePair",
              "name": "Name value",
              "value": "Value value"
            }
          ]
        }
      ],
      "nestedSchemaItems": [
        {
          "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
          "index": 5,
          "parentIndex": 11,
          "schemaItemKey": "Schema Item Key value",
          "displayName": "Display Name value",
          "description": "Description value",
          "defaultBoolValue": true,
          "defaultIntValue": 15,
          "defaultStringValue": "Default String Value value",
          "defaultStringArrayValue": [
            "Default String Array Value value"
          ],
          "dataType": "integer",
          "selections": [
            {
              "@odata.type": "microsoft.graph.keyValuePair",
              "name": "Name value",
              "value": "Value value"
            }
          ]
        }
      ]
    }
  ]
}
```





