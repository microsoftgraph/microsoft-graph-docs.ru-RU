---
title: Создание ГраупполиципресентатионлонгдеЦималтекстбокс
description: Создание нового объекта ГраупполиципресентатионлонгдеЦималтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0f96507c8d354acda092e910b5f496f979a4c265
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730947"
---
# <a name="create-grouppolicypresentationlongdecimaltextbox"></a>Создание ГраупполиципресентатионлонгдеЦималтекстбокс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) .

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
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
В тексте запроса добавьте представление объекта ГраупполиципресентатионлонгдеЦималтекстбокс в формате JSON.

В следующей таблице приведены свойства, необходимые при создании ГраупполиципресентатионлонгдеЦималтекстбокс.

|Свойство|Тип|Описание|
|:---|:---|:---|
|label|Строка|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Строка|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|Int64|Целое число без знака, задающее начальное значение для десятичного текстового поля. Значение по умолчанию равно 1.|
|повернуть|Логический|Если значение — true, создайте элемент управления "Счетчик"; в противном случае создайте текстовое поле для числового элемента. Значение по умолчанию: true.|
|спинстеп|Int64|Целое число без знака, которое указывает приращение изменения элемента управления "Счетчик". Значение по умолчанию равно 1.|
|Обязательный|Логический|Требование ввести значение в поле параметр. Значение по умолчанию  false.|
|minValue|Int64|Длинное целое число без знака, задающее минимальное допустимое значение. Значение по умолчанию равно 0.|
|maxValue|Int64|Длинное целое число без знака, задающее максимальное допустимое значение. Значение по умолчанию — 9999.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатионлонгдеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 338

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "Label value",
  "id": "754d8495-8495-754d-9584-4d7595844d75",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```





