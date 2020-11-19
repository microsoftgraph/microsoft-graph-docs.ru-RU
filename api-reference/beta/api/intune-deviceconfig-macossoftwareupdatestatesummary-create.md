---
title: Создание Макоссофтвареупдатестатесуммари
description: Создание нового объекта Макоссофтвареупдатестатесуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a94fae032fd3bae053b7af170d5ac1c4f43b2a08
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49219938"
---
# <a name="create-macossoftwareupdatestatesummary"></a>Создание Макоссофтвареупдатестатесуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
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
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Макоссофтвареупдатестатесуммари в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Макоссофтвареупдатестатесуммари.

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Понятное имя обновления программного обеспечения|
|productKey|String|Ключ продукта обновления программного обеспечения.|
|упдатекатегори|[macOSSoftwareUpdateCategory](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|Категория обновлений программного обеспечения. Возможные значения: `critical`, `configurationDataFile`, `firmware`, `other`.|
|упдатеверсион|String|Версия обновления программного обеспечения|
|state|[macOSSoftwareUpdateState](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|Состояние обновления программного обеспечения. Возможные значения: `success` , `downloading` ,,,,, `downloaded` `installing` `idle` `available` `scheduled` ,,, `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` , `downloadInsufficientNetwork` , `installInsufficientSpace` , `installInsufficientPower` , `installFailed` , `commandFailed` .|
|lastUpdatedDateTime|DateTimeOffset|Дата и время последнего обновления отчета для этого устройства и ключа продукта.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макоссофтвареупдатестатесуммари](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "9527a1df-a1df-9527-dfa1-2795dfa12795",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




