---
title: Тип ресурса reportRoot
description: Представляет контейнер для ресурсов отчетов Azure Active Directory (Azure AD).
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 51816aef9b5b21732111206785057233c5144bc5
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2022
ms.locfileid: "66855947"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет контейнер для ресурсов отчетов Azure Active Directory (Azure AD).

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [Перечисление applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md) | [Коллекция applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Получение **объектов applicationSignInDetailedSummary** . |
| [Получение applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Чтение свойств и связей объекта **applicationSignInDetailedSummary** . |
| [getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md) | [applicationSignInSummary](applicationsigninsummary.md) | Чтение свойств и связей объекта **applicationSignInSummary** . |
|[Перечисление credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md)|[Коллекция credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Получение сведений об объектах credentialUserRegistrationDetails для заданного клиента.|
|[Перечисление userCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md)|[Коллекция userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Получение объектов userCredentialUsageDetails для заданного клиента. Сведения включают сведения о пользователе, состояние сброса и причину сбоя.|
<!--Temporarily hide these functions until we document them and others.
|[getAzureADLicenseUsage](../api/reportroot-getazureadlicenseusage.md)|[azureADLicenseUsage](../resources/azureadlicenseusage.md) collection|**TODO: Add Description**|
|[getAzureADUserFeatureUsage](../api/reportroot-getazureaduserfeatureusage.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADFeatureUsage](../api/reportroot-getazureadfeatureusage.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md) collection|**TODO: Add Description**|
|[getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection|**TODO: Add Description**|
|[getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md)|[credentialUsageSummary](../resources/credentialusagesummary.md) collection|**TODO: Add -->

## <a name="properties"></a>Свойства
Нет

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|applicationSignInDetailedSummary|[Коллекция applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Представляет подробную сводку по входу в приложение.|
|authenticationMethods|[authenticationMethodsRoot](../resources/authenticationmethodsroot.md)|Контейнер для свойств навигации для Azure AD методов проверки подлинности.|
|credentialUserRegistrationDetails|[Коллекция credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Сведения об использовании самостоятельного сброса пароля и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.|
|userCredentialUsageDetails|[Коллекция userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Представляет использование самостоятельного сброса пароля (SSPR) для данного клиента.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot"
}
```
