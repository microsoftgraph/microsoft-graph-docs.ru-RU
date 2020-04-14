---
title: Обновление Граупполиципресентатионкомбобокс
description: Обновление свойств объекта Граупполиципресентатионкомбобокс.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c68718732d7a332c857f36a4b2963603dd613c49
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43424678"
---
# <a name="update-grouppolicypresentationcombobox"></a>Обновление Граупполиципресентатионкомбобокс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) .

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
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations/{groupPolicyPresentationId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|label|String|Локализованная текстовая подпись для любой сущности презентации. По умолчанию это значение пусто. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Ключ объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполиципресентатион](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|Значение|String|Локализованная строка по умолчанию, отображаемая в поле со списком. По умолчанию это значение пусто.|
|мнение|Коллекция String|Локализованные строки, перечисленные в раскрывающемся списке поля со списком. По умолчанию это значение пусто.|
|Обязательный|Логическое|Указывает, следует ли указать значение для параметра. Значение по умолчанию  false.|
|maxLength|Int64|Целое число без знака, задающее максимальное количество текстовых символов для параметра. Значение по умолчанию — 1023.|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [граупполиципресентатионкомбобокс](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation
Content-type: application/json
Content-length: 233

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "Label value",
  "id": "44332a1d-2a1d-4433-1d2a-33441d2a3344",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "defaultValue": "Default Value value",
  "suggestions": [
    "Suggestions value"
  ],
  "required": true,
  "maxLength": 9
}
```



