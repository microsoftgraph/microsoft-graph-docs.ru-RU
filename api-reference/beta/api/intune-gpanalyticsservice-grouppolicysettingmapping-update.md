---
title: Update groupPolicySettingMapping
description: Обновление свойств объекта groupPolicySettingMapping.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f73f00d1d323a3bc48824aaada4591f6f2cb01d6790c3e0fa850eaf7b8fab35a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54157019"
---
# <a name="update-grouppolicysettingmapping"></a>Update groupPolicySettingMapping

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)

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
PATCH /deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)

В следующей таблице показаны свойства, необходимые при создании [groupPolicySettingMapping.](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Пока не задокументировано.|
|parentId|Строка|Родительский Id параметра групповой политики.|
|childIdList|Коллекция String|Список детских ид параметра групповой политики.|
|settingName|String|Имя этого параметра групповой политики.|
|settingValue|Строка|Значение этого параметра групповой политики.|
|settingValueType|Строка|Тип значения этого параметра групповой политики.|
|settingDisplayName|Строка|Отображение имени этого параметра групповой политики.|
|settingDisplayValue|Строка|Отображение значения этого параметра групповой политики.|
|settingDisplayValueType|Строка|Тип отображения значения этого параметра групповой политики.|
|settingValueDisplayUnits|String|Отображаемая единица этого значения групповой политики|
|settingCategory|Строка|Категория, в которая находится параметр групповой политики.|
|mdmCspName|Строка|CSP назовет эту групповую политику, устанавливая карты.|
|mdmSettingUri|Строка|MDM CSP URI этой групповой политики, устанавливая карты.|
|mdmMinimumOSVersion|Int32|Минимальная версия ОС, поддерживаемая этим параметром mdm.|
|settingType|[groupPolicySettingType](../resources/intune-gpanalyticsservice-grouppolicysettingtype.md)|Тип параметра (безопасность или admx) групповой политики. Возможные значения: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|isMdmSupported|Логический|Указывает, поддерживает ли параметр Intune или нет.|
|mdmSupportedState|[mdmSupportedState](../resources/intune-gpanalyticsservice-mdmsupportedstate.md)|Указывает, поддерживается ли параметр в Mdm или нет. Возможные значения: `unknown`, `supported`, `unsupported`, `deprecated`.|
|settingScope|[groupPolicySettingScope](../resources/intune-gpanalyticsservice-grouppolicysettingscope.md)|Область настройки. Возможные значения: `unknown`, `device`, `user`.|
|intuneSettingUriList|Коллекция String|Список URL-адресов intune Setting this group policy setting maps to|
|intuneSettingDefinitionId|Строка|Id определения параметра Intune|
|admxSettingDefinitionId|String|Admx Group Policy Id|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект groupPolicySettingMapping](../resources/intune-gpanalyticsservice-grouppolicysettingmapping.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyMigrationReports/{groupPolicyMigrationReportId}/groupPolicySettingMappings/{groupPolicySettingMappingId}
Content-type: application/json
Content-length: 1023

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1072

{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "8fa04560-4560-8fa0-6045-a08f6045a08f",
  "parentId": "Parent Id value",
  "childIdList": [
    "Child Id List value"
  ],
  "settingName": "Setting Name value",
  "settingValue": "Setting Value value",
  "settingValueType": "Setting Value Type value",
  "settingDisplayName": "Setting Display Name value",
  "settingDisplayValue": "Setting Display Value value",
  "settingDisplayValueType": "Setting Display Value Type value",
  "settingValueDisplayUnits": "Setting Value Display Units value",
  "settingCategory": "Setting Category value",
  "mdmCspName": "Mdm Csp Name value",
  "mdmSettingUri": "Mdm Setting Uri value",
  "mdmMinimumOSVersion": 3,
  "settingType": "policy",
  "isMdmSupported": true,
  "mdmSupportedState": "supported",
  "settingScope": "device",
  "intuneSettingUriList": [
    "Intune Setting Uri List value"
  ],
  "intuneSettingDefinitionId": "Intune Setting Definition Id value",
  "admxSettingDefinitionId": "Admx Setting Definition Id value"
}
```




