---
title: Создание Граупполициуплоадеддефинитион
description: Создание нового объекта Граупполициуплоадеддефинитион.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c4f40f61d61050d3311f11bd8f8ded8381027a05
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42463873"
---
# <a name="create-grouppolicyuploadeddefinition"></a>Создание Граупполициуплоадеддефинитион

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создание нового объекта [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyDefinitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта Граупполициуплоадеддефинитион в формате JSON.

В следующей таблице приведены свойства, необходимые при создании Граупполициуплоадеддефинитион.

|Свойство|Тип|Описание|
|:---|:---|:---|
|класстипе|[граупполицидефинитионкласстипе](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Определяет тип групп, к которым можно применить политику. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md). Возможные значения: `user`, `machine`.|
|displayName|Строка|Имя локализованной политики. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|експлаинтекст|String|Локализованное объяснение или текст справки, связанный с политикой. По умолчанию это значение пусто. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|категорипас|String|Локализованный полный путь к категории для политики. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|суппортедон|String|Локализованная строка, используемая для указания версии операционной системы или приложения, на которые влияет политика. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|полицитипе|[граупполицитипе](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md). Возможные значения: `admxBacked`, `admxIngested`.|
|id|String|Ключ объекта. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Наследуется от [граупполицидефинитион](../resources/intune-grouppolicy-grouppolicydefinition.md)|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [граупполициуплоадеддефинитион](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
Content-type: application/json
Content-length: 293

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 406

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





