---
title: Использование параметра запроса $search в Microsoft Graph
description: Microsoft Graph поддерживает параметр запроса OData $search для ограничения результатов запроса с помощью условия поиска.
author: mumbi-o
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: c552f510eb65370cd331784c98ea7359b278a56d
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53367012"
---
# <a name="use-the-search-query-parameter-to-match-a-search-criterion"></a><span data-ttu-id="4d1fb-103">Использование параметра поискового запроса для сопоставления с условием поиска</span><span class="sxs-lookup"><span data-stu-id="4d1fb-103">Use the search query parameter to match a search criterion</span></span>

<span data-ttu-id="4d1fb-104">В дополнение к [другим параметрам запросов OData](/graph/query-parameters) Microsoft Graph поддерживает параметр запроса `$search` для ограничения результатов запроса с помощью условия поиска.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-104">In addition to [other OData query parameters](/graph/query-parameters), Microsoft Graph supports the `$search` query parameter to restrict the results of a request to match a search criterion.</span></span>

<span data-ttu-id="4d1fb-105">Поддержка параметра запроса `$search` зависит от сущности. Некоторые из них, например ресурсы Azure AD, которые являются производными от [directoryObject](/graph/api/resources/directoryobject), поддерживают `$search` только в [расширенных запросах](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="4d1fb-105">The support for the `$search` query parameter varies by entity, with some, such as Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject), supporting `$search` only in [advanced queries](/graph/aad-advanced-queries).</span></span>

> [!NOTE]
> <span data-ttu-id="4d1fb-106">В настоящее время параметр запроса `$search` недоступен в клиентах Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-106">The `$search` query parameter is currently not available in Azure AD B2C tenants.</span></span>

## <a name="using-search-on-message-collections"></a><span data-ttu-id="4d1fb-107">Использование параметра $search в коллекциях message</span><span class="sxs-lookup"><span data-stu-id="4d1fb-107">Using $search on message collections</span></span>

<span data-ttu-id="4d1fb-108">Можно искать сообщения, основываясь на их конкретных свойствах.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-108">You can search messages based on a value in specific message properties.</span></span> <span data-ttu-id="4d1fb-109">Результаты поиска сортируются по дате и времени отправки сообщения.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-109">The results of the search are sorted by the date and time that the message was sent.</span></span> <span data-ttu-id="4d1fb-110">Запрос `$search` возвращает до 250 результатов.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-110">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="4d1fb-111">Если при поиске сообщений указано только значение, а конкретные свойства не заданы, поиск выполняется по свойствам поиска по умолчанию: **from**, **subject** и **body**.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-111">If you do a search on messages and specify only a value without specific message properties, the search is carried out on the default search properties of **from**, **subject**, and **body**.</span></span>

<span data-ttu-id="4d1fb-112">Следующий пример кода возвращает все сообщения из папки "Входящие" вошедшего пользователя, содержащие слово "pizza" в любом из трех свойств поиска по умолчанию:</span><span class="sxs-lookup"><span data-stu-id="4d1fb-112">The following example returns all messages in the signed-in user's Inbox that contains "pizza" in any of the three default search properties:</span></span>

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

<span data-ttu-id="4d1fb-113">Кроме того, для поиска сообщений можно указать в таблице ниже их имена свойств, распознаваемые синтаксисом языка запросов по ключевым словам (KQL).</span><span class="sxs-lookup"><span data-stu-id="4d1fb-113">Alternatively, you can search messages by specifying message property names in the following table, that are recognized by the Keyword Query Language (KQL) syntax.</span></span> <span data-ttu-id="4d1fb-114">Эти имена свойств соответствуют свойствам, определенным в сущности **message** в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-114">These property names correspond to properties defined in the **message** entity of Microsoft Graph.</span></span> <span data-ttu-id="4d1fb-115">Синтаксис KQL поддерживается в Outlook и других приложениях Microsoft 365, например SharePoint. Благодаря этому возможно использование общего домена обнаружения для соответствующих хранилищ данных.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-115">Outlook and other Microsoft 365 applications such as SharePoint support KQL syntax, providing the convenience of a common discovery domain for their data stores.</span></span>


| <span data-ttu-id="4d1fb-116">Свойство электронных писем, по которому можно выполнять поиск</span><span class="sxs-lookup"><span data-stu-id="4d1fb-116">Searchable email property</span></span>                | <span data-ttu-id="4d1fb-117">Описание</span><span class="sxs-lookup"><span data-stu-id="4d1fb-117">Description</span></span> | <span data-ttu-id="4d1fb-118">Пример</span><span class="sxs-lookup"><span data-stu-id="4d1fb-118">Example</span></span> 
|:-------------------------|:------------|:---------|
| <span data-ttu-id="4d1fb-119">**attachment**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-119">**attachment**</span></span>           | <span data-ttu-id="4d1fb-120">Имена файлов, вложенных в сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-120">The names of files attached to an email message.</span></span>|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| <span data-ttu-id="4d1fb-121">**bcc**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-121">**bcc**</span></span>           | <span data-ttu-id="4d1fb-122">Поле **Скрытая копия** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-122">The **bcc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| <span data-ttu-id="4d1fb-123">**body**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-123">**body**</span></span>           | <span data-ttu-id="4d1fb-124">Текст сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-124">The body of an email message.</span></span>|[`me/messages?$search="body:excitement"`][search-body-example]
| <span data-ttu-id="4d1fb-125">**cc**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-125">**cc**</span></span>           | <span data-ttu-id="4d1fb-126">Поле **Копия** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-126">The **cc** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| <span data-ttu-id="4d1fb-127">**from**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-127">**from**</span></span>           | <span data-ttu-id="4d1fb-128">Отправитель сообщения электронной почты, на которого указывает SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-128">The sender of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| <span data-ttu-id="4d1fb-129">**hasAttachment**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-129">**hasAttachment**</span></span> | <span data-ttu-id="4d1fb-130">Значение TRUE означает, что сообщение электронной почты содержит вложение, не являющееся встроенным. В противном случае задается значение FALSE.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-130">True if an email message contains an attachment that is not an inline attachment, false otherwise.</span></span> |[`me/messages?$search="hasAttachments:true"`][search-from-example]
| <span data-ttu-id="4d1fb-131">**importance**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-131">**importance**</span></span>           | <span data-ttu-id="4d1fb-132">Важность сообщения, которую отправитель может указать при отправке.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-132">The importance of an email message, which a sender can specify when sending a message.</span></span> <span data-ttu-id="4d1fb-133">Возможные значения — `low`, `medium` и `high`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-133">The possible values are `low`, `medium`, or `high`.</span></span>|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| <span data-ttu-id="4d1fb-134">**kind**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-134">**kind**</span></span>           | <span data-ttu-id="4d1fb-135">Тип сообщения.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-135">The type of message.</span></span> <span data-ttu-id="4d1fb-136">Допустимые значения — `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` и `voicemail`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-136">The possible values are `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks`, or `voicemail`.</span></span>|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| <span data-ttu-id="4d1fb-137">**participants**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-137">**participants**</span></span>           | <span data-ttu-id="4d1fb-138">Такие поля сообщения электронной почты, как **От**, **Кому**, **Копия** и **Скрытая копия**, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-138">The **from**, **to**, **cc**, and **bcc** fields of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="participants:danas"`][search-part-example]
| <span data-ttu-id="4d1fb-139">**received**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-139">**received**</span></span>           | <span data-ttu-id="4d1fb-140">Дата получения сообщения адресатом.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-140">The date that an email message was received by a recipient.</span></span>|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| <span data-ttu-id="4d1fb-141">**recipients**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-141">**recipients**</span></span>           | <span data-ttu-id="4d1fb-142">Такие поля сообщения электронной почты, как **Кому**, **Копия** и **Скрытая копия**, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-142">The **to**, **cc**, and **bcc** fields of an email meesage, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| <span data-ttu-id="4d1fb-143">**sent**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-143">**sent**</span></span>           | <span data-ttu-id="4d1fb-144">Дата отправки сообщения отправителем.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-144">The date that an email message was sent by the sender.</span></span>|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| <span data-ttu-id="4d1fb-145">**size**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-145">**size**</span></span>           | <span data-ttu-id="4d1fb-146">Размер элемента в байтах.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-146">The size of an item in bytes.</span></span>|[`me/messages?$search="size:1..500000"`][search-size-example]
| <span data-ttu-id="4d1fb-147">**subject**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-147">**subject**</span></span>           | <span data-ttu-id="4d1fb-p105">Текст в строке темы сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-p105">The text in the subject line of an email message. .</span></span>|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| <span data-ttu-id="4d1fb-150">**to**</span><span class="sxs-lookup"><span data-stu-id="4d1fb-150">**to**</span></span>           | <span data-ttu-id="4d1fb-151">Поле **Кому** в сообщении электронной почты, где указан SMTP-адрес, отображаемое имя или псевдоним.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-151">The **to** field of an email message, specified as an SMTP address, display name, or alias.</span></span>|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


<span data-ttu-id="4d1fb-152">Дополнительные сведения о доступных для поиска свойствах, синтаксисе KQL, поддерживаемых операторах и подсказках для поиска вы найдете в таких статьях:</span><span class="sxs-lookup"><span data-stu-id="4d1fb-152">For more information about searchable email properties, KQL syntax, supported operators, and tips on searching, see the following articles:</span></span>

- <span data-ttu-id="4d1fb-153">[Свойства, доступные для поиска в Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)</span><span class="sxs-lookup"><span data-stu-id="4d1fb-153">[Searchable properties in Exchange](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange).</span></span>

- [<span data-ttu-id="4d1fb-154">Руководство по синтаксису языка запросов по ключевым словам (KQL)</span><span class="sxs-lookup"><span data-stu-id="4d1fb-154">Keyword Query Language (KQL) syntax reference</span></span>](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- <span data-ttu-id="4d1fb-155">[Свойства сообщений и операторы поиска для обнаружения электронных данных на месте в Exchange 2016](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators).</span><span class="sxs-lookup"><span data-stu-id="4d1fb-155">[Message properties and search operators for In-Place eDiscovery in Exchange 2016](/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators)</span></span>

## <a name="using-search-on-person-collections"></a><span data-ttu-id="4d1fb-156">Использование параметра $search в коллекциях person</span><span class="sxs-lookup"><span data-stu-id="4d1fb-156">Using $search on person collections</span></span>

<span data-ttu-id="4d1fb-157">[API People](/graph/api/resources/person) Microsoft Graph можно использовать для получения сведений о наиболее релевантных для пользователя людях.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-157">You can use the Microsoft Graph [People API](/graph/api/resources/person) to retrieve the people who are most relevant to a user.</span></span> <span data-ttu-id="4d1fb-158">Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-158">Relevance is determined by the user’s communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="4d1fb-159">API People поддерживает параметр запроса `$search`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-159">The People API supports the `$search` query parameter.</span></span> <span data-ttu-id="4d1fb-160">Запрос `$search` возвращает до 250 результатов.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-160">A `$search` request returns up to 250 results.</span></span>

<span data-ttu-id="4d1fb-161">Поиск людей выполняется по свойствам **displayName** и **emailAddress** ресурса [person](/graph/api/resources/person).</span><span class="sxs-lookup"><span data-stu-id="4d1fb-161">Searches on people occur on both the **displayName** and **emailAddress** properties of the [person](/graph/api/resources/person) resource.</span></span>

<span data-ttu-id="4d1fb-162">По приведенному ниже запросу выполняется поиск человека с именем Irene McGowen в свойствах **displayName** и **emailAddress** всех людей из коллекции **people** вошедшего пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-162">The following request does a search for a person named "Irene McGowen" in the **displayName** and **emailAddress** properties in each person in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="4d1fb-163">Так как человек с именем Irene McGowan является релевантным для вошедшего пользователя, возвращается информация о нем.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-163">Because a person named "Irene McGowan" is relevant to the signed-in user, the information for "Irene McGowan" is returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

<span data-ttu-id="4d1fb-164">Ниже показан пример ответа.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-164">The following example shows the response.</span></span> 

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

<span data-ttu-id="4d1fb-165">Дополнительные сведения об API People см. в [этой статье](./people-example.md#search-people).</span><span class="sxs-lookup"><span data-stu-id="4d1fb-165">To learn more about the People API, see [Get information about relevant people](./people-example.md#search-people).</span></span>  

## <a name="using-search-on-directory-object-collections"></a><span data-ttu-id="4d1fb-166">Использование $search в коллекциях объектов каталога</span><span class="sxs-lookup"><span data-stu-id="4d1fb-166">Using $search on directory object collections</span></span>

<span data-ttu-id="4d1fb-167">Ресурсы Azure AD и их связи, которые являются производными от [directoryObject](/graph/api/resources/directoryobject), поддерживают параметр запроса `$search` только в расширенных запросах.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-167">Azure AD resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject) support the `$search` query parameter only in advanced queries.</span></span> <span data-ttu-id="4d1fb-168">Поиск использует разметку, которая выполняется путем извлечения слов из входной и выходной строки, использования пробелов, чисел, разного регистра и символов для разделения слов, как показано ниже.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-168">The search uses a tokenization approach which works by extracting words from your input and output string, using spaces, numbers, different casing, and symbols to separate the words, as follows:</span></span>

* <span data-ttu-id="4d1fb-169">**Пробелы**: `hello world` => `hello`, `world`</span><span class="sxs-lookup"><span data-stu-id="4d1fb-169">**Spaces**: `hello world` => `hello`, `world`</span></span>
* <span data-ttu-id="4d1fb-170">**Разный регистр**⁽¹⁾: `HelloWorld` или `helloWORLD` => `hello`, `world`</span><span class="sxs-lookup"><span data-stu-id="4d1fb-170">**Different casing**⁽¹⁾: `HelloWorld` or `helloWORLD` => `hello`, `world`</span></span>
* <span data-ttu-id="4d1fb-171">**Символы**⁽²⁾: `hello.world` => `hello`, `.`, `world`, `helloworld`</span><span class="sxs-lookup"><span data-stu-id="4d1fb-171">**Symbols**⁽²⁾: `hello.world` => `hello`, `.`, `world`, `helloworld`</span></span>
* <span data-ttu-id="4d1fb-172">**Числа**: `hello123world` => `hello`, `123`, `world`</span><span class="sxs-lookup"><span data-stu-id="4d1fb-172">**Numbers**: `hello123world` => `hello`, `123`, `world`</span></span>

<span data-ttu-id="4d1fb-173">⁽¹⁾ В настоящее время разметка работает только в том случае, когда регистр изменяется с нижнего на верхний, поэтому `HELLOworld` считается одним маркером: `helloworld`, а `HelloWORld` — двумя маркерами: `hello`, `world`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-173">⁽¹⁾ Currently, tokenization only works when the casing is changing from lowercase to uppercase, so `HELLOworld` is considered a single token: `helloworld`, and `HelloWORld` is two tokens: `hello`, `world`.</span></span> <span data-ttu-id="4d1fb-174">⁽²⁾ Логика разметки также объединяет слова, разделенные только символами, например поиск по запросу `helloworld` выдаст результаты `hello-world` и `hello.world`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-174">⁽²⁾ Tokenization logic also combines words that are separated only by symbols; for example, searching for `helloworld` will find `hello-world` and `hello.world`.</span></span>

> <span data-ttu-id="4d1fb-175">**Примечание**. После разметки маркеры сопоставляются независимо от исходного регистра, и они сопоставляются в любом порядке.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-175">**Note**: after tokenization, the tokens are matched independently of the original casing, and they are matched in any order.</span></span>

<span data-ttu-id="4d1fb-176">Поддержка поиска с разметкой работает только в полях **displayName** и **description**.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-176">The tokenized search support works only on the **displayName** and **description** fields.</span></span> <span data-ttu-id="4d1fb-177">Любое поле строкового типа можно поместить в `$search`, поля, отличные от **displayName** и **description** по умолчанию представляют собой поведение `$filter` `startswith`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-177">Any field of string type can be put in `$search`; fields other than **displayName** and **description** default to `$filter` `startswith` behavior.</span></span> <span data-ttu-id="4d1fb-178">Например:</span><span class="sxs-lookup"><span data-stu-id="4d1fb-178">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$search="displayName:OneVideo"`

<span data-ttu-id="4d1fb-179">В результате будут выводиться все группы с именами типа "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="4d1fb-179">This looks for all groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="4d1fb-180">`$search` можно использовать вместе с `$filter`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-180">`$search` can be used together with `$filter` as well.</span></span> <span data-ttu-id="4d1fb-181">Пример:</span><span class="sxs-lookup"><span data-stu-id="4d1fb-181">For example:</span></span>

`https://graph.microsoft.com/beta/groups/?$filter=mailEnabled eq true&$search="displayName:OneVideo"`

<span data-ttu-id="4d1fb-182">В результате будут выводиться все группы с включенной поддержкой почты с именами типа "OneVideo".</span><span class="sxs-lookup"><span data-stu-id="4d1fb-182">This looks for all mail-enabled groups with display names that look like "OneVideo".</span></span> <span data-ttu-id="4d1fb-183">Результаты ограничены на основе логического соединения `$filter` ("И") и всего запроса в `$search`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-183">The results are restricted based on a logical conjunction (an "AND") of the `$filter` and the entire query in the `$search`.</span></span> <span data-ttu-id="4d1fb-184">Искомый текст маркируется с учетом регистра, но совпадения выполняются без его учета.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-184">The search text is tokenized based on casing, but matches are performed in a case-insensitive manner.</span></span> <span data-ttu-id="4d1fb-185">Например, "OneVideo" разбивается на два маркера ввода "one" и "video", но не учитывает регистр.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-185">For example, "OneVideo" would be split into two input tokens "one" and "video", but matches properties insensitive to case.</span></span>

<span data-ttu-id="4d1fb-186">В синтаксисе поиска применяются следующие правила:</span><span class="sxs-lookup"><span data-stu-id="4d1fb-186">The syntax of search follows these rules:</span></span>

* <span data-ttu-id="4d1fb-187">Универсальный формат: $search="clause1" \[И \| ИЛИ\] "\[clauseX\]"\.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-187">Generic format: $search="clause1" \[AND \| OR\] "\[clauseX\]"\.</span></span>
* <span data-ttu-id="4d1fb-188">Поддерживается любое количество предложений.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-188">Any number of clauses is supported.</span></span> <span data-ttu-id="4d1fb-189">Также поддерживаются круглые скобки для приоритета.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-189">Parentheses for precedence is also supported.</span></span>
* <span data-ttu-id="4d1fb-190">Синтаксис каждого предложения — "\<property>:\<text to search>".</span><span class="sxs-lookup"><span data-stu-id="4d1fb-190">The syntax for each clause is: "\<property>:\<text to search>".</span></span>
* <span data-ttu-id="4d1fb-191">Имя свойства должно быть указано в предложении.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-191">The property name must be specified in the clause.</span></span> <span data-ttu-id="4d1fb-192">Любое свойство, которое можно использовать в `$filter`, можно также использовать в `$search`.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-192">Any property that can be used in `$filter` can also be used inside `$search`.</span></span> <span data-ttu-id="4d1fb-193">В зависимости от свойства поведение поиска является либо "search", либо "startswith", если поиск не поддерживается в свойстве.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-193">Depending on the property, the search behavior is either "search" or "startswith" if search is not supported on the property.</span></span>
* <span data-ttu-id="4d1fb-194">Вся часть предложения должна быть заключена в двойные кавычки.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-194">The whole clause part must be put inside double quotes.</span></span>
* <span data-ttu-id="4d1fb-195">Логический оператор "И" "ИЛИ" не должен быть в двойных кавычках.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-195">Logical operator 'AND' 'OR' must be put outside double quotes.</span></span> <span data-ttu-id="4d1fb-196">Они должны быть прописными.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-196">They must be in upper case.</span></span>
* <span data-ttu-id="4d1fb-p116">Учитывая, что вся часть предложения должна быть помещена в двойные кавычки, если она содержит двойные кавычки и обратную косую черту, ее необходимо экранировать с помощью обратной косой черты. Другие символы не требуется экранировать.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-p116">Given that the whole clause part needs to be put inside double quotes, if it contains double quote and backslash, it needs to be escaped with a backslash. No other characters need to be escaped.</span></span>

<span data-ttu-id="4d1fb-199">В таблице ниже приведено несколько примеров.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-199">The following table shows some examples.</span></span>

| <span data-ttu-id="4d1fb-200">Класс объекта</span><span class="sxs-lookup"><span data-stu-id="4d1fb-200">Object class</span></span> | <span data-ttu-id="4d1fb-201">Описание</span><span class="sxs-lookup"><span data-stu-id="4d1fb-201">Description</span></span> | <span data-ttu-id="4d1fb-202">Пример</span><span class="sxs-lookup"><span data-stu-id="4d1fb-202">Example</span></span> |
| ------------ | ----------- | ------- |
| <span data-ttu-id="4d1fb-203">Пользователь</span><span class="sxs-lookup"><span data-stu-id="4d1fb-203">User</span></span> | <span data-ttu-id="4d1fb-204">Отображаемое имя пользователя из адресной книги.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-204">Address book display name of the user.</span></span> | <span data-ttu-id="4d1fb-205">
  [
  https://graph.microsoft.com/beta/users?$search="displayName:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span><span class="sxs-lookup"><span data-stu-id="4d1fb-205">[https://graph.microsoft.com/beta/users?$search="displayName:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span></span> |
| <span data-ttu-id="4d1fb-206">Пользователь</span><span class="sxs-lookup"><span data-stu-id="4d1fb-206">User</span></span> | <span data-ttu-id="4d1fb-207">Отображаемое имя пользователя или электронная почта из адресной книги.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-207">Address book display name or mail of the user.</span></span> | <span data-ttu-id="4d1fb-208">
  [
  https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span><span class="sxs-lookup"><span data-stu-id="4d1fb-208">[https://graph.microsoft.com/beta/users?$search="displayName:Guthr" OR "mail:Guthr"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24search%3D%22displayName%3AGuthr%22%20OR%20%22mail%3AGuthr%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span></span> |
| <span data-ttu-id="4d1fb-209">Группа</span><span class="sxs-lookup"><span data-stu-id="4d1fb-209">Group</span></span> | <span data-ttu-id="4d1fb-210">Отображаемое имя пользователя или описание из адресной книги.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-210">Address book display name or description of the group.</span></span> | <span data-ttu-id="4d1fb-211">
  [
  https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span><span class="sxs-lookup"><span data-stu-id="4d1fb-211">[https://graph.microsoft.com/beta/groups?$search="description:One" AND ("displayName:Video" OR "displayName:Drive")](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24search%3D%22description%3AOne%22%20AND%20(%22displayName%3AVideo%22%20OR%20%22displayName%3ADrive%22)&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span></span> |
| <span data-ttu-id="4d1fb-212">Группа</span><span class="sxs-lookup"><span data-stu-id="4d1fb-212">Group</span></span> | <span data-ttu-id="4d1fb-213">Отображаемое имя адресной книги в группе с поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="4d1fb-213">Address book display name on a mail-enabled group.</span></span> | <span data-ttu-id="4d1fb-214">
  [
  https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span><span class="sxs-lookup"><span data-stu-id="4d1fb-214">[https://graph.microsoft.com/beta/groups?$filter=mailEnabled eq true&$search="displayName:OneVideo"](https://developer.microsoft.com/en-us/graph/graph-explorer?request=groups%3F%24filter%3DmailEnabled%20eq%20true%26%24search%3D%22displayName%3AOneVideo%22&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d)</span></span> |

<span data-ttu-id="4d1fb-215">Строки ввода, указанные в `$search`, а также свойства для поиска, разделяются на части с помощью пробелов, различных регистров и типов символов (чисел и специальных символов).</span><span class="sxs-lookup"><span data-stu-id="4d1fb-215">Both the string inputs you provide in `$search`, as well as the searchable properties, are split up into parts by spaces, different casing, and character types (numbers and special characters).</span></span>

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

## <a name="see-also"></a><span data-ttu-id="4d1fb-216">См. также</span><span class="sxs-lookup"><span data-stu-id="4d1fb-216">See also</span></span>

- [<span data-ttu-id="4d1fb-217">Настройка откликов с помощью параметров запроса</span><span class="sxs-lookup"><span data-stu-id="4d1fb-217">Use query parameters to customize responses</span></span>](/graph/query-parameters)
- [<span data-ttu-id="4d1fb-218">Расширенные возможности запросов для объектов каталога Azure AD</span><span class="sxs-lookup"><span data-stu-id="4d1fb-218">Advanced query capabilities on Azure AD directory objects</span></span>](/graph/aad-advanced-queries)
- [<span data-ttu-id="4d1fb-219">Ограничения параметров запроса</span><span class="sxs-lookup"><span data-stu-id="4d1fb-219">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)