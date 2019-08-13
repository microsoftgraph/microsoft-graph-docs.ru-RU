---
title: Создание Девицеманажементинтежерсеттингинстанце
description: Создание нового объекта Девицеманажементинтежерсеттингинстанце.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 645afa20e3e3e4bd5a0afe4be445c713868eef59
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343757"
---
# <a name="create-devicemanagementintegersettinginstance"></a>Создание Девицеманажементинтежерсеттингинстанце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .

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
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта Девицеманажементинтежерсеттингинстанце в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Девицеманажементинтежерсеттингинстанце.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|дефинитионид|String|Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|валуежсон|String|Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|Int32|Целое значение|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```






