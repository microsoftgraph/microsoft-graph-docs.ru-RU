---
title: Различия между типами ресурсов в Azure AD Graph и Microsoft Graph
description: Описываются различия между ресурсами в графике и ресурсах Azure AD в Microsoft Graph, которые помогут перенести приложения.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 96ff54b2f47aab40ac9096e00d6443964d2d23b4
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845913"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Различия между типами ресурсов в Azure AD Graph и Microsoft Graph

Эта статья входит в *Шаг 1: Ознакомьтесь с различиями* в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

При переносе приложений из Graph Azure AD в Microsoft Graph имейте в виду, что некоторые ресурсы имеют разные имена и типы.  Например, если приложение Azure AD Graph использует ресурс **тенантинфо** , вам потребуется обновить код, чтобы он ссылался на [организацию](/graph/api/resources/organization?view=graph-rest-1.0) .

В следующей таблице описываются различия между ресурсами Azure AD Graph и Microsoft Graph.  В нем отображаются ресурсы с отличающимися именами или недоступными; Кроме того, в ней выделяются ресурсы, доступные в бета-версии Microsoft Graph, но не в версии 1.0.

Если ресурс **не** отображается в этом списке, он уже доступен в [версии 1.0](/graph/api/overview?view=graph-rest-1.0) для Microsoft Graph с тем же именем, что и в Azure AD Graph.

> **Note**: имена типов ресурсов в Azure AD Graph в стиле Pascal, в то время как в Microsoft Graph они имеют стиль Camel.

|Azure AD Graph <br>ресурс (v 1.6) |Microsoft Graph<br>resource|Комментарии|
|---|---|---|
| [цертификатеаусоритинформатион](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [цертификатеаусорити](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>Версия 1.0 &nbsp; - &nbsp; [цертификатеаусорити](/graph/api/resources/certificateauthority?view=graph-rest-1.0) | |
| [контакт](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference); | бета- &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>Версия 1.0 &nbsp; - &nbsp; [orgContact](/graph/api/resources/orgContact?view=graph-rest-1.0) | |
| [директорилинкчанже](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; _новый &nbsp; способ_ бета-тестирования <br>&nbsp; - &nbsp; _новый &nbsp; способ_ версии 1.0 | Запрос Delta поддерживает обнаружение изменений связи с механизмом, который не требует использования этого ресурса. Ознакомьтесь [с различиями между функциями Azure AD Graph и Microsoft Graph](migrate-azure-ad-graph-feature-differences.md). |
| [OAuth2Permission](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-1.0) ||
| [PasswordProfile](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [passwordprofile необходима](/graph/api/resources/passwordProfile?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [passwordprofile необходима](/graph/api/resources/passwordProfile?view=graph-rest-1.0) ||
 [Политика](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [политики](/graph/api/resources/policy-overview?view=graph-rest-beta) бета-версий <br> версии 1.0 &nbsp; - &nbsp; [политики](/graph/api/resources/policy-overview?view=graph-rest-1.0)| Каждый тип политики имеет уникальное имя типа и структуру в сегменте пути URL-адреса **политик** в Microsoft Graph. В Azure AD Graph это был один тип политики. |
| [провисионинжеррор](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия &nbsp; - &nbsp; _недоступна_ <br> Версия 1.0 &nbsp; - &nbsp; _недоступна_ | Этот ресурс устарел.  Однако новый ресурс, описывающий все ошибки подготовки AD Connect, можно найти в [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-1.0). |
| [сервицеендпоинт](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp; - &nbsp; [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) бета-версии <br> &nbsp; - &nbsp; [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-1.0) версии 1.0 | [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) доступна только в составе ресурса [Group](/graph/api/resources/group?view=graph-rest-beta) .|
| [сигниннаме](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия &nbsp; - &nbsp; _пока недоступна_ <br> Версия 1.0 &nbsp; - &nbsp; _еще недоступна_ | Создание модели для идентификаторов, используемых для входа в учетную запись пользователя, которая называется **идентитйобжект**, но пока недоступна. Поддерживает сценарии B2C для Azure AD. |
| [тенантдетаил](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [Организация](/graph/api/resources/organization?view=graph-rest-beta) <br> Версия 1.0, &nbsp; - &nbsp; [Организация](/graph/api/resources/organization?view=graph-rest-1.0) | |
| [трустедкасфорпассвордаус](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [цертификатебаседаусконфигуратион](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [цертификатебаседаусконфигуратион](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-1.0) | |
| [UserIdentity](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- &nbsp; - &nbsp; [обжектидентити](/graph/api/resources/objectidentity?view=graph-rest-beta) <br> Версия 1.0 &nbsp; - &nbsp; [обжектидентити](/graph/api/resources/objectidentity?view=graph-rest-1.0) |  Новое моделирование идентификаторов, используемых для входа в учетную запись пользователя с именем **обжектидентити**. Поддерживает сценарии B2C для Azure AD. |

## <a name="next-steps"></a>Дальнейшие действия

- Сведения о [различиях свойств сущностей](migrate-azure-ad-graph-property-differences.md) в Azure AD Graph и Microsoft Graph.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .