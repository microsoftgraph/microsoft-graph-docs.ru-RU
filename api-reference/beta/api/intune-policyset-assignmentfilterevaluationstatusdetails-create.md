---
title: Создание assignmentFilterEvaluationStatusDetails
description: Создание нового объекта assignmentFilterEvaluationStatusDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: aa4418ea4e00099e807684196d8960231d3b9c28
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158733"
---
# <a name="create-assignmentfilterevaluationstatusdetails"></a>Создание assignmentFilterEvaluationStatusDetails

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта assignmentFilterEvaluationStatusDetails.](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса подарим представление JSON для объекта assignmentFilterEvaluationStatusDetails.

В следующей таблице показаны свойства, необходимые при создании назначенияFilterEvaluationStatusDetails.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта AssignmentFilterEvaluationStatusDetails.|
|payloadId|Строка|PayloadId, на котором применен фильтр.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код ответа и объект `201 Created` [assignmentFilterEvaluationStatusDetails](../resources/intune-policyset-assignmentfilterevaluationstatusdetails.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/assignmentFilterEvaluationStatusDetails
Content-type: application/json
Content-length: 117

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "payloadId": "Payload Id value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 166

{
  "@odata.type": "#microsoft.graph.assignmentFilterEvaluationStatusDetails",
  "id": "820ef068-f068-820e-68f0-0e8268f00e82",
  "payloadId": "Payload Id value"
}
```




