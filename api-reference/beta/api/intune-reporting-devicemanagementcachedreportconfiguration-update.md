---
title: Обновление deviceManagementCachedReportConfiguration
description: Обновление свойств объекта deviceManagementCachedReportConfiguration.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e91a43b87bd35930caf92f383f1e406976d82623
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59138654"
---
# <a name="update-devicemanagementcachedreportconfiguration"></a>Обновление deviceManagementCachedReportConfiguration

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта deviceManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)

В следующей таблице показаны свойства, необходимые при создании [устройстваManagementCachedReportConfiguration.](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта|
|reportName|String|Имя отчета|
|filter|String|Фильтры, применяемые при создании отчета.|
|select|Коллекция объектов string|Столбцы, выбранные из отчета|
|orderBy|Коллекция объектов string|Порядок столбцов в отчете|
|метаданные|String|Метаданные, управляемые вызывателями, связанные с отчетом|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Состояние кэшного отчета. Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|lastRefreshDateTime|DateTimeOffset|Время последнего обновления кэшного отчета|
|expirationDateTime|DateTimeOffset|Время истечения срока действия кэш-отчета|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и обновленный объект `200 OK` [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
Content-type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "46947722-7722-4694-2277-944622779446",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "metadata": "Metadata value",
  "status": "notStarted",
  "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```



