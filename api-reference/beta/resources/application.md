---
title: Тип ресурса приложения
description: 'Представляет приложение. Любое приложение, которое outsources проверка подлинности Azure Active Directory (Azure AD) должны быть зарегистрированы в каталоге. Регистрация приложения включает в себя Azure AD сообщает о приложении, включая URL-адрес, где он находится, URL-адрес для отправки ответов после проверки подлинности, URI для идентификации приложения и многое другое. Для получения дополнительных сведений см. основные сведения о регистрации приложения в Azure AD. Наследуется от directoryObject. '
localization_priority: Priority
ms.openlocfilehash: b64de5670ccb9deebbabe32bb691d15b5a621f30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805672"
---
# <a name="application-resource-type"></a>Тип ресурса приложения

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет приложение. Любое приложение, которое outsources проверка подлинности Azure Active Directory (Azure AD) должны быть зарегистрированы в каталоге. Регистрация приложения включает в себя Azure AD сообщает о приложении, включая URL-адрес, где он находится, URL-адрес для отправки ответов после проверки подлинности, URI для идентификации приложения и многое другое. Для получения дополнительных сведений см. [Основные сведения о регистрации приложения в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad). Наследуется от [directoryObject](directoryobject.md). 

> **Примечание:** Тип ресурса приложения изменяются в настоящее время при разработке. Для получения дополнительных сведений см [Известные проблемы, связанные с Microsoft Graph](/graph/known-issues#application-and-serviceprincipal-api-changes).

Этот ресурс поддерживает:

- отслеживание дополнений, удалений и обновлений с помощью [запроса изменений](/graph/delta-query-overview) (функция [delta](../api/application-delta.md)).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Получение приложения](../api/application-get.md) | application |Чтение свойства и связи объекта приложения.|
|[Создание приложения](../api/application-post-applications.md) | application | (Регистрах) создает новое приложение.|
|[Список приложений](../api/application-list.md) | application | Извлечь список приложений в организации. |
|[Обновление приложения](../api/application-update.md) | application |Обновление объекта приложения. |
|[Удаление приложения](../api/application-delete.md) | Нет |Удаление объекта приложения. |
|[Список назначенных политик](../api/policy-list-assigned.md)| [политики](policy.md) семейства сайтов| Получите все политики, назначенные для этого объекта.|
|[Создание владельца](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Создайте новый владелец, отправку сообщений владельцев семейства.|
|[Список владельцев](../api/application-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение владельца коллекции объектов.|
|[delta](../api/application-delta.md)|коллекции приложения| Получите добавочные изменения для приложений. |
|[Создание вызова](../api/application-post-calls.md)|[звонок](call.md)|Создайте новый звонок, отправку сообщений в коллекцию звонки.|
|[Создание собрания по сети](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|Создание нового собрания по сети с отправку сообщений в коллекцию onlineMeetings.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|API|[API](api.md)| Задает параметры для приложения API. |
|appId| String | Уникальный идентификатор для приложения, назначаемый приложению Azure AD. Значение null не допускается. Только для чтения. |
|appRoles|Коллекция [роли приложения](approle.md)|Коллекция ролей приложений, которые могут объявить приложения. Эти роли можно назначить только пользователей, групп и субъектов-служб. Значение null не допускается.|
|createdDateTime|DateTimeOffset| Дата и время регистрации приложения. |
|deletedDateTime|DateTimeOffset| Дата и время приложения был удален. |
|displayName|Строка|Отображаемое имя для приложения. |
|id|Строка|Уникальный идентификатор для приложения. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
|identifierUris|Коллекция String| Коды URI, определения приложения. Дополнительные сведения содержатся, [приложения и объекты участников-служб](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). *Любой* оператор является обязательным для выражения фильтра с несколькими значениями свойств. Значение null не допускается. |
|сведения о|[informationalUrl](informationalurl.md)| Сведения о базовой профиля приложения. |
|isFallbackPublicClient|Логический| Указывает тип возврата приложения как общедоступный клиентом, например установленные приложения, работающего на мобильном устройстве. Значение по умолчанию — *значение false,* что означает, что тип возврата приложения является конфиденциальным клиентом, например веб-приложения. Существуют некоторые сценарии, где Azure AD не может определить тип клиентского приложения (например [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) поток где настроен без указания URI перенаправления). В таких случаях Azure AD интерпретирует типа приложения, в зависимости от значения этого свойства.|
|keyCredentials|[keyCredential](keycredential.md) коллекции|Коллекция ключа учетных данных, связанных с приложением, не допускает значение NULL. |
|logo|Stream|Основной логотип для приложения. Значение null не допускается. |
|optionalClaims|optionalClaims| Зарезервировано для последующего использования. |
|orgRestrictions|Коллекция String| Зарезервировано для последующего использования. |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |Указывает параметры родительского элемента управления для приложения.|
|passwordCredentials|[passwordCredential](passwordcredential.md) коллекции|Коллекция пароль учетных данных, связанных с приложением. Значение null не допускается.|
|publicClient|[publicClient](publicclient.md)| Задает параметры для установленных клиентов, таких как настольного компьютера или мобильного устройства. |
|publisherDomain| Строка | Домен подтвержденным publisher для приложения. Только для чтения.|
|requiredResourceAccess|[requiredResourceAccess](requiredresourceaccess.md) коллекции|Указывает ресурсы, которые этого приложения требуется доступ к и набор области разрешений OAuth и роли приложений, которые требуется в каждом из этих ресурсов. В этом предварительной настройки доступа к необходимых ресурсов дисков на взаимодействие с согласия пользователя. Значение null не допускается.|
|signInAudience | Строка | Указывает, какие учетные записи Microsoft поддерживаются для текущего приложения. Приведены поддерживаемые значения.<ul><li>**AzureADMyOrg**: работы пользователей с помощью Microsoft или школе учетной записи в моей организации Azure AD для клиентов (то есть одним клиентом)</li><li>**AzureADMultipleOrgs**: работы пользователей с помощью Microsoft или школы учетной записи в любой организации Azure AD для клиентов (то есть многопользовательские)</li> <li>**AzureADandPersonalMicrosoftAccount**: пользователи, имеющие личная учетная запись Майкрософт или рабочего или школы учетной записи в любой организации Azure AD для клиентов</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|теги|Коллекция String| Настраиваемых строк, которые можно использовать для классификации и определения приложения. |
|web|[Web](web.md)| Задает параметры для веб-приложения. |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|звонки           |[вызов](call.md) семейства сайтов                  |Только для чтения. Допускается значение null.|
|connectorGroup|[connectorGroup](connectorgroup.md)| ConnectorGroup приложение использует с прокси-сервером приложения Azure AD. Допускается значение null.|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Только для чтения.|
|onlineMeetings  |[onlineMeeting](onlinemeeting.md) коллекции|Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталога, являющиеся владельцами приложения. Владельцы — это набор пользователей без прав администратора, которые могут изменять этот объект. Требуется версия 2013-11-08 или более поздней версии. Только для чтения. Допускается значение null.|
|политика|[политики](policy.md) семейства сайтов|Политики, назначенные для этого приложения.|

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
<!-- {
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
