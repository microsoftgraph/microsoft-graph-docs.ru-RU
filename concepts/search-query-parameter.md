---
title: Использование параметра запроса $search в Microsoft Graph
description: Microsoft Graph поддерживает параметр запроса OData $search для ограничения результатов запроса с помощью условия поиска.
author: mumbi-o
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 3456985a8d8af1971cdda67a06c24e77e61efd4b
ms.sourcegitcommit: 3e2239e60b6dc53997b7d4356a20fc3d365d6238
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/02/2021
ms.locfileid: "61266084"
---
# <a name="use-the-search-query-parameter-to-match-a-search-criterion"></a>Использование параметра поискового запроса для сопоставления с условием поиска

В дополнение к [другим параметрам запросов OData](/graph/query-parameters) Microsoft Graph поддерживает параметр запроса `$search` для ограничения результатов запроса с помощью условия поиска.

Поддержка параметра запроса `$search` зависит от сущности. Некоторые из них, например ресурсы Azure AD, которые являются производными от [directoryObject](/graph/api/resources/directoryobject), поддерживают `$search` только в [расширенных запросах](/graph/aad-advanced-queries).

> [!NOTE]
> В настоящее время параметр запроса `$search` недоступен в клиентах Azure AD B2C.

## <a name="using-search-on-message-collections"></a>Использование параметра $search в коллекциях message

Можно искать сообщения, основываясь на их конкретных свойствах. Результаты поиска сортируются по дате и времени отправки сообщения. Запрос `$search` возвращает до 1000 результатов.

Если при поиске сообщений указано только значение, а конкретные свойства не заданы, поиск выполняется по свойствам поиска по умолчанию: **from**, **subject** и **body**.

Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово "pizza" в любом из трех свойств поиска по умолчанию:

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

Кроме того, для поиска сообщений можно указать в таблице ниже их имена свойств, распознаваемые синтаксисом языка запросов по ключевым словам (KQL). Эти имена свойств соответствуют свойствам, определенным в сущности **message** в Microsoft Graph. Синтаксис KQL поддерживается в Outlook и других приложениях Microsoft 365, например SharePoint. Благодаря этому возможно использование общего домена обнаружения для соответствующих хранилищ данных.


| Свойство электронных писем, по которому можно выполнять поиск                | Описание | Пример 
|:-------------------------|:------------|:---------|
| **attachment**           | Имена файлов, вложенных в сообщение электронной почты.|[GET][search-att-example] `../me/messages?$search="attachment:api-catalog.md"`
| **bcc**           | Поле **Скрытая копия** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.|[GET][search-bcc-example] `../me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`
| **body**           | Текст сообщения электронной почты.|[GET][search-body-example] `../me/messages?$search="body:excitement"`
| **cc**           | Поле **Копия** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.|[GET][search-cc-example] `../me/messages?$search="cc:danas"&$select=subject,ccRecipients`
| **from**           | Отправитель сообщения электронной почты, на которого указывает SMTP-адрес, отображаемое имя или псевдоним.| [GET][search-from-example] `../me/messages?$search="from:randiw"&$select=subject,from`
| **hasAttachment** | Значение TRUE означает, что сообщение электронной почты содержит вложение, не являющееся встроенным. В противном случае задается значение FALSE. | [GET][search-from-example] `../me/messages?$search="hasAttachments:true"`
| **importance**           | Важность сообщения, которую отправитель может указать при отправке. Возможные значения — `low`, `medium` и `high`.|[GET][search-imp-example] `../me/messages?$search="importance:high"&$select=subject,importance`
| **kind**           | Тип сообщения. Допустимые значения — `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` и `voicemail`.| [GET][search-kind-example] `../me/messages?$search="kind:voicemail"`
| **participants**           | Такие поля сообщения электронной почты, как **От**, **Кому**, **Копия** и **Скрытая копия**, где указан SMTP-адрес, отображаемое имя или псевдоним.| [GET][search-part-example] `../me/messages?$search="participants:danas"`
| **received**           | Дата получения сообщения адресатом.| [GET][search-rcvd-example] `../me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`
| **recipients**           | Такие поля сообщения электронной почты, как **Кому**, **Копия** и **Скрытая копия**, где указан SMTP-адрес, отображаемое имя или псевдоним.| [GET][search-rcpts-example] `../me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`
| **sent**           | Дата отправки сообщения отправителем.|[GET][search-sent-example] `../me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`
| **size**           | Размер элемента в байтах.|[GET][search-size-example] `../me/messages?$search="size:1..500000"`
| **subject**           | Текст в строке темы сообщения электронной почты.|[GET][search-sbj-example] `../me/messages?$search="subject:has"&$select=subject`
| **to**           | Поле **Кому** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.|[GET][search-to-example]`.../me/messages?$search="to:randiw"&$select=subject,toRecipients`


Дополнительные сведения о доступных для поиска свойствах, синтаксисе KQL, поддерживаемых операторах и подсказках для поиска вы найдете в таких статьях:

- [Свойства, доступные для поиска в Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)

- [Руководство по синтаксису языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- [Свойства сообщений и операторы поиска для обнаружения электронных данных на месте в Exchange 2016](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators).

## <a name="using-search-on-person-collections"></a>Использование параметра $search в коллекциях person

[API People](/graph/api/resources/person) Microsoft Graph можно использовать для получения сведений о наиболее релевантных для пользователя людях. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. API People поддерживает параметр запроса `$search`. Запрос `$search` возвращает до 250 результатов.

Поиск людей выполняется по свойствам **displayName** и **emailAddress** ресурса [person](/graph/api/resources/person).

По приведенному ниже запросу выполняется поиск человека с именем Irene McGowen в свойствах **displayName** и **emailAddress** всех людей из коллекции **people** вошедшего пользователя. Так как человек с именем Irene McGowan является релевантным для вошедшего пользователя, возвращается информация о нем.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

Ниже показан пример ответа. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

Дополнительные сведения об API People см. в [этой статье](./people-example.md#search-people).  

## <a name="using-search-on-directory-object-collections"></a>Использование $search в коллекциях объектов каталога

Ресурсы Azure AD и их связи, которые являются производными от [directoryObject](/graph/api/resources/directoryobject), поддерживают параметр запроса `$search` только в расширенных запросах. Реализация поиска **не** поддерживает `contains`. Вместо этого используется метод разметки, который извлекает слова из значения свойства и строки поиска с использованием пробелов, чисел, разного регистра и символов, как показано в следующих примерах.

* **Пробелы**: `hello world` => `hello`, `world`
* **Разный регистр**⁽¹⁾: `HelloWorld` или `helloWORLD` => `hello`, `world`
* **Символы**⁽²⁾: `hello.world` => `hello`, `.`, `world`, `helloworld`
* **Числа**: `hello123world` => `hello`, `123`, `world`

⁽¹⁾ В настоящее время разметка работает только в том случае, когда регистр изменяется с нижнего на верхний, поэтому `HELLOworld` считается одним маркером: `helloworld`, а `HelloWORld` — двумя маркерами: `hello`, `world`. ⁽²⁾ Логика разметки также объединяет слова, разделенные только символами, например поиск по запросу `helloworld` выдаст результаты `hello-world` и `hello.world`.

> **Примечание**. После разметки маркеры сопоставляются независимо от исходного регистра, и они сопоставляются в любом порядке. Например, displayName `李四(David Li)` будет соответствовать строкам поиска, таким как `李四(David Li)`, `李四`, `David`, `Li`, `David)`, `(李四`, `Li 李`.

Поддержка поиска с разметкой работает только в полях **displayName** и **description**. Любое поле строкового типа можно поместить в `$search`; поля, отличные от **displayName** и **description**, по умолчанию представляют поведение `$filter` `startswith`. Например:

`https://graph.microsoft.com/v1.0/groups/?$search="displayName:OneVideo"`

В результате будут выводиться все группы с именами типа "OneVideo". `$search` можно использовать вместе с `$filter`. Пример:

`https://graph.microsoft.com/v1.0/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

В результате будут выводиться все группы с включенной поддержкой почты с именами типа "OneVideo". Результаты ограничены на основе логического соединения `$filter` ("И") и всего запроса в `$search`. Искомый текст маркируется с учетом регистра, но совпадения выполняются без его учета. Например, "OneVideo" разбивается на два маркера ввода "one" и "video", но не учитывает регистр.

В синтаксисе поиска применяются следующие правила:

* Универсальный формат: $search="clause1" \[И \| ИЛИ\] "\[clauseX\]"\.
* Поддерживается любое количество предложений. Также поддерживаются круглые скобки для приоритета.
* Синтаксис каждого предложения — "\<property>:\<text to search>".
* Имя свойства должно быть указано в предложении. Любое свойство, которое можно использовать в `$filter`, можно также использовать в `$search`. В зависимости от свойства поведение поиска является либо "search", либо "startswith", если поиск не поддерживается в свойстве.
* Вся часть предложения должна быть заключена в двойные кавычки.
* Логический оператор "И" "ИЛИ" не должен быть в двойных кавычках. Они должны быть прописными.
* Учитывая, что вся часть предложения должна быть помещена в двойные кавычки, если она содержит двойные кавычки и обратную косую черту, ее необходимо экранировать с помощью обратной косой черты. Другие символы не требуется экранировать.

В таблице ниже приведено несколько примеров.

| Класс объекта | Описание | Пример |
| ------------ | ----------- | ------- |
| Пользователь | Отображаемое имя пользователя из адресной книги. | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr"`  |
| Пользователь | Отображаемое имя пользователя или электронная почта из адресной книги. | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$search="displayName:Guthr" OR "mail:Guthr"` |
| Группа | Отображаемое имя пользователя или описание из адресной книги. | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive"` |
| Группа | Отображаемое имя адресной книги в группе с поддержкой почты. | 
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"` |


Строки ввода, указанные в `$search`, а также свойства для поиска, разделяются на части с помощью пробелов, различных регистров и типов символов (чисел и специальных символов).

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.0
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

## <a name="see-also"></a>См. также

- [Настройка откликов с помощью параметров запроса](/graph/query-parameters)
- [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries)
- [Ограничения параметров запроса](known-issues.md#query-parameter-limitations)
