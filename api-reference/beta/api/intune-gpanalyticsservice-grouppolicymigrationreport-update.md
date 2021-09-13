---
title: Update groupPolicyMigrationReport
description: Обновление свойств объекта groupPolicyMigrationReport.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 44c63d97cd4d8606e8b03ef2dbba600d701f12ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59121706"
---
# <a name="update-grouppolicymigrationreport"></a>Update groupPolicyMigrationReport

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта [GroupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)

В следующей таблице показаны свойства, необходимые при создании [groupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|groupPolicyObjectId|Guid|GUID объекта групповой политики из контента GPO Xml|
|displayName|String|Имя объекта групповой политики из контента GPO Xml|
|ouDistinguishedName|String|Отличительное имя OU.|
|createdDateTime|DateTimeOffset|Дата и время создания GroupPolicyMigrationReport.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения GroupPolicyMigrationReport.|
|groupPolicyCreatedDateTime|DateTimeOffset|Дата и время создания GroupPolicyMigrationReport.|
|groupPolicyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения GroupPolicyMigrationReport.|
|migrationReadiness|[groupPolicyMigrationReadiness](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|Покрытие Intune для связанного объекта групповой политики. Возможные значения: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Логический|Свойство Targeted in AD из GPO Xml Content|
|totalSettingsCount|Int32|Общее число групповых политик Параметры из GPO-файла.|
|supportedSettingsCount|Int32|Количество групповых политик Параметры поддерживается Intune.|
|supportedSettingsPercent|Int32|Процент групповой политики Параметры поддерживается Intune.|



## <a name="response"></a>Отклик
В случае успеха этот метод возвращает код отклика и обновленный объект `200 OK` [groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}
Content-type: application/json
Content-length: 544

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "@odata.type": "#microsoft.graph.groupPolicyMigrationReport",
  "id": "60663fa8-3fa8-6066-a83f-6660a83f6660",
  "groupPolicyObjectId": "ca1c97af-97af-ca1c-af97-1ccaaf971cca",
  "displayName": "Display Name value",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "groupPolicyCreatedDateTime": "2016-12-31T23:58:14.0676812-08:00",
  "groupPolicyLastModifiedDateTime": "2017-01-01T00:02:51.2241017-08:00",
  "migrationReadiness": "partial",
  "targetedInActiveDirectory": true,
  "totalSettingsCount": 2,
  "supportedSettingsCount": 6,
  "supportedSettingsPercent": 8
}
```



