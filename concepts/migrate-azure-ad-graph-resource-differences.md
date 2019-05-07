---
title: Различия между типами ресурсов в Azure AD Graph и Microsoft Graph
description: Описываются различия между ресурсами в графике и ресурсах Azure AD в Microsoft Graph, которые помогут перенести приложения.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 590ec2fae33e5172e274341793c82409a4c28c8c
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630204"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Различия между типами ресурсов в Azure AD Graph и Microsoft Graph

Эта статья входит в *Шаг 1: ознакомьтесь* с различиями в API [процесса переноса приложений](migrate-azure-ad-graph-planning-checklist.md).

При переносе приложений из Graph Azure AD в Microsoft Graph имейте в виду, что некоторые ресурсы имеют разные имена и типы.  Например, если приложение Azure AD Graph использует ресурс **тенантинфо** , вам потребуется обновить код, чтобы он ссылался на [организацию](/graph/api/resources/organization?view=graph-rest-1.0) .

В следующей таблице описываются различия между ресурсами Azure AD Graph и Microsoft Graph.  В нем отображаются ресурсы с отличающимися именами или недоступными; Кроме того, в ней выделяются ресурсы, доступные в бета-версии Microsoft Graph, но не в версии 1.0.

Если ресурс не отображается в этом списке, он уже доступен в [версии 1.0](/graph/api/overview?view=graph-rest-1.0) для Microsoft Graph с тем же именем, что и в Azure AD Graph.

> **Note**: имена типов ресурсов в Azure AD Graph в стиле Pascal, в то время как в Microsoft Graph они имеют стиль Camel.

|Azure AD Graph <br>ресурс (v 1.6) |Microsoft Graph<br>resource|Comments|
|---|---|---|
| [Надстройк](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference)       | бета-версия _еще_ недоступна<br>Версия 1.0 _еще_ недоступна ||
| [Приложение](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия [приложения](/graph/api/resources/application?view=graph-rest-beta)<br>Версия 1.0 _еще_ недоступна ||
| [Аппроле](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [аппроле](/graph/api/resources/approle?view=graph-rest-beta)<br>Версия 1.0 _еще_ недоступна | |
| [Аппролеассигнмент](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-[аппролеассигнмент](/graph/api/resources/approleassignment?view=graph-rest-beta)<br>Версия 1.0 _еще_ недоступна | |
| [Contact](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [orgContact](/graph/api/resources/orgContact?view=graph-rest-beta)<br>Версия 1.0 _еще_ недоступна | |
| [Директорилинкчанже](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | _новый&nbsp;подход_ к бета-версии <br>v 1.0 — _новый&nbsp;подход_ | Запрос Delta поддерживает обнаружение изменений связи с механизмом, который не требует использования этого ресурса. Ознакомьтесь [с различиями между функциями Azure AD Graph и Microsoft Graph](migrate-azure-ad-graph-feature-differences.md). |
| [Кэйкредентиал](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference)| бета- [кэйкредентиал](/graph/api/resources/keyCredential?view=graph-rest-beta)<br>Версия 1.0 _еще_ недоступна | |
| [Ключзначение](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [ключзначение](/graph/api/resources/keyValue?view=graph-rest-beta) <br> Версия 1.0 _еще_ недоступна ||
| [OAuth2Permission](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [permissionScope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> Версия 1.0 _еще_ недоступна ||
| [OAuth2PermissionGrant](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-[oAuth2PermissionGrant](/graph/api/resources/oAuth2PermissionGrant?view=graph-rest-beta) <br> Версия 1.0 _еще_ недоступна ||
| [Оптионалклаим](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-Оптионалклаим <br> Версия 1.0 _еще_ недоступна | |
| [Оптионалклаимс](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-Оптионалклаимс<br> Версия 1.0 _еще_ недоступна ||
| [Паренталконтролсеттингс](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [паренталконтролсеттингс](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) <br> Версия 1.0 _еще_ недоступна ||
| [Пассвордкредентиал](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [пассвордкредентиал](/graph/api/resources/passwordCredential?view=graph-rest-beta) <br> Версия 1.0 _еще_ недоступна ||
| [PasswordProfile](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [passwordprofile необходима](/graph/api/resources/passwordProfile?view=graph-rest-beta) <br> Версия 1.0 — Passwordprofile необходима ||
| [Политика](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [Политика](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) _(подлежит изменению)_ <br> Версия 1.0 _еще_ недоступна | Каждая политика будет иметь уникальное имя типа и структуру.|
| [Провисионинжеррор](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-[onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-beta) <br> Версия 1.0&nbsp;-&nbsp;onPremisesProvisioningError  | |
| [Рекуиредресаурцеакцесс](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [рекуиредресаурцеакцесс](/graph/api/resources/requiredResourceAccess?view=graph-rest-beta) <br> Версия 1.0 _еще_ недоступна | |
| [Ресаурцеакцесс](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [ресаурцеакцесс](/graph/api/resources/resourceAccess?view=graph-rest-beta) <br> Версия 1.0 _еще_ недоступна | |
| [Сервицеендпоинт](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) <br> Версия 1.0 — конечная точка _пока_ недоступна | [Конечная точка](/graph/api/resources/endpoint?view=graph-rest-beta) доступна только в составе ресурса [группы](/graph/api/resources/group?view=graph-rest-beta)|
| [ServicePrincipal](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) <br> Версия 1.0 _еще_ недоступна | |
| [Сигниннаме](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия _еще_ недоступна <br> Версия 1.0 _еще_ недоступна | Создание модели для идентификаторов, используемых для входа в учетную запись пользователя, которая называется **идентитйобжект**, но пока недоступна. Поддерживает сценарии B2C для Azure AD. |
| [Тенантдетаил](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета- [Организация](/graph/api/resources/organization?view=graph-rest-beta) <br> v 1.0 — [Организация](/graph/api/resources/organization?view=graph-rest-v1.0) | |
| [Трустедкасфорпассвордаус](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета&nbsp;-&nbsp;-версия_пока_ недоступна <br> Версия 1.0 _еще_ недоступна  | Переименование в **цертификатебаседаусконфигуратион** , но пока недоступно.|
| [UserIdentity](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | бета-версия _еще_ недоступна <br> Версия 1.0 _еще_ недоступна |  Создание модели для идентификаторов, используемых для входа в учетную запись пользователя, которая называется **идентитйобжект**, но пока недоступна. Поддерживает сценарии B2C для Azure AD. |

## <a name="next-steps"></a>Дальнейшие действия

- Сведения о [различиях свойств сущностей](migrate-azure-ad-graph-property-differences.md) в Azure AD Graph и Microsoft Graph.
- Ознакомьтесь с основными понятиями и рекомендациями [Microsoft Graph](/graph/overview) .
- Поэкспериментируйте с Microsoft Graph с помощью [проводника диаграмм](https://aka.ms/ge) .
