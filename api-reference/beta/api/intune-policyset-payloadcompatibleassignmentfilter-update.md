---
title: Обновление полезной нагрузкиCompatibleAssignmentFilter
description: Обновление свойств объекта payloadCompatibleAssignmentFilter.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6bb6288669a48d8ad52a0dbe4ad45073e3565e95
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135559"
---
# <a name="update-payloadcompatibleassignmentfilter"></a>Обновление полезной нагрузкиCompatibleAssignmentFilter

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта [payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)

В следующей таблице показаны свойства, необходимые при создании полезной [нагрузкиCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|createdDateTime|DateTimeOffset|Время создания фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|displayName|String|DisplayName фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|description|String|Описание фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|платформа|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Тип платформы устройств, на которых будет применяться фильтр назначения. Наследуется [от deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md). Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|правило|String|Определение правила фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|roleScopeTags|Коллекция объектов string|RoleScopeTags фильтра назначения. Унаследованный от [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|payloadType|[assignmentFilterPayloadType](../resources/intune-policyset-assignmentfilterpayloadtype.md)|PayloadType фильтра назначения. Возможные значения: `notSet`, `enrollmentRestrictions`.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и обновленный объект `200 OK` [payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/assignmentFilters/{deviceAndAppManagementAssignmentFilterId}
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.payloadCompatibleAssignmentFilter",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ],
  "payloadType": "enrollmentRestrictions"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.payloadCompatibleAssignmentFilter",
  "id": "6d189738-9738-6d18-3897-186d3897186d",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "platform": "androidForWork",
  "rule": "Rule value",
  "roleScopeTags": [
    "Role Scope Tags value"
  ],
  "payloadType": "enrollmentRestrictions"
}
```



