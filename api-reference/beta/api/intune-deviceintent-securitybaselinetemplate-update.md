---
title: Обновление Секуритибаселинетемплате
description: Обновление свойств объекта Секуритибаселинетемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1d0ceaf67d8f951b792f31c625204b1544d8d9ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42470114"
---
# <a name="update-securitybaselinetemplate"></a>Обновление Секуритибаселинетемплате

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) .

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
PATCH /deviceManagement/templates/{deviceManagementTemplateId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/migratableTo/{deviceManagementTemplateId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор шаблона, унаследованный от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|displayName|Строка|Отображаемое имя шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|description|String|Описание шаблона, унаследованное от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|versionInfo|String|Сведения о версии шаблона, унаследованные от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|нерекомендуемый|Логический|Шаблон устарел или не является устаревшим. Не удается создать объект "удержания" из устаревшего шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|интенткаунт|Int32|Количество целей, созданных на основе этого шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|
|TemplateType — тип|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|Тип шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.|
|platformType|[полициплатформтипе](../resources/intune-shared-policyplatformtype.md)|Платформа шаблона. Наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md). Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|publishedDateTime|DateTimeOffset|При публикации шаблона наследуется от [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md)|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [секуритибаселинетемплате](../resources/intune-deviceintent-securitybaselinetemplate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "platformType": "androidForWork",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 420

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
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```





