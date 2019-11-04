---
title: Различия между типами ресурсов в Azure AD Graph и Microsoft Graph
description: Описываются различия между ресурсами в графике и ресурсах Azure AD в Microsoft Graph, которые помогут перенести приложения.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 925faf5aa27adcdef3d0ade88f9c3d5d8a911c75
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37934741"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Различия между типами ресурсов в Azure AD Graph и Microsoft Graph

Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

При переносе приложений из Graph Azure AD в Microsoft Graph имейте в виду, что некоторые ресурсы имеют разные имена и типы.  Например, если приложение Azure AD Graph использует ресурс **тенантинфо** , вам потребуется обновить код, чтобы он ссылался на [организацию](/graph/api/resources/organization?view=graph-rest-1.0) .

В следующей таблице описываются различия между ресурсами Azure AD Graph и Microsoft Graph.  В нем отображаются ресурсы с отличающимися именами или недоступными; Кроме того, в ней выделяются ресурсы, доступные в бета-версии Microsoft Graph, но не в версии 1.0.

Если ресурс не отображается в этом списке, он уже доступен в [версии 1.0](/graph/api/overview?view=graph-rest-1.0) для Microsoft Graph с тем же именем, что и в Azure AD Graph.

> **Note**: имена типов ресурсов в Azure AD Graph в стиле Pascal, в то время как в Microsoft Graph они имеют стиль Camel.

|Azure AD Graph <br>ресурс (v 1.6) |Microsoft Graph<br>resource|Комментарии|
|---|---|---|
| [Application](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия [приложения](/graph/api/resources/application?view=graph-rest-beta)<br>v 1.0 — [приложение](/graph/api/resources/application?view=graph-rest-1.0) ||
| [аппроле](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [аппроле](/graph/api/resources/approle?view=graph-rest-beta)<br>Версия 1.0 — [аппроле](/graph/api/resources/appRole?view=graph-rest-1.0) | |
| [аппролеассигнмент](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-[аппролеассигнмент](/graph/api/resources/approleassignment?view=graph-rest-beta)<br>Версия 1.0 _еще недоступна_ | |
| [цертификатеаусоритинформатион](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-[цертификатеаусорити](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>Версия 1.0&nbsp;-&nbsp;[цертификатеаусорити](/graph/api/resources/certificateauthority?view=graph-rest-v1.0) | |
| [Contact](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>Версия 1.0 — [orgContact](/graph/api/resources/orgContact?view=graph-rest-v1.0) | |
| [директорилинкчанже](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | _новый&nbsp;подход_ к бета-версии <br>v 1.0 — _новый&nbsp;подход_ | Запрос Delta поддерживает обнаружение изменений связи с механизмом, который не требует использования этого ресурса. Ознакомьтесь [с различиями между функциями Azure AD Graph и Microsoft Graph](migrate-azure-ad-graph-feature-differences.md). |
| [OAuth2Permission](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> Версия 1.0 — [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-1.0) ||
| [OAuth2PermissionGrant](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-[oAuth2PermissionGrant](/graph/api/resources/oAuth2PermissionGrant?view=graph-rest-beta) <br> Версия 1.0 _еще недоступна_ ||
| [PasswordProfile](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [passwordprofile необходима](/graph/api/resources/passwordProfile?view=graph-rest-beta) <br> Версия 1.0 — Passwordprofile необходима ||
| [Политика](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [Политика](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) _(подлежит изменению)_ <br> Версия 1.0 _еще недоступна_ | Каждая политика будет иметь уникальное имя типа и структуру.|
| [провисионинжеррор](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-версия_недоступна_ <br> Версия 1.0&nbsp;-&nbsp;_недоступна_ | Этот ресурс устарел.  Однако новый ресурс, описывающий все ошибки подготовки AD Connect, можно найти в [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-v1.0). |
| [сервицеендпоинт](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) <br> Версия 1.0 — конечная точка _пока недоступна_ | [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) доступна только в составе ресурса [Group](/graph/api/resources/group?view=graph-rest-beta) .|
| [ServicePrincipal](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) <br> Версия 1.0 _еще недоступна_ | |
| [сигниннаме](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия _еще недоступна_ <br> Версия 1.0 _еще недоступна_ | Создание модели для идентификаторов, используемых для входа в учетную запись пользователя, которая называется **идентитйобжект**, но пока недоступна. Поддерживает сценарии B2C для Azure AD. |
| [тенантдетаил](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [Организация](/graph/api/resources/organization?view=graph-rest-beta) <br> v 1.0 — [Организация](/graph/api/resources/organization?view=graph-rest-v1.0) | |
| [трустедкасфорпассвордаус](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-[цертификатебаседаусконфигуратион](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> Версия 1.0&nbsp;-&nbsp;[цертификатебаседаусконфигуратион](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-v1.0) | |
| [UserIdentity](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия _еще недоступна_ <br> Версия 1.0 _еще недоступна_ |  Создание модели для идентификаторов, используемых для входа в учетную запись пользователя, которая называется **идентитйобжект**, но пока недоступна. Поддерживает сценарии B2C для Azure AD. |

## <a name="next-steps"></a>Дальнейшие действия

- Сведения о [различиях свойств сущностей](migrate-azure-ad-graph-property-differences.md) в Azure AD Graph и Microsoft Graph.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
