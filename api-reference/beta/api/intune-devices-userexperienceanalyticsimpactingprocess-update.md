---
title: Обновление userExperienceAnalyticsImpactingProcess
description: Обновление свойств объекта userExperienceAnalyticsImpactingProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f2d1f2c3a2791e6536e701be35bc0c5c91e62949
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146225"
---
# <a name="update-userexperienceanalyticsimpactingprocess"></a>Обновление userExperienceAnalyticsImpactingProcess

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)

В следующей таблице показаны свойства, необходимые при создании [userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор объекта аналитики пользовательского интерфейса, который оказывает влияние на процесс.|
|deviceId|String|Уникальный идентификатор влияемого устройства.|
|category|String|Категория воздействия процесса.|
|processName|Строка|Имя процесса.|
|description|Строка|Описание процесса.|
|publisher|String|Издатель процесса.|
|impactValue|Двойное с плавающей точкой|Значение влияния процесса. Допустимые значения от 0 до 1.79769313486232E+308|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код ответа и обновленный `200 OK` [объект userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "id": "faefd665-d665-faef-65d6-effa65d6effa",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```




