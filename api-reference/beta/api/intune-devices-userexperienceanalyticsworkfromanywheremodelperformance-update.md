---
title: Обновление userExperienceAnalyticsWorkFromAnywhereModelPerformance
description: Обновление свойств объекта userExperienceAnalyticsWorkFromAnywhereModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d870340ff08e36f2b6f60bc2f945ded6300b400
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62292374"
---
# <a name="update-userexperienceanalyticsworkfromanywheremodelperformance"></a>Обновление userExperienceAnalyticsWorkFromAnywhereModelPerformance

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereModelPerformance/{userExperienceAnalyticsWorkFromAnywhereModelPerformanceId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) .

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта производительности модели аналитики пользовательских интерфейсов.|
|model|String|Пользовательский интерфейс работает с любого типового имени устройств.|
|manufacturer|String|Пользовательский интерфейс работает с любого имени производителя устройств.|
|modelDeviceCount|Int32|Пользовательский опыт работы с устройств в любом месте считается для модели. Допустимые значения 2147483648 2147483647|
|workFromAnywhereScore|Double|Пользовательский опыт работы с любой общей оценкой для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|WindowsScore|Double|Пользовательский опыт работы из любого окна оценка для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudManagementScore|Double|Пользовательский опыт работы с любой оценкой облачного управления для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudIdentityScore|Double|Пользовательский опыт работы с облачной оценкой удостоверений в любом месте для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|cloudProvisioningScore|Double|Пользовательский опыт работы с облачной оценкой для модели. Допустимые значения -1.79769313486232E+308 до 1.797693133486232E+308|
|healthStatus|[userExperienceAnalyticsHealthState](../resources/intune-devices-userexperienceanalyticshealthstate.md)|Состояние состояния аналитики пользовательских интерфейсов работает из любой модели. Возможные значения: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## <a name="response"></a>Отклик
В случае `200 OK` успеха этот метод возвращает код отклика и обновленный объект [userExperienceAnalyticsWorkFromAnywhereModelPerformance](../resources/intune-devices-userexperienceanalyticsworkfromanywheremodelperformance.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereModelPerformance/{userExperienceAnalyticsWorkFromAnywhereModelPerformanceId}
Content-type: application/json
Content-length: 411

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereModelPerformance",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
  "workFromAnywhereScore": 7.0,
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereModelPerformance",
  "id": "7ec79407-9407-7ec7-0794-c77e0794c77e",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "modelDeviceCount": 0,
  "workFromAnywhereScore": 7.0,
  "windowsScore": 4.0,
  "cloudManagementScore": 6.666666666666667,
  "cloudIdentityScore": 6.0,
  "cloudProvisioningScore": 7.333333333333333,
  "healthStatus": "insufficientData"
}
```




