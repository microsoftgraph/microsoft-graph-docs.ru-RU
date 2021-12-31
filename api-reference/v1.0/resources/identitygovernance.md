---
title: Тип ресурса identityGovernance
description: Singleton для содержащих ресурсы управления удостоверением.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: be8bb2f562b05892f972431fd32db72b29af305a
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649685"
---
# <a name="identitygovernance-resource-type"></a>Тип ресурса identityGovernance

Пространство имен: microsoft.graph

Синглтон управления удостоверением — это контейнер для следующих Azure Active Directory функций управления удостоверением, которые будут выставлены с помощью следующих ресурсов и API:

+ [Проверки доступа](accessreviewsv2-overview.md)
+ [Управление правами](entitlementmanagement-overview.md)
+ [Согласие приложения](consentrequests-overview.md)
+ [Условия использования](agreement.md)

## <a name="methods"></a>Методы

Нет.

## <a name="properties"></a>Свойства

Нет

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|accessReviews|[accessReviewSet](accessreviewset.md)| Контейнер для базовых ресурсов, которые раскрывают API обзоров доступа и функций. В настоящее время предоставляется [только ресурс определений.](accessreviewscheduledefinition.md)|
|appConsent|[appConsent](appconsentapprovalroute.md)| Контейнер для базовых ресурсов, которые раскрывают API запроса на согласие приложения и функции. В настоящее время предоставляется [только ресурс appConsentRequests.](appconsentrequest.md)|
|entitlementManagement|[entitlementManagement](entitlementmanagement.md)| Контейнер для ресурсов управления правами, включая [accessPackageCatalog,](accesspackagecatalog.md) [connectedOrganization](connectedorganization.md)и [entitlementManagementSettings.](entitlementmanagementsettings.md)|
|termsOfUse|[termsOfUseContainer](termsofusecontainer.md)| Контейнер для ресурсов, которые раскрывают условия использования API [](agreement.md) и его функции, включая соглашения и [agreementAcceptances.](agreementacceptance.md) |

