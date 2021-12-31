---
title: Тип ресурса reportRoot
description: Контейнер для ресурсов отчетов Azure AD.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0cd17a6f8a06b9c5a4b263b06c3bb3ec71d7dc0c
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647076"
---
# <a name="reportroot-resource-type"></a>Тип ресурса reportRoot

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Контейнер, который предоставляет свойства навигации для ресурсов отчетов Azure AD.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
| [List applicationSignInDetailedSummary](../api/reportroot-list-applicationsignindetailedsummary.md) | [коллекция applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Получение **объектов applicationSignInDetailedSummary.** |
| [Получение applicationSignInDetailedSummary](../api/applicationsignindetailedsummary-get.md) | [applicationSignInDetailedSummary](applicationsignindetailedsummary.md) | Ознакомьтесь с свойствами и отношениями **объекта applicationSignInDetailedSummary.** |
| [getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md) | [applicationSignInSummary](applicationsigninsummary.md) | Ознакомьтесь с свойствами и отношениями **объекта applicationSignInSummary.** |
|[Список credentialUserRegistrationDetails](../api/reportroot-list-credentialuserregistrationdetails.md)|[коллекция credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Сведения о объектах credentialUserRegistrationDetails для данного клиента.|
|[Список пользователейCredentialUsageDetails](../api/reportroot-list-usercredentialusagedetails.md)|[коллекция userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Получите объекты userCredentialUsageDetails для данного клиента. Сведения включают сведения о пользователях, состояние сброса и причину сбоя.|
<!--Temporarily hide these functions until we document them and others.
|[getAzureADLicenseUsage](../api/reportroot-getazureadlicenseusage.md)|[azureADLicenseUsage](../resources/azureadlicenseusage.md) collection|**TODO: Add Description**|
|[getAzureADUserFeatureUsage](../api/reportroot-getazureaduserfeatureusage.md)|[azureADUserFeatureUsage](../resources/azureaduserfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADFeatureUsage](../api/reportroot-getazureadfeatureusage.md)|[azureADFeatureUsage](../resources/azureadfeatureusage.md) collection|**TODO: Add Description**|
|[getAzureADApplicationSignInSummary](../api/reportroot-getazureadapplicationsigninsummary.md)|[applicationSignInSummary](../resources/applicationsigninsummary.md) collection|**TODO: Add Description**|
|[getCredentialUserRegistrationCount](../api/reportroot-getcredentialuserregistrationcount.md)|[credentialUserRegistrationCount](../resources/credentialuserregistrationcount.md) collection|**TODO: Add Description**|
|[getCredentialUsageSummary](../api/reportroot-getcredentialusagesummary.md)|[credentialUsageSummary](../resources/credentialusagesummary.md) collection|**TODO: Add -->

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|applicationSignInDetailedSummary|[коллекция applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)|Представляет подробную сводку регистрации приложения.|
|authenticationMethods|[authenticationMethodsRoot](../resources/authenticationmethodsroot.md)|Контейнер для свойств навигации для ресурсов методов проверки подлинности Azure AD.|
|credentialUserRegistrationDetails|[коллекция credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md)|Сведения об использовании сброса пароля самообслуживления и многофакторной проверки подлинности (MFA) для всех зарегистрированных пользователей.|
|userCredentialUsageDetails|[коллекция userCredentialUsageDetails](../resources/usercredentialusagedetails.md)|Представляет использование сброса пароля самообслуживщика (SSPR) для данного клиента.|

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
