---
title: Создание ГраупполиципресентатиондеЦималтекстбокс
description: Создание нового объекта ГраупполиципресентатиондеЦималтекстбокс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 22bc04b8c6b66110d1de858b698fc2924b917ef5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424591"
---
# <a name="create-grouppolicypresentationdecimaltextbox"></a>Создание ГраупполиципресентатиондеЦималтекстбокс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) .

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
В тексте запроса добавьте представление объекта ГраупполиципресентатиондеЦималтекстбокс в формате JSON.

В следующей таблице приведены свойства, необходимые при создании ГраупполиципресентатиондеЦималтекстбокс.

|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|Int64|Целое число без знака, задающее начальное значение для десятичного текстового поля. Значение по умолчанию равно 1.|
|повернуть|Boolean|Если значение — true, создайте элемент управления "Счетчик"; в противном случае создайте текстовое поле для числового элемента. Значение по умолчанию: true.|
|спинстеп|Int64|Целое число без знака, которое указывает приращение изменения элемента управления "Счетчик". Значение по умолчанию равно 1.|
|Обязательный|Boolean|Требование ввести значение в поле параметр. Значение по умолчанию  false.|
|minValue|Int64|Целое число без знака, задающее минимальное допустимое значение. Значение по умолчанию равно 0.|
|maxValue|Int64|Целое число без знака, задающее максимальное допустимое значение. Значение по умолчанию — 9999.|



## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполиципресентатиондеЦималтекстбокс](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 221

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
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
Content-Length: 334

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "Label value",
  "id": "988daea7-aea7-988d-a7ae-8d98a7ae8d98",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": 12,
  "spin": true,
  "spinStep": 8,
  "required": true,
  "minValue": 8,
  "maxValue": 8
}
```



