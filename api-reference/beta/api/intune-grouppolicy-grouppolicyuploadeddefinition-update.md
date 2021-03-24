---
title: Update groupPolicyUploadedDefinition
description: Обновление свойств объекта groupPolicyUploadedDefinition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f643d8f957590f2a619174ccc50545bdd5b53520
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135280"
---
# <a name="update-grouppolicyuploadeddefinition"></a>Update groupPolicyUploadedDefinition

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/category/definitions/{groupPolicyDefinitionId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile/definitions/{groupPolicyDefinitionId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)

В следующей таблице показаны свойства, необходимые при создании [groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Определяет тип групп, к которые можно применить политику. Унаследовано от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md). Возможные значения: `user`, `machine`.|
|displayName|Строка|Имя локализованной политики. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|explainText|Строка|Локализованный текст объяснения или справки, связанные с политикой. По умолчанию это значение пусто. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|categoryPath|Строка|Путь к локализованным полным категориям для политики. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|supportedOn|Строка|Локализованная строка, используемая для указания того, на какую операционную систему или версию приложения влияет политика. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Указывает тип групповой политики. Унаследовано от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md). Возможные значения: `admxBacked`, `admxIngested`.|
|groupPolicyCategoryId|Guid|ID категории родительской категории, унаследованной от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|id|Строка|Ключ объекта. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта. Унаследованный от [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный `200 OK` [объект groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitions/{groupPolicyDefinitionId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 474

{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "machine",
  "displayName": "Display Name value",
  "explainText": "Explain Text value",
  "categoryPath": "Category Path value",
  "supportedOn": "Supported On value",
  "policyType": "admxIngested",
  "groupPolicyCategoryId": "4d1e97a2-97a2-4d1e-a297-1e4da2971e4d",
  "id": "a5f83119-3119-a5f8-1931-f8a51931f8a5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




