---
title: Добавление пользовательских данных в ресурсы с помощью расширений
description: Вы можете расширить Microsoft Graph данными своего приложения. Добавляйте настраиваемые свойства в ресурсы Microsoft Graph без необходимости во внешнем хранилище данных.
author: dkershaw10
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: fca4c70795f06007b7d51bfaa2ccad6968fd9d16
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66554899"
---
# <a name="add-custom-properties-to-resources-using-extensions"></a>Добавляйте пользовательские свойства к ресурсам с помощью расширений

Microsoft Graph предоставляет единую конечную точку API для доступа к аналитическим данным и сведениям, ориентированным на людей, с помощью таких ресурсов, как [пользователь](/graph/api/resources/user) и [сообщение](/graph/api/resources/message). Вы также можете расширить Microsoft Graph, добавив настраиваемые свойства в экземпляры ресурсов без необходимости во внешнем хранилище данных.

В этой статье мы обсудим, как Microsoft Graph поддерживает расширение своих ресурсов, какие параметры доступны для добавления настраиваемых свойств и когда их использовать.

> [!IMPORTANT]
> Не используйте расширения для хранения конфиденциальных личных сведений, таких как учетные данные, государственные идентификационные номера, данные держателя карты, данные финансового счета, медицинские сведения или конфиденциальные справочные сведения.

## <a name="why-add-custom-properties-to-microsoft-graph"></a>Зачем добавлять настраиваемые свойства в Microsoft Graph?

> [!IMPORTANT]
> Вы не должны использовать расширения для хранения конфиденциальных личных сведений, таких как учетные данные, государственные идентификационные номера, данные держателя карты, данные финансового счета, медицинские сведения или конфиденциальные справочные сведения.
* Как независимый разработчик, вы можете решить сохранить легкость своего приложения и хранить данные профиля пользователя для конкретного приложения в Microsoft Graph, расширив ресурс **пользователя**.
* В качестве альтернативы вы можете сохранить существующее хранилище профилей пользователей вашего приложения и добавить идентификатор приложения к ресурсу **пользователя**.
* Как корпоративный разработчик, создавая внутренние приложения, вы можете полагаться на связанные с персоналом данные своей организации. Интеграцию с несколькими приложениями можно упростить, сохранив эти данные в настраиваемых свойствах Microsoft Graph.

## <a name="custom-property-options-in-microsoft-graph"></a>Параметры настраиваемых свойств в Microsoft Graph

Microsoft Graph предлагает четыре типа расширений для добавления настраиваемых свойств.

- Свойства атрибутов расширения
- Расширения каталога (Azure AD)
- Расширения схемы
- Открытые расширения

### <a name="extension-attributes"></a>Атрибуты расширения

Azure AD предлагает набор из 15 настраиваемых свойств с предопределенными именами для ресурсов [пользователя](/graph/api/resources/onpremisesextensionattributes) и [устройства](/graph/api/resources/onpremisesextensionattributes). Эти свойства изначально были настраиваемыми атрибутами, предоставляемыми в локальной среде Active Directory (AD) и Microsoft Exchange. Однако теперь их можно использовать не только для синхронизации локальных данных AD и Microsoft Exchange с Azure AD через Microsoft Graph.

#### <a name="developer-experience"></a>Среда разработки

Вы можете использовать 15 атрибутов расширения для хранения значений строки в экземплярах ресурсов **пользователя** или **устройства** через свойства **onPremisesExtensionAttributes** и **extensionAttributes** соответственно. Значения могут быть присвоены при создании нового экземпляра ресурса или при обновлении существующего экземпляра ресурса. Их также можно отфильтровать.

##### <a name="add-or-update-data-in-extension-attributes"></a>Добавление или обновление данных в атрибутах расширения

В следующем примере показано, как сохранить данные в **extensionAttribute1** и удалить существующие данные из **extensionAttribute12** с помощью операции обновления с помощью метода PATCH.

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/071cc716-8147-4397-a5ba-b2105951cc0b

{
    "onPremisesExtensionAttributes": {
        "extensionAttribute1": "skypeId.adeleVance",
        "extensionAttribute13": null
    }
}
```

Запрос возвращает объект отклика `204 No Content`.

##### <a name="retrieve-data-from-extension-attributes-1-15"></a>Получить данные из атрибутов расширения 1-15

###### <a name="request"></a>Запрос

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$select=id,displayName,onPremisesExtensionAttributes
```

###### <a name="response"></a>Отклик

```http
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,displayName,onPremisesExtensionAttributes)",
    "value": [
        {
            "id": "071cc716-8147-4397-a5ba-b2105951cc0b",
            "displayName": "Adele Vance",
            "onPremisesExtensionAttributes": {
                "extensionAttribute1": "Contractor",
                "extensionAttribute2": "50",
                "extensionAttribute3": null,
                "extensionAttribute4": "1478354",
                "extensionAttribute5": "10239390",
                "extensionAttribute6": null,
                "extensionAttribute7": null,
                "extensionAttribute8": null,
                "extensionAttribute9": null,
                "extensionAttribute10": "11",
                "extensionAttribute11": null,
                "extensionAttribute12": "/o=ExchangeLabs/ou=Exchange Administrative Group (FYDIBOHF47SPDLT)/cn=Recipients/cn=5ee781fc7egc7aa0b9394bddb44e7f04-Adele Vance",
                "extensionAttribute13": null,
                "extensionAttribute14": null,
                "extensionAttribute15": null
            }
        }
    ]
}
```

### <a name="directory-azure-ad-extensions"></a>Расширения каталога (Azure AD)

[Расширения каталогов](/graph/api/resources/extensionProperty) предоставляют разработчикам строго типизированные, обнаруживаемые и фильтруемые расширения для объектов каталогов.

Расширения каталога сначала регистрируются в приложении с помощью операции [Create extensionProperty](/graph/api/application-post-extensionproperty) и должны быть явно нацелены на определенные объекты каталога. После одобрения приложения пользователем или администратором, свойства расширения становятся немедленно доступными в клиенте. Все авторизованные приложения в клиенте могут считывать и записывать данные о любых свойствах расширения, определенных для экземпляра целевого объекта каталога.

Список типов ресурсов, которые можно указать в качестве целевых объектов для расширения каталога, см. в разделе [Выбор типа расширения для своего приложения](#choose-an-extension-type-for-your-application).

#### <a name="developer-experience"></a>Среда разработки

Определения расширения каталога управляются с помощью ресурса [extensionProperty](/graph/api/resources/extensionproperty) и связанных с ним методов. Данные управляются с помощью тех же запросов REST, которые вы используете для управления экземпляром ресурса.

##### <a name="create-a-directory-extension-definition"></a>Создание определения расширения каталога

Прежде чем вы сможете добавить расширение каталога к экземпляру ресурса, необходимо создать определение расширения каталога.

###### <a name="request"></a>Запрос

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/applications/30a5435a-1871-485c-8c7b-65f69e287e7b/extensionProperties

{
    "name": "jobGroupTracker",
    "dataType": "String",
    "targetObjects": [
        "User"
    ]
}
```

###### <a name="response"></a>Отклик

Именованное свойство расширения каталога `extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker` создается с именем расширения, соответствующим следующему соглашению об именовании: *extension_{appId-без дефисов}_{extensionProperty-name}*.

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications('30a5435a-1871-485c-8c7b-65f69e287e7b')/extensionProperties/$entity",
    "id": "4e3dbc8f-ca32-41b4-825a-346215d7d20f",
    "deletedDateTime": null,
    "appDisplayName": "HR-sync-app",
    "dataType": "String",
    "isSyncedFromOnPremises": false,
    "name": "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker",
    "targetObjects": [
        "User"
    ]
}
```

##### <a name="add-a-directory-extension-property-to-a-target-object"></a>Добавление свойства расширения каталога к целевому объекту

После создания определения расширения каталога вы можете добавить его к экземпляру целевого типа объекта. Вы можете хранить данные в свойстве расширения каталога при создании нового экземпляра целевого объекта или при обновлении существующего объекта. В следующем примере показано, как сохранить данные в свойстве расширения каталога при создании нового объекта пользователя.

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": false,
        "password": "xWwvJ]6NMw+bWH-d"
    },
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "JobGroupN"
}
```

Запрос возвращает код отклика `201 Created` и объект [пользователь](/graph/api/resources/user) в тексте отклика.

##### <a name="retrieve-a-directory-extension-property"></a>Получить свойство расширения каталога

В следующем примере показано, как свойства расширения каталога и связанные данные представлены в экземпляре ресурса. Свойство расширения будет возвращено по умолчанию через конечную точку `beta`, но только на `$select`через конечную точку `v1.0`.

##### <a name="request"></a>Запрос

```msgraph-interactive
GET https://graph.microsoft.com/beta/users?$select=id,displayName,extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker,extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable
```

##### <a name="response"></a>Отклик

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users(id,displayName,extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker,extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable)",
    "value": [
        {
            "id": "63384f56-42d2-4aa7-b1d6-b10c78f143a2",
            "displayName": "Adele Vance",
            "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "E4",
            "extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable": true
        }
    ]
}
```

##### <a name="update-or-delete-directory-extension-properties"></a>Обновление или удаление свойств расширения каталога

Чтобы обновить или удалить значение свойства расширения каталога для экземпляра ресурса, используйте метод PATCH. Чтобы удалить свойство расширения и связанное с ним значение из экземпляра ресурса, установите для него значение `null`.

Следующий запрос обновляет значение одного свойства расширения каталога и удаляет другое свойство расширения.

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/63384f56-42d2-4aa7-b1d6-b10c78f143a2

{
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable": null,
    "extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker": "E4"
}
```

Запрос возвращает код отклика `204 No Content`.

### <a name="schema-extensions"></a>Расширения схемы

[Расширения схемыMicrosoft Graph](/graph/api/resources/schemaextension) концептуально похожи на расширения каталогов. Вначале создайте определение расширения схемы, Затем используйте его для расширения поддерживаемых экземпляров ресурсов с помощью строго типизированных настраиваемых свойств. Кроме того, вы можете контролировать [состояние](/graph/api/resources/schemaextension#schema-extensions-lifecycle) расширения схемы и сделать его доступным другим приложениям.

Список типов ресурсов, которые поддерживают расширения схемы, см. в разделе [Выбор типа расширения для своего приложения](#choose-an-extension-type-for-your-application).

> [!VIDEO https://www.youtube-nocookie.com/embed/3MOAlUFNus0]

#### <a name="developer-experience"></a>Среда разработки

При создании определения расширения схемы необходимо присвоить уникальное имя его свойству **id**. Есть два варианта:

- Если у вас уже есть личный домен `.com`, `.net`, `.gov`, `.edu` или домен `.org`, который вы подтвердили в своем клиенте, вы можете использовать доменное имя вместе с именем схемы для определения уникального имени в следующем формате *{domainName}* _ *{schemaName}*. Например, если ваш личный домен — `contoso.com`, вы можете определить **идентификатор** для `contoso_mySchema`. Этот параметр настоятельно рекомендуется.
- Если у вас нет проверенного личного домена, вы можете установить **идентификатор** на имя схемы (без префикса имени домена). Например, `mySchema`. Microsoft Graph назначит вам строковый идентификатор на основе предоставленного имени в следующем формате: `ext{8-random-alphanumeric-chars}_{schema-name}`. Например, `extkvbmkofy_mySchema`.

**Идентификатор** будет именем сложного типа, который будет хранить ваши данные в экземпляре расширенного ресурса.

После регистрации расширения схемы оно доступно для использования всеми приложениями в том же арендаторе, что и связанное приложение-владелец (в состоянии `InDevelopment`), или всеми приложениями в любом клиенте (в состоянии `Available`). Как и расширения каталогов, авторизованные приложения могут считывать и записывать данные о любых расширениях, определенных для целевого объекта.

В отличие от открытых расширений вы управляете [определениями расширений схемы](/graph/api/resources/schemaextension) и их данными в экземпляре расширенного ресурса как отдельными наборами операций API. Для управления данными расширения схемы в экземпляре расширенного ресурса используйте тот же запрос REST, что и для управления экземпляром ресурса.

##### <a name="create-a-schema-extension-definition"></a>Создание определения расширения схемы

###### <a name="request"></a>Запрос

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/schemaExtensions

{
    "id": "graphLearnCourses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "user"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

###### <a name="response"></a>Отклик

```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#schemaExtensions/$entity",
    "id": "extkmpdyld2_graphLearnCourses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "user"
    ],
    "status": "InDevelopment",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="add-a-schema-extension-to-a-resource-instance"></a>Добавление расширения схемы к экземпляру ресурса

Теперь, после создания определения расширения схемы можно добавить свойство расширения к экземпляру целевого типа объекта. Вы можете хранить данные в расширении схемы при создании нового экземпляра целевого объекта или при обновлении существующего объекта. В следующем примере показано, как сохранить данные в свойстве расширения схемы при создании нового объекта пользователя.

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@m365x72712789.onmicrosoft.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": false,
        "password": "xWwvJ]6NMw+bWH-d"
    },
    "extkmpdyld2_graphLearnCourses": {
        "courseId": 100,
        "courseName": "Explore Microsoft Graph",
        "courseType": "Online"
    }
}
```

Запрос возвращает код отклика `201 Created` и объект [schemaExtension](/graph/api/resources/schemaextension) в тексте отклика.

##### <a name="update-or-delete-a-schema-extension-property"></a>Обновление или удаление свойства расширения схемы

Используйте операцию PATCH, чтобы обновить свойство расширения схемы или удалить существующий объект расширения схемы. Чтобы удалить свойство расширения и связанное с ним значение из экземпляра ресурса, установите для него значение `null`.

В следующем примере удаляется значение свойства **courseId** и обновляется свойство **courseType**. Чтобы полностью удалить свойство расширения `extkmpdyld2_graphLearnCourses`, установите для него значение `null`.

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/users/0668e673-908b-44ea-861d-0661297e1a3e

{
    "extkmpdyld2_graphLearnCourses": {
        "courseType": "Instructor-led",
        "courseId": null
    }
}
```

Запрос возвращает объект отклика `204 No Content`.

##### <a name="retrieve-the-schema-extension-property"></a>Получение свойства расширения схемы

Чтобы прочитать свойства расширения схемы в экземпляре ресурса, укажите имя расширения в запросе `$select`.

###### <a name="request"></a>Запрос
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/0668e673-908b-44ea-861d-0661297e1a3e?$select=id,displayName,extkmpdyld2_graphLearnCourses
```

###### <a name="response"></a>Отклик
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users(id,displayName,extkmpdyld2_graphLearnCourses)/$entity",
    "id": "63384f56-42d2-4aa7-b1d6-b10c78f143a2",
    "displayName": "Adele Vance",
    "extkmpdyld2_graphLearnCourses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseType": "Instructor-led",
        "courseName": "Explore Microsoft Graph",
        "courseId": null
    }
}
```

Дополнительные сведения о том, как использовать расширения схемы для добавления настраиваемых свойств и связанных данных, см. в разделах [Тип ресурса schemaExtension](/graph/api/resources/schemextension) и [Добавление настраиваемых свойств в группы с помощью расширений схемы](extensibility-schema-groups.md).

### <a name="open-extensions"></a>Открытые расширения

[Открытые расширения Microsoft Graph](/graph/api/resources/opentypeextension) — это [открытые типы](https://www.odata.org/getting-started/advanced-tutorial/#openType), которые предлагают простой и гибкий способ добавления нетипизированных данных непосредственно в экземпляр ресурса. Эти расширения не являются строго типизированными, недоступными для обнаружения или фильтрации.

Список типов ресурсов, поддерживающих открытые расширения Microsoft Graph, см. в разделе [Выбор типа расширения для вашего приложения](#choose-an-extension-type-for-your-application).

> [!VIDEO https://www.youtube-nocookie.com/embed/ibdlADb8IZc]

#### <a name="developer-experience"></a>Среда разработки

Открытые расширения вместе с их данными доступны через свойство навигации по **расширениям** экземпляра ресурса. Они позволяют группировать связанные свойства для облегчения доступа и управления.

Свойство **extensionName** — это единственное *предварительно определенное* записываемое свойство в открытом расширении. При создании открытого расширения нужно назначить свойству **extensionName** имя, которое уникально для клиента. Для этого можно использовать формат обратных DNS, который зависит от *принадлежащего вам домена*, например `Com.Contoso.ContactInfo`. **Не используйте домен Microsoft (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения**.

##### <a name="create-an-open-extension"></a>Создание открытого расширения

В следующем примере показано определение открытого расширения с тремя свойствами и то, как настраиваемые свойства и связанные данные представлены в экземпляре ресурса.

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.socialSettings",
    "skypeId": "skypeId.AdeleV",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile",
    "xboxGamerTag": "AwesomeAdele",
    "id": "com.contoso.socialSettings"
}
```

Запрос возвращает код ответа `201 Created` и объект [openTypeExtension](/graph/api/resources/opentypeextension) в тексте отклика.

##### <a name="update-an-existing-open-extension"></a>Обновление существующего открытого расширения

Чтобы обновить открытое расширение, необходимо указать все его свойства в тексте запроса. В противном случае неуказанные свойства будут обновлены до `null`и удалены из открытого расширения.

В следующем запросе указываются только свойства **linkedInProfile** и **xboxGamerTag**. Значение свойства **xboxGamerTag** обновляется, а свойство **linkedInProfile** остается прежним. Этот запрос также удаляет неуказанное свойство **skypeId**.

```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions/com.contoso.socialSettings

{
    "xboxGamerTag": "FierceAdele",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile"
}
```
Этот запрос возвращает код отклика `204 No Content`.


##### <a name="retrieve-the-open-extensions"></a>Извлечение открытых расширений

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users/3fbd929d-8c56-4462-851e-0eb9a7b3a2a5/extensions/com.contoso.socialSettings

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('3fbd929d-8c56-4462-851e-0eb9a7b3a2a5')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "xboxGamerTag": "FierceAdele",
    "linkedInProfile": "www.linkedin.com/in/testlinkedinprofile",
    "id": "com.contoso.socialSettings"
}
```

Дополнительные сведения о том, как использовать открытые расширения для добавления настраиваемых свойств и связанных данных, см. в разделах [Тип ресурса openTypeExtension](/graph/api/resources/opentypeextension) и [Добавление настраиваемых свойств пользователям с помощью открытых расширений](extensibility-open-users.md).

## <a name="choose-an-extension-type-for-your-application"></a>Выбор типа расширения для своего приложения

В приведенной ниже таблице сопоставляются и сравниваются типы расширений, что должно помочь вам решить, какой вариант больше подходит для вашего сценария.

| Возможность | Атрибуты расширения 1–15 | Расширения каталогов | Расширения схемы | Открытые расширения |
|--|--|--|--|--|
| Поддерживаемые типы ресурсов | [user][] <br/>[device][] | [user][] <br/> [group][] [administrativeUnit][] <br/> [application][] <br/>[device][] <br/> [organization][] | [user][] <br/> [group][] [administrativeUnit][] <br/> [contact][] <br/> [device][] <br/> [event][] (календари пользователей и групп) <br/> [message][] <br/> [organization][] <br/> [post][] <br/> [todoTask][] <br/> [todoTaskList][] | [user][] <br/> [group][] <!--<br/> [administrativeUnit][]--> <br/> [contact][] <br/> [device][] <br/> [event][]<sup>1</sup> (как пользовательский, так и групповой календари) <br/> [message][] <br/> [organization][] <br/> [post][] |
| Строго типизированный | Нет | Да | Да | Нет |
| Filterable | Да | Да | Да | Нет |
| Управляется через | Microsoft Graph <br/> Центр администрирования Exchange | Microsoft Graph | Microsoft Graph | Microsoft Graph |
| Синхронизация данных из локальной среды с расширениями с помощью [AD Connect][] | Да, для пользователей | [Да][ADConnect-YES] | Нет | Нет |
| Создание [правил динамического членства][] с использованием свойств и данных настраиваемых расширений. | [Да][DynamicMembership-YES] | [Да][DynamicMembership-YES] | Нет | Нет |
| Может использоваться для настройки требований токена | Да | [Да][DirectoryExt-CustomClaims] | Нет | Нет |
| Доступно в Azure AD B2C | Да | [Да][B2CDirectoryExt] | Да | Да |
| Ограничения | <li>15 предопределенных атрибутов для каждого пользователя или экземпляра ресурса устройства | <li>100 значений расширения на экземпляр ресурса | <li>Максимум пять определений на одного владельца приложения <br/><li> 100 значений расширения на экземпляр ресурса (только объекты каталога) | <li>Два открытых расширения на приложение-создатель на экземпляр ресурса<sup>2</sup> <br/><li> Максимальная 2Кб на открытое расширение<sup>2</sup><li> Для ресурсов Outlook каждое открытое расширение хранится в [именованном свойстве MAPI][MAPI-named-property]<sup>3</sup> |


> [!NOTE]
> 
> <sup>1</sup> Из-за существующего ограничения службы делегаты не могут создавать открытые события с добавлением расширения в календарях общих почтовых ящиков. Попытка сделать это приведет к ответу `ErrorAccessDenied`.
>
> <sup>2</sup> Эти ограничения на открытые расширения применяются к следующим ресурсам каталога: **пользователь**, **группа**, **устройство**, <!--**administrativeUnit**,--> и **организация**.
>
> <sup>3</sup> Каждое [открытое расширение](/graph/api/resources/opentypeextension) хранится в [именованном свойстве MAPI](/office/client-developer/outlook/mapi/mapi-named-properties), которое является ограниченным ресурсом в почтовом ящике пользователя. Это ограничение распространяется на следующие ресурсы Outlook: **сообщения**, **события** и **контакты**
>
> Вы можете управлять всеми расширениями, войдя в рабочую или учебную учетную запись. Кроме того, при входе с личной учетной записью Майкрософт вы можете управлять открытыми расширениями для следующих ресурсов: **событие**, **публикация**, **группа**, **сообщение**, **контакт** и **пользователь**.

## <a name="permissions"></a>Разрешения

Для чтения или записи данных для расширений в ресурсе необходимы те же [разрешения](./permissions-reference.md), что и для чтения или записи ресурса. Например, чтобы приложение могло обновить профиль любого пользователя с помощью настраиваемых данных приложения, приложению должно быть предоставлено разрешение *User.ReadWrite.All*.

## <a name="known-limitations"></a>Известные ограничения

Об известных ограничениях на использование расширений можно узнать в [соответствующем разделе](known-issues.md#extensions) статьи об известных проблемах.

## <a name="see-also"></a>См. также

- [Добавление настраиваемых свойств пользователям с помощью открытых расширений](extensibility-open-users.md)
- [Добавление настраиваемых свойств в группы с помощью расширений схемы](extensibility-schema-groups.md)
- [Домены Microsoft 365](/office365/servicedescriptions/office-365-platform-service-description/domains)
- [Добавление и проверка домена для клиента Microsoft 365](https://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)


<!-- Links -->

[user]: /graph/api/resources/user
[group]: /graph/api/resources/group
[contact]: /graph/api/resources/contact
[administrativeUnit]: /graph/api/resources/administrativeunit
[application]: /graph/api/resources/application
[device]: /graph/api/resources/device
[event]: /graph/api/resources/event
[message]: /graph/api/resources/message
[organization]: /graph/api/resources/organization
[post]: /graph/api/resources/post
[todoTask]: /graph/api/resources/todotask
[todoTaskList]: /graph/api/resources/todotasklist
[servicePrincipal]: /graph/api/resources/serviceprincipal
[AD connect]: /azure/active-directory/hybrid/whatis-hybrid-identity?context=/azure/active-directory/enterprise-users/context/ugr-context
[ADConnect-YES]: /azure/active-directory/hybrid/how-to-connect-sync-feature-directory-extensions
[правила динамического членства]: /azure/active-directory/enterprise-users/groups-dynamic-membership
[DynamicMembership-YES]: /azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties
[DirectoryExt-CustomClaims]: /azure/active-directory/develop/active-directory-optional-claims#configuring-directory-extension-optional-claims
[B2CDirectoryExt]: /azure/active-directory-b2c/user-profile-attributes#extension-attributes
[MAPI-named-property]: /office/client-developer/outlook/mapi/mapi-named-properties