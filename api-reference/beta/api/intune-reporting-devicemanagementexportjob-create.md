---
title: Создание deviceManagementExportJob
description: Создание нового объекта deviceManagementExportJob.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b650e7c5023d0a581986b13a175e95f516baf78e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59138647"
---
# <a name="create-devicemanagementexportjob"></a>Создание deviceManagementExportJob

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового [объекта deviceManagementExportJob.](../resources/intune-reporting-devicemanagementexportjob.md)

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
POST /deviceManagement/reports/exportJobs
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта deviceManagementExportJob.

В следующей таблице показаны свойства, необходимые при создании устройстваManagementExportJob.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для этого объекта|
|reportName|String|Имя отчета|
|filter|String|Фильтры, применяемые в отчете|
|select|Коллекция объектов string|Столбцы, выбранные из отчета|
|format|[deviceManagementReportFileFormat](../resources/intune-reporting-devicemanagementreportfileformat.md)|Формат экспортируемого отчета. Возможные значения: `csv`, `pdf`.|
|snapshotId|String|Снимок — это идентифицируемый подмножество наборов данных, представленных в ReportName. Здесь можно использовать id sessionId или CachedReportConfiguration. Если задана sessionId, фильтр, выберите и OrderBy применяются к данным, представленным sessionId. Фильтр, выбор и OrderBy нельзя указать вместе с id CachedReportConfiguration.|
|ЛокализацияТип|[deviceManagementExportJobLocalizationType](../resources/intune-reporting-devicemanagementexportjoblocalizationtype.md)|Настройка локализации запрашиваемого задания экспорта. Возможные значения: `localizedValuesAsAdditionalColumn`, `replaceLocalizableValues`.|
|status|[deviceManagementReportStatus](../resources/intune-reporting-devicemanagementreportstatus.md)|Состояние задания экспорта. Возможные значения: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String|Временное расположение экспортируемого отчета|
|requestDateTime|DateTimeOffset|Время запроса экспортируемой отчетности|
|expirationDateTime|DateTimeOffset|Время истечения срока действия экспортируемой отчетности|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика и `201 Created` [объект deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
Content-type: application/json
Content-length: 455

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 504

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "9ddfb995-b995-9ddf-95b9-df9d95b9df9d",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "pdf",
  "snapshotId": "Snapshot Id value",
  "localizationType": "replaceLocalizableValues",
  "status": "notStarted",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:03:07.1589002-08:00",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
}
```



