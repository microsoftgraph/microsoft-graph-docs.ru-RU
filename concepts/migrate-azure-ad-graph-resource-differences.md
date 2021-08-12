---
title: Различия в типах ресурсов между Azure AD Graph и Microsoft Graph
description: Описывает различия между ресурсами в Azure AD Graph и ресурсами в Microsoft Graph, чтобы помочь перенести приложения.
author: dkershaw10
localization_priority: Normal
ms.prod: applications
ms.openlocfilehash: 5a02e165b84ae35299fe6b6b91e1c4eade61bcb1cd771a1aa43f92f6e4a468fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54174796"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Различия в типах ресурсов между Azure AD Graph и Microsoft Graph

Эта статья является *частью шага 1: просмотрите различия API* процесса переноса [приложений.](migrate-azure-ad-graph-planning-checklist.md)

При переносе приложений из Azure AD Graph Microsoft Graph, следует помнить, что некоторые ресурсы имеют разные имена и разные типы.  Например, если приложение Azure AD Graph использует ресурс **tenantInfo,** необходимо обновить код для ссылки [на организацию.](/graph/api/resources/organization?view=graph-rest-1.0)

В следующей таблице выделяются различия между ресурсами Azure AD Graph и Microsoft Graph.  В нем показаны ресурсы с разными именами или недоступными; он также выделяет ресурсы, доступные в бета-версии Microsoft Graph, но не в версии v1.0.

Если ресурс  не отображается в этом списке, он уже доступен в [версии v1.0](/graph/api/overview?view=graph-rest-1.0) Microsoft Graph с тем же именем, что и в Azure AD Graph.

> **ПРИМЕЧАНИЕ.** Имена типов ресурсов в Azure AD Graph pascal-cased, в то время как в Microsoft Graph — верблюды.

|Azure AD Graph <br>(v1.6) ресурс |Microsoft Graph<br>resource|Комментарии|
|---|---|---|
| [CertificateAuthorityInformation](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [бета-сертификатАторичность](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>v1.0 &nbsp; - &nbsp; [certificateAuthority](/graph/api/resources/certificateauthority?view=graph-rest-1.0) | |
| [Contact](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [бета-версия orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>v1.0 &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-1.0) | |
| [DirectoryLinkChange](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; _бета-новый &nbsp; подход_ <br>v1.0 &nbsp; - &nbsp; _Новый &nbsp; подход_ | Запрос Delta поддерживает обнаружение изменений отношений с помощью механизма, который не требует этого ресурса. См. [отличия функций между Azure AD Graph и Microsoft Graph.](migrate-azure-ad-graph-feature-differences.md) |
| [OAuth2Permission](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | beta &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-1.0) ||
 [Политика](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | политики &nbsp; - &nbsp; [бета-версии](/graph/api/resources/policy-overview?view=graph-rest-beta) <br> политики v1.0 &nbsp; - &nbsp; [](/graph/api/resources/policy-overview?view=graph-rest-1.0)| Каждый тип политики имеет уникальное имя типа  и структуру в сегменте url-адресов политик в Microsoft Graph. В Azure AD Graph это был один тип политики. Например, для Azure AD Graph работать с ресурсом **Политики** и  задать свойство типа , в то время как в Microsoft Graph это будет `TokenIssuancePolicy` ресурс **tokenIssuancePolicy.** |
| [ProvisioningError](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; _бета-версия недоступна_ <br> v1.0 &nbsp; - &nbsp; _Недоступны_ | Этот ресурс обесценив.  Однако в [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-1.0)можно найти новый ресурс, описывающий все ошибки, связанные с Подключение AD. |
| [ServiceEndpoint](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [Конечная точка бета-версии](/graph/api/resources/endpoint?view=graph-rest-beta) <br> конечная точка v1.0 &nbsp; - &nbsp; [](/graph/api/resources/endpoint?view=graph-rest-1.0) | **Конечные точки** доступны только [](/graph/api/resources/group?view=graph-rest-beta) как часть группового ресурса в бета-версии, так и ресурса [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) как в бета-версии, так и в v1.0.|
| [SignInName](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; _бета-новый подход_ <br> v1.0 &nbsp; - &nbsp; _Новый подход_ | Новое моделирование идентификаторов, используемых для входов в учетную запись пользователя. Дополнительные сведения см. в типе ресурса [objectIdentity.](/graph/api/resources/objectIdentity?view=graph-rest-1.0) Поддерживает сценарии Azure AD B2C. |
| [TenantDetail](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [бета-версия организации](/graph/api/resources/organization?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [организация](/graph/api/resources/organization?view=graph-rest-1.0) | |
| [TrustedCasForPasswordAuth](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [бета-сертификатBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [certificateBasedAuthConfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-1.0) | |
| [UserIdentity](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [бета-объект objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-beta) <br> v1.0 &nbsp; - &nbsp; [objectIdentity](/graph/api/resources/objectidentity?view=graph-rest-1.0) |  Новое моделирование идентификаторов, используемых для входов в учетную запись пользователя под названием **objectIdentity.** Поддерживает сценарии Azure AD B2C. |

## <a name="next-steps"></a>Дальнейшие действия

- Узнайте о [различиях свойств](migrate-azure-ad-graph-property-differences.md) объектов между Azure AD Graph и Microsoft Graph.
- Снова [просмотрите контрольный](migrate-azure-ad-graph-planning-checklist.md) список.