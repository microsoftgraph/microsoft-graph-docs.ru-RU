---
title: Создание groupPolicyMigrationReport
description: Создайте новый объект GroupPolicyMigrationReport.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08901e26346c1bae90e080e2bc2313c7cd46ed8d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135581"
---
# <a name="create-grouppolicymigrationreport"></a>Создание groupPolicyMigrationReport

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект GroupPolicyMigrationReport.](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md)

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
POST /deviceManagement/groupPolicyMigrationReports
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта GroupPolicyMigrationReport.

В следующей таблице показаны свойства, необходимые при создании groupPolicyMigrationReport.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Пока не задокументировано.|
|groupPolicyObjectId|Guid|GUID объекта групповой политики из контента GPO Xml|
|displayName|Строка|Имя объекта групповой политики из контента GPO Xml|
|ouDistinguishedName|Строка|Отличительное имя OU.|
|createdDateTime|DateTimeOffset|Дата и время создания GroupPolicyMigrationReport.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения GroupPolicyMigrationReport.|
|groupPolicyCreatedDateTime|DateTimeOffset|Дата и время создания GroupPolicyMigrationReport.|
|groupPolicyLastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения GroupPolicyMigrationReport.|
|migrationReadiness|[groupPolicyMigrationReadiness](../resources/intune-gpanalyticsservice-grouppolicymigrationreadiness.md)|Покрытие Intune для связанного объекта групповой политики. Возможные значения: `none`, `partial`, `complete`, `error`, `notApplicable`.|
|targetedInActiveDirectory|Boolean|Свойство Targeted in AD из GPO Xml Content|
|totalSettingsCount|Int32|Общее число параметров групповой политики из GPO-файла.|
|supportedSettingsCount|Int32|Количество параметров групповой политики, поддерживаемых Intune.|
|supportedSettingsPercent|Int32|Процент параметров групповой политики, поддерживаемых Intune.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект groupPolicyMigrationReport](../resources/intune-gpanalyticsservice-grouppolicymigrationreport.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports
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
HTTP/1.1 201 Created
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




