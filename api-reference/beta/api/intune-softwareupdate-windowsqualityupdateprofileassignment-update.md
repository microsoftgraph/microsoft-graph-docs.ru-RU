---
title: Обновление windowsQualityUpdateProfileAssignment
description: Обновление свойств объекта windowsQualityUpdateProfileAssignment.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eae3b285e4b628a7705fa6361df02ab021271d0c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345746"
---
# <a name="update-windowsqualityupdateprofileassignment"></a>Обновление windowsQualityUpdateProfileAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments/{windowsQualityUpdateProfileAssignmentId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта WindowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)

В следующей таблице показаны свойства, необходимые при создании [windowsQualityUpdateProfileAssignment.](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор сущности|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения, на которую назначен профиль обновления качества.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и обновленный `200 OK` [объект windowsQualityUpdateProfileAssignment](../resources/intune-softwareupdate-windowsqualityupdateprofileassignment.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}/assignments/{windowsQualityUpdateProfileAssignmentId}
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfileAssignment",
  "id": "0c3a8422-8422-0c3a-2284-3a0c22843a0c",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  }
}
```




