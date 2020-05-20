---
title: Тип ресурса application
description: Представляет приложение.
localization_priority: Priority
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 27dc4650fa177dcba4d691d2c0d51985fc06e8a4
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290478"
---
# <a name="application-resource-type"></a>Тип ресурса application

Пространство имен: microsoft.graph

Представляет приложение. Любое приложение, передающее проверку подлинности в Azure Active Directory (Azure AD), должно быть зарегистрировано в каталоге. Регистрация приложения включает уведомление Azure AD о вашем приложении, в том числе URL-адрес его расположения, URL-адрес для отправки ответов после проверки подлинности, URI для определения приложения и многое другое. Дополнительную информацию см. в статье [Основные сведения о регистрации приложения в Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad). Наследуется от [directoryObject](directoryobject.md).

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/application-delta.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Перечисление приложений](../api/application-list.md) | Коллекция [application](application.md) | Получение списка приложений в организации. |
|[Создание приложения](../api/application-post-applications.md) | [application](application.md) | Создает (регистрирует) новое приложение.|
|[Получение приложения](../api/application-get.md) | [application](application.md) |Считывание свойств и связей объекта application.|
|[Обновление приложения](../api/application-update.md) | [application](application.md) |Обновление объекта application. |
|[Удаление приложения](../api/application-delete.md) | Нет |Удаление объекта application. |
|[Получение дельты](../api/application-delta.md)|[application](application.md)|Создавайте, обновляйте или удаляйте приложения без необходимости чтения всей коллекции ресурсов.|
|[Список удаленных приложений](../api/directory-deleteditems-list.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка недавно удаленных приложений. |
|[Получение удаленного приложения](../api/directory-deleteditems-get.md) | [directoryObject](directoryobject.md) | Получение свойств недавно удаленного приложения. |
|[Окончательное удаление приложения](../api/directory-deleteditems-delete.md) | Нет | Окончательное удаление приложения. |
|[Восстановление удаленного приложения](../api/directory-deleteditems-restore.md) | [directoryObject](directoryobject.md) | Восстановление недавно удаленного приложения. |
|**Сертификаты и секреты**| | |
|[Добавление пароля](../api/application-addpassword.md)|[passwordCredential](passwordcredential.md)|Добавление надежного пароля в приложение.|
|[Удаление пароля](../api/application-removepassword.md)|[passwordCredential](passwordcredential.md)|Удаление пароля приложения.|
|[Клавиша прибавления](../api/application-addkey.md)|[кэйкредентиал](keycredential.md)|Добавление в приложение учетных данных ключа.|
|[Удалить ключ](../api/application-removekey.md)|Нет|Удаление ключевых учетных данных из приложения.|
|**Extensions**| | |
| [Список расширений](../api/application-list-extensionproperty.md) | Коллекция [extensionProperty](extensionProperty.md) | Список свойств расширения для объекта application. |
| [Создание расширения](../api/application-post-extensionproperty.md) | [extensionProperty](extensionProperty.md) | Создание свойства расширения для объекта application. |
| [Удаление расширения](../api/application-delete-extensionproperty.md) | Нет | Удаление свойства расширения объекта application. |
|**Owners**| | |
|[Перечисление владельцев](../api/application-list-owners.md) |Коллекция [directoryObject](directoryobject.md)| Получение коллекции объектов owner.|
|[Добавление владельца](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| Добавление владельца путем помещения в коллекцию владельцев.|
|[Удаление владельца](../api/application-delete-owners.md) |Нет| Удаление владельца приложения.|
|[Назначение типа ресурса tokenLifetimePolicy](../api/application-post-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Назначение типа ресурса tokenLifetimePolicy объекту.|
|[Перечисление типов ресурсов tokenLifetimePolicy](../api/application-list-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Получение всех типов ресурсов tokenLifetimePolicies, назначенных объекту.|
|[Удаление типа ресурса tokenLifetimePolicy](../api/application-delete-tokenlifetimepolicies.md)| Коллекция [tokenLifetimePolicy](tokenlifetimepolicy.md)| Удаление типа ресурса tokenLifetimePolicy из объекта.|
|[Назначить tokenIssuancePolicy](../api/application-post-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Присвойте tokenIssuancePolicy этому объекту.|
|[Перечислить tokenIssuancePolicies](../api/application-list-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Назначьте все tokenIssuancePolicies этому объекту.|
|[Убрать tokenIssuancePolicy](../api/application-delete-tokenissuancepolicies.md)| [tokenIssuancePolicy](tokenissuancepolicy.md) Коллекция| Удалите tokenIssuancePolicy из этого объекта.|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
| addIns | Коллекция [addIn](addin.md)| Определяет пользовательское поведение, которое служба может использовать для вызова приложения в определенных контекстах. Например, приложения, которые способны визуализировать файловые потоки, [могут установить свойство addIns](https://docs.microsoft.com/onedrive/developer/file-handlers/?view=odsp-graph-online) для его функции "FileHandler". Это позволит таким службам, как Office 365, вызывать приложение в контексте документов, над которыми работает пользователь. |
| api | [apiApplication](apiapplication.md) | Задает параметры приложения, реализующего веб-API. |
| appId | String | Уникальный идентификатор, назначенный для приложения с помощью Azure AD. Значение null не допускается. Только для чтения. |
| appRoles | Коллекция [appRole](approle.md) | Коллекция ролей, объявляемых приложением. С помощью [назначений ролей приложений](approleassignment.md)эти роли могут быть назначены пользователям, группам или субъектам служб других приложений. Значение null не допускается. |
| createdDateTime | DateTimeOffset | Дата и время регистрации приложения. Только для чтения. |
| deletedDateTime | DateTimeOffset | Дата и время удаления приложения. Только для чтения. |
| displayName | Строка | Отображаемое имя приложения. |
| groupMembershipClaims | String | Настраивает утверждение `groups`, выданное в маркере пользователя или маркере доступа OAuth 2.0, которого ожидает приложение. Чтобы задать этот атрибут, используйте одно из следующих допустимых строковых значений.<ul><li>`None`</li><li>`SecurityGroup` — для групп безопасности и ролей Azure AD</li><li>`All` — предоставит все группы безопасности, группы рассылки и роли каталога Azure AD, членом которых является выполнивший вход пользователь</li></ul> |
| id | Строка | Уникальный идентификатор приложения. Наследуется от [directoryObject](directoryobject.md). Ключ. Значение null не допускается. Только для чтения. |
| identifierUris | Коллекция String | URI, идентифицирующие приложение в клиенте Azure AD или в проверенном личном домене, если приложение является мультитенантным. Дополнительные сведения см. в статье [Объекты приложения и субъекта-службы](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals). Для выражений фильтра в случае многозначных свойств требуется оператор *any*. Значение null не допускается. |
| info | [informationalUrl](informationalurl.md) | Базовые данные профиля для приложения, такие как URL-адреса маркетинга, поддержки, условий обслуживания и заявления о конфиденциальности. Условия обслуживания и заявление о конфиденциальности отображаются в окне запроса согласия пользователя. Дополнительные сведения см. в статье [Добавление условий обслуживания и заявления о конфиденциальности для зарегистрированных приложений Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). |
| isFallbackPublicClient | Boolean | Указывает резервный тип приложения как общедоступный клиент, например установленное приложение, запущенное на мобильном устройстве. Значение по умолчанию — `false`. Это означает, что резервный тип приложения является конфиденциальным клиентом, таким как веб-приложение. Существуют определенные сценарии, при которых Azure AD не удается определить тип клиентского приложения (например, поток [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) с настройкой без указания URI перенаправления). В таких случаях Azure AD будет интерпретировать тип приложения на основе значения этого свойства.|
| keyCredentials | Коллекция [keyCredential](keycredential.md) | Коллекция ключевых учетных данных, связанных с приложением. Значение null не допускается. |
| logo | Stream | Основной логотип для приложения. Значение null не допускается. |
| optionalClaims | [optionalClaims](optionalclaims.md) | Разработчики приложений могут настраивать необязательные утверждения в своих приложениях Azure AD, чтобы указать, какие утверждения им нужны в маркерах, отправляемых в приложения службой маркеров безопасности (Майкрософт). Дополнительные сведения см. в статье [Предоставление необязательных утверждений для приложения Azure AD](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).|
| parentalControlSettings | [parentalControlSettings](parentalcontrolsettings.md) |Указывает параметры родительского контроля для приложения. |
| passwordCredentials | Коллекция [passwordCredential](passwordcredential.md)|Коллекция учетных данных паролей, связанных с приложением. Значение null не допускается.|
| publicClient | [publicClientApplication](publicclientapplication.md) | Указывает параметры для установленных клиентов, например классических или мобильных устройств. |
| publisherDomain | String | Проверенный домен издателя для приложения. Только для чтения.|
| requiredResourceAccess |Коллекция [requiredResourceAccess](requiredresourceaccess.md)|Указывает ресурсы, к которым приложению требуется доступ, и устанавливает области разрешений OAuth и роли приложения, требующиеся приложению для каждого из этих ресурсов. Эта предварительная настройка доступа к необходимым ресурсам определяет интерфейс предоставления согласия. Значение null не допускается.|
| signInAudience | String | Указывает, какие учетные записи Майкрософт поддерживаются для текущего приложения. Поддерживаемые значения:<ul><li>`AzureADMyOrg` — пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD моей организации (т. е. один клиент)</li><li>`AzureADMultipleOrgs` — пользователи с рабочей или учебной учетной записью Майкрософт в клиенте Azure AD любой организации (т. е. несколько клиентов)</li> <li>`AzureADandPersonalMicrosoftAccount` — пользователи с личной учетной записью Майкрософт, рабочей или учебной учетной записью в клиенте Azure AD любой организации</li></ul> |
| tags |Коллекция String| Настраиваемые строки, которые можно использовать для классификации и определения приложения. Значение null не допускается.|
| tokenEncryptionKeyId |String|Задает значение открытого ключа keyId из коллекции keyCredentials. При настройке Azure AD шифрует все созданные маркеры с помощью ключа, на который указывает это свойство. Код приложения, получающий зашифрованный маркер, должен использовать соответствующий закрытый ключ для расшифровки маркера, прежде чем его можно будет применить для пользователя, выполнившего вход.|
| web |[webApplication](webapplication.md)| Указывает параметры для веб-приложения. |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
|:---------------|:--------|:----------|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| Только для чтения.|
|extensionProperties|Коллекция [extensionProperty](extensionproperty.md)| Только для чтения. Допускается значение null.|
|owners|Коллекция [directoryObject](directoryobject.md)|Объекты каталогов, владеющие приложением. Владельцы — это группа пользователей, которые не являются администраторами и которым разрешено изменять объект. Требуется версия 2013-11-08 или более поздняя. Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "addIns": [{"@odata.type": "microsoft.graph.addIn"}],
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "groupMembershipClaims": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": false,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "optionalClaims": {"@odata.type": "microsoft.graph.optionalClaims"},
  "parentalControlSettings": {"@odata.type": "microsoft.graph.parentalControlSettings"},
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "tokenEncryptionKeyId": "String",
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
  "suppressions": []
}
-->
