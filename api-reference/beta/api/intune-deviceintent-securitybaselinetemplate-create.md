---
title: Создание Секуритибаселинетемплате
description: Создание нового объекта Секуритибаселинетемплате.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dce4f2b8f46148b8ebaf11185eb02f78eaa0aa10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088197"
---
# <a name="create-securitybaselinetemplate"></a>Создание Секуритибаселинетемплате

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
POST /deviceManagement/templates
POST /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Секуритибаселинетемплате в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Секуритибаселинетемплате.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|Строка|Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|Строка|Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|Строка|Сведения о версии шаблона, унаследованные от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|нерекомендуемый|Boolean|Шаблон устарел или не является устаревшим. Не удается создать объект "удержания" из устаревшего шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|интенткаунт|Int32|Количество целей, созданных на основе этого шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|TemplateType — тип|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|Тип шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`, `deviceConfigurationForOffice365`, `cloudPC`.|
|platformType|[полициплатформтипе](../resources/intune-shared-policyplatformtype.md)|Платформа шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|темплатесубтипе|[deviceManagementTemplateSubtype](../resources/intune-deviceintent-devicemanagementtemplatesubtype.md)|Подтип шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `none`, `firewall`, `diskEncryption`, `attackSurfaceReduction`, `endpointDetectionReponse`, `accountProtection`, `antivirus`.|
|publishedDateTime|DateTimeOffset|При публикации шаблона наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "id": "3f61d4c2-d4c2-3f61-c2d4-613fc2d4613f",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "templateSubtype": "firewall",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```






