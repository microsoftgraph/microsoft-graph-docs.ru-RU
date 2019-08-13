---
title: Создание Девицеманажементтемплате
description: Создание нового объекта Девицеманажементтемплате.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8df263e974037e747eb65169f6d305cef2b7b3b5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343134"
---
# <a name="create-devicemanagementtemplate"></a>Создание Девицеманажементтемплате

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) .

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

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Девицеманажементтемплате в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Девицеманажементтемплате.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор шаблона|
|displayName|Строка|Отображаемое имя шаблона|
|description|String|Описание шаблона|
|versionInfo|String|Сведения о версии шаблона|
|нерекомендуемый|Boolean|Шаблон устарел или не является устаревшим. Не удается создать объект "удержания" из устаревшего шаблона.|
|интенткаунт|Int32|Количество целей, созданных на основе этого шаблона.|
|TemplateType — тип|[девицеманажементтемплатетипе](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|Тип шаблона. Возможные значения: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`.|
|publishedDateTime|DateTimeOffset|При публикации шаблона|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементтемплате](../resources/intune-deviceintent-devicemanagementtemplate.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates
Content-type: application/json
Content-length: 334

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 383

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "edd764ca-64ca-edd7-ca64-d7edca64d7ed",
  "displayName": "Display Name value",
  "description": "Description value",
  "versionInfo": "Version Info value",
  "isDeprecated": true,
  "intentCount": 11,
  "templateType": "specializedDevices",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00"
}
```






