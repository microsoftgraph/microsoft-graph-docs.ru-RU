---
title: Тип ресурса application
description: 'Представляет приложение. Любое приложение, передающее проверку подлинности в Azure Active Directory (Azure AD), должно быть зарегистрировано в каталоге. Регистрация приложения включает уведомление Azure AD о вашем приложении, в том числе URL-адрес его расположения, URL-адрес для отправки ответов после проверки подлинности, URI для определения приложения и многое другое. Дополнительную информацию см. в статье "Основные сведения о регистрации приложения в Azure AD". Наследуется от directoryObject. '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 694f6b12dd8fe1fd59f12cafebd47c842a4077cb
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641556"
---
# <a name="application-resource-type"></a>Тип ресурса application

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет приложение. Любое приложение, передающее проверку подлинности в Azure Active Directory (Azure AD), должно быть зарегистрировано в каталоге. Регистрация приложения включает уведомление Azure AD о вашем приложении, в том числе URL-адрес его расположения, URL-адрес для отправки ответов после проверки подлинности, URI для определения приложения и многое другое. Дополнительную информацию см. в статье [Основные сведения о регистрации приложения в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad). Наследуется от [directoryObject](directoryobject.md). 

> **Примечание.** В настоящее время разрабатываются изменения типа ресурса application. Дополнительные сведения см. в статье [Известные проблемы с Microsoft Graph](/graph/known-issues#application-and-serviceprincipal-api-changes).

Этот ресурс поддерживает:

- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/application-delta.md)).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Получение приложения](../api/application-get.md) | application |Считывание свойств и связей объекта application.|
|[Создание приложения](../api/application-post-applications.md) | application | Создает (регистрирует) новое приложение.|
|[Перечисление приложений](../api/application-list.md) | application | Получение списка приложений в организации. |
|[Обновление приложения](../api/application-update.md) | application |Обновление объекта application. |
|[Удаление приложения](../api/application-delete.md) | Нет |Удаление объекта application. |
|[Перечисление назначенных политик](../api/policy-list-assigned.md)| Коллекция [policy](policy.md)| Получение всех политик, назначенных объекту.|
|[Создание владельца](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Создание владельца путем добавления в коллекцию владельцев.|
|[Перечисление владельцев](../api/application-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов owner.|
|[delta](../api/application-delta.md)|Коллекция application| Получение добавочных изменений для приложений. |
|[Создание звонка](../api/application-post-calls.md)|[call](call.md)|Создание звонка путем добавления в коллекцию calls.|
|[Создание собрания по сети](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|Создание собрания по сети путем добавления в коллекцию onlineMeetings.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|api|[api](api.md)| Указывает параметры для приложения API. |
|appId| String | Уникальный идентификатор, назначенный для приложения с помощью Azure AD. Значение null не допускается. Только для чтения. |
|appRoles|Коллекция [appRole](approle.md)|Коллекция ролей приложения, которые могут быть объявлены приложением. Эти роли могут назначаться пользователям, группам или субъектам-службам. Значение null не допускается.|
|createdDateTime|DateTimeOffset| Дата и время регистрации приложения. |
|deletedDateTime|DateTimeOffset| Дата и время удаления приложения. |
|displayName|String|Отображаемое имя приложения. |
|id|String|Уникальный идентификатор приложения. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
|identifierUris|Коллекция String| URI, определяющие приложение. Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Для выражений фильтра в случае многозначных свойств требуется оператор *any*. Значение null не допускается. |
|info|[informationalUrl](informationalurl.md)| Основные сведения о профиле приложения. |
|isFallbackPublicClient|Boolean| Указывает резервный тип приложения как общедоступный клиент, например установленное приложение, запущенное на мобильном устройстве. Значение по умолчанию: *false*. Это означает, что резервный тип приложения является конфиденциальным клиентом, например веб-приложение. Существуют определенные сценарии, при которых Azure AD не удается определить тип приложения клиента (например, поток [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) с настройкой без указания URI перенаправления). В таких случаях Azure AD будет интерпретировать тип приложения на основе значения этого свойства.|
|keyCredentials|Коллекция [keyCredential](keycredential.md)|Коллекция ключевых учетных данных, связанных с приложением. Значение null не допускается. |
|logo|Stream|Основной логотип для приложения. Значение null не допускается. |
|optionalClaims|optionalClaims| Зарезервировано для последующего использования. |
|orgRestrictions|Коллекция String| Зарезервировано для последующего использования. |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |Указывает параметры родительского контроля для приложения.|
|passwordCredentials|Коллекция [passwordCredential](passwordcredential.md)|Коллекция учетных данных паролей, связанных с приложением. Значение null не допускается.|
|publicClient|[publicClient](publicclient.md)| Указывает параметры для установленных клиентов, например классических или мобильных устройств. |
|publisherDomain| String | Проверенный домен издателя для приложения. Только для чтения.|
|requiredResourceAccess|Коллекция [requiredResourceAccess](requiredresourceaccess.md)|Указывает ресурсы, к которым приложению требуется доступ, и устанавливает области разрешений OAuth и роли приложения, требующиеся приложению для каждого из этих ресурсов. Эта предварительная настройка доступа к необходимым ресурсам определяет интерфейс предоставления согласия. Значение null не допускается.|
|signInAudience | String | Указывает, какие учетные записи Майкрософт поддерживаются для текущего приложения. Поддерживаемые значения:<ul><li>**AzureADMyOrg**: пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD моей организации (т. е. один клиент)</li><li>**AzureADMultipleOrgs**: пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD любой организации (т. е. несколько клиентов)</li> <li>**AzureADandPersonalMicrosoftAccount**: пользователи с личной учетной записью Майкрософт, рабочей или учебной учетной записью в клиенте Azure AD любой организации</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|tags|Коллекция String| Настраиваемые строки, которые можно использовать для классификации и определения приложения. |
|web|[web](web.md)| Указывает параметры для веб-приложения. |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|calls           |Коллекция [call](call.md)                  |Только для чтения. Допускается значение null.|
|connectorGroup|[connectorGroup](connectorgroup.md)| Параметр connectorGroup, используемый приложением с Azure AD Application Proxy. Допускается значение null.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Только для чтения.|
|onlineMeetings  |Коллекция [onlineMeeting](onlinemeeting.md)|Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, владеющие приложением. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект. Требуется версия 2013-11-08 или более поздняя. Только для чтения. Допускается значение null.|
|policy|Коллекция [policy](policy.md)|Политики, назначенные приложению.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": true,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "optionalClaims": [{"@odata.type": "microsoft.graph.optionalClaims"}],
  "orgRestrictions": ["Guid"],
  "parentalControlSettings": [{"@odata.type": "microsoft.graph.parentalControlSettings"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "web": {"@odata.type": "microsoft.graph.webApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/application.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
