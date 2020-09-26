---
title: Различия между типами ресурсов в Azure AD Graph и Microsoft Graph
description: Описываются различия между ресурсами в графике и ресурсах Azure AD в Microsoft Graph, которые помогут перенести приложения.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 7844235b1665c06911b8280f8f95517796b34348
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289101"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Различия между типами ресурсов в Azure AD Graph и Microsoft Graph

Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

При переносе приложений из Graph Azure AD в Microsoft Graph имейте в виду, что некоторые ресурсы имеют разные имена и типы.  Например, если приложение Azure AD Graph использует ресурс **тенантинфо** , вам потребуется обновить код, чтобы он ссылался на [организацию](/graph/api/resources/organization?view=graph-rest-1.0) .

В следующей таблице описываются различия между ресурсами Azure AD Graph и Microsoft Graph.  В нем отображаются ресурсы с отличающимися именами или недоступными; Кроме того, в ней выделяются ресурсы, доступные в бета-версии Microsoft Graph, но не в версии 1.0.

Если ресурс **не** отображается в этом списке, он уже доступен в [версии 1.0](/graph/api/overview?view=graph-rest-1.0) для Microsoft Graph с тем же именем, что и в Azure AD Graph.

> **Note**: имена типов ресурсов в Azure AD Graph в стиле Pascal, в то время как в Microsoft Graph они имеют стиль Camel.

|Azure AD Graph <br>ресурс (v 1.6) |Microsoft Graph<br>resource|Комментарии|
|---|---|---|
| [цертификатеаусоритинформатион](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [цертификатеаусорити](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>Версия 1.0 &nbsp; - &nbsp; [цертификатеаусорити](/graph/api/resources/certificateauthority?view=graph-rest-1.0) | |
| [Contact](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>Версия 1.0 &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-1.0) | |
| [директорилинкчанже](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; _новый &nbsp; способ_ бета-тестирования <br>&nbsp; - &nbsp; _новый &nbsp; способ_ версии 1.0 | Запрос Delta поддерживает обнаружение изменений связи с механизмом, который не требует использования этого ресурса. Ознакомьтесь [с различиями между функциями Azure AD Graph и Microsoft Graph](migrate-azure-ad-graph-feature-differences.md). |
| [OAuth2Permission](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-1.0) ||
 [Политика](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [политики](/graph/api/resources/policy-overview?view=graph-rest-beta) бета-версий <br> версии 1.0 &nbsp; - &nbsp; [политики](/graph/api/resources/policy-overview?view=graph-rest-1.0)| Каждый тип политики имеет уникальное имя типа и структуру в сегменте пути URL-адреса **политик** в Microsoft Graph. В Azure AD Graph это был один тип политики. Например, для Azure AD Graph вы будете работать с ресурсом **Policy** и присвоить свойству **Type** значение `TokenIssuancePolicy` , в то время как в Microsoft Graph это будет ресурс **токениссуанцеполици** . |
| [провисионинжеррор](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия &nbsp; - &nbsp; _недоступна_ <br> Версия 1.0 &nbsp; - &nbsp; _недоступна_ | Этот ресурс устарел.  Однако новый ресурс, описывающий все ошибки подготовки AD Connect, можно найти в [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-1.0). |
| [сервицеендпоинт](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) бета-версии <br> &nbsp; - &nbsp; [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-1.0) версии 1.0 | **конечные точки** доступны только в рамках ресурса [группы](/graph/api/resources/group?view=graph-rest-beta) в бета-версии, а ресурс [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-1.0) в бета-версиях и версии 1.0.|
| [сигниннаме](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; _новый способ_ бета-тестирования <br> &nbsp; - &nbsp; _новый способ_ версии 1.0 | Новое моделирование идентификаторов, используемых для входа в учетную запись пользователя. Для получения дополнительных сведений см. тип ресурса [обжектидентити](/graph/api/resources/objectIdentity?view=graph-rest-1.0) . Поддерживает сценарии B2C для Azure AD. |
| [тенантдетаил](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [Организация](/graph/api/resources/organization?view=graph-rest-beta) <br> Версия 1.0, &nbsp; - &nbsp; [Организация](/graph/api/resources/organization?view=graph-rest-1.0) | |
| [трустедкасфорпассвордаус](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [цертификатебаседаусконфигуратион](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [цертификатебаседаусконфигуратион](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-1.0) | |
| [UserIdentity](/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [обжектидентити](/graph/api/resources/objectidentity?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [обжектидентити](/graph/api/resources/objectidentity?view=graph-rest-1.0) |  Новое моделирование идентификаторов, используемых для входа в учетную запись пользователя с именем **обжектидентити**. Поддерживает сценарии B2C для Azure AD. |

## <a name="next-steps"></a>Дальнейшие действия

- Сведения о [различиях свойств сущностей](migrate-azure-ad-graph-property-differences.md) в Azure AD Graph и Microsoft Graph.
- Снова просмотрите [Контрольный список](migrate-azure-ad-graph-planning-checklist.md) .