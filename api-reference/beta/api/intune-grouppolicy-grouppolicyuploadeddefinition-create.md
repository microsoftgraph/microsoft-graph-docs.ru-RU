---
title: Создание groupPolicyUploadedDefinition
description: Создайте новый объект groupPolicyUploadedDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8c44f462ebece0ebba6662c0f9ffc216c0e1d44
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788558"
---
# <a name="create-grouppolicyuploadeddefinition"></a>Создание groupPolicyUploadedDefinition

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Создайте новый [объект groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyDefinitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для объекта groupPolicyUploadedDefinition.

В следующей таблице показаны свойства, необходимые при создании groupPolicyUploadedDefinition.

|Свойство|Тип|Описание|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Определяет тип групп, к которые можно применить политику. Унаследовано от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md). Возможные значения: `user`, `machine`.|
|displayName|Строка|Имя локализованной политики. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|explainText|String|Локализованный текст объяснения или справки, связанные с политикой. По умолчанию это значение пусто. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|categoryPath|String|Путь к локализованным полным категориям для политики. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|supportedOn|String|Локализованная строка, используемая для указания того, на какую операционную систему или версию приложения влияет политика. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Унаследовано от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md). Возможные значения: `admxBacked`, `admxIngested`.|
|hasRelatedDefinitions|Boolean|Означает, есть ли связанные определения с этим определением, унаследованные от [groupPolicyDefinition.](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|groupPolicyCategoryId|Guid|ID категории родительской категории, унаследованной от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|minDeviceCspVersion|Строка|Минимальная требуемая версия CSP для конфигурации устройства в этом определении, унаследованной от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|minUserCspVersion|String|Минимальная требуемая версия CSP для конфигурации пользователя в этом определении, унаследованной от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|version|String|Настройка версии определения, унаследованной [от groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|id|String|Ключ объекта. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и `201 Created` [объект groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions
Content-type: application/json
Content-length: 538

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "minDeviceCspVersion": "Min Device Csp Version value",
  "minUserCspVersion": "Min User Csp Version value",
  "version": "Version value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "minDeviceCspVersion": "Min Device Csp Version value",
  "minUserCspVersion": "Min User Csp Version value",
  "version": "Version value",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



