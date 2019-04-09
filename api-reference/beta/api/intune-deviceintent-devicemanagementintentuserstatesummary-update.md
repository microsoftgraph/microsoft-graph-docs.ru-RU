---
title: Обновление Девицеманажементинтентусерстатесуммари
description: Обновление свойств объекта Девицеманажементинтентусерстатесуммари.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a4ed99765d325930cae186a9c7b6548e0a477a8
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522834"
---
# <a name="update-devicemanagementintentuserstatesummary"></a>Обновление Девицеманажементинтентусерстатесуммари

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
```

## <a name="request-headers"></a>Заголовки запросов
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [Девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор|
|conflictCount|Int32|Количество пользователей в конфликте|
|errorCount|Int32|Количество пользователей с ошибками|
|failedCount|Int32|Количество пользователей с ошибками|
|notApplicableCount|Int32|Количество неприменимых пользователей|
|successCount|Int32|Количество успешных пользователей|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицеманажементинтентусерстатесуммари](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStateSummary
Content-type: application/json
Content-length: 198

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```

### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "be567e02-7e02-be56-027e-56be027e56be",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "successCount": 12
}
```







