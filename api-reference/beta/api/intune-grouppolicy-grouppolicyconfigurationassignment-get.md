---
title: Get groupPolicyConfigurationAssignment
description: Чтение свойств и связей объекта groupPolicyConfigurationAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 27dde826c6215f644907b5739d50c6d531f8f411
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161168"
---
# <a name="get-grouppolicyconfigurationassignment"></a>Get groupPolicyConfigurationAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Чтение свойств и связей объекта [groupPolicyConfigurationAssignment.](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)

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
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и объект `200 OK` [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) в теле отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/assignments/{groupPolicyConfigurationAssignmentId}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
    "id": "2a4161e9-61e9-2a41-e961-412ae961412a",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "target": {
      "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include",
      "collectionId": "Collection Id value"
    }
  }
}
```




