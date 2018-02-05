# <a name="use-the-people-api-in-microsoft-graph-to-get-information-about-the-people-most-relevant-to-you"></a><span data-ttu-id="edf0c-101">Использование API People в Microsoft Graph для получения сведений о наиболее релевантных для вас людях</span><span class="sxs-lookup"><span data-stu-id="edf0c-101">Use the People API in Microsoft Graph to get information about the people most relevant to you</span></span>
<span data-ttu-id="edf0c-p101">Приложения Microsoft Graph могут использовать API People для получения сведений о наиболее релевантных для пользователя людях. Релевантность определяется шаблонами общения и совместной работы пользователя, а также его бизнес-отношениями. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype). Наряду с функцией создания таких сведений в API People поддерживается поиск с нечетким соответствием, а также возможность получать список пользователей, релевантных для другого пользователя, в организации пользователя, выполнившего вход в систему. Особенно удобно использовать API People в сценариях выбора людей при написании электронных писем, создании собраний и т. д. Например, вы можете использовать API People в сценариях написания электронных писем.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p101">Microsoft Graph applications can use the People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. People can be local contacts, contacts from social networking or from an organization’s directory, and people from recent communications (such as email and Skype). Along with generating this insight, the People API also provides fuzzy matching search support and the ability to retrieve the list of users relevant to another user in the signed-in user's organization. The People API is particularly useful for people picking scenarios, such as composing an email or creating a meeting. For example, you can use the People API in email compose scenarios.</span></span>
 
## <a name="authorization"></a><span data-ttu-id="edf0c-108">Authorization</span><span class="sxs-lookup"><span data-stu-id="edf0c-108">Authorization</span></span>
<span data-ttu-id="edf0c-109">Чтобы ваше приложение в Microsoft Graph могло вызывать API People, ему потребуются указанные ниже разрешения.</span><span class="sxs-lookup"><span data-stu-id="edf0c-109">To call the People API in Microsoft Graph, your app will need the appropriate permissions:</span></span> 

* <span data-ttu-id="edf0c-p102">Разрешение People.Read используется для совершения общих вызовов к API People. Пример: https://graph.microsoft.com/v1.0/me/people/. Для использования разрешения People.Read требуется согласие пользователя.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p102">People.Read - Use to make general People API calls; for example, https://graph.microsoft.com/v1.0/me/people/. People.Read requires end user consent.</span></span>
* <span data-ttu-id="edf0c-p103">Разрешение People.Read.All необходимо для получения людей, наиболее релевантных для указанного пользователя, в вызовах организации пользователя, выполнившего вход в систему (https://graph.microsoft.com/v1.0/users('{id}')/people). Для использования разрешения People.Read.All требуется согласие администратора.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p103">People.Read.All - Required to retrieve the people most relevant to a specified user in the signed-in user’s organization (https://graph.microsoft.com/v1.0/users('{id}')/people) calls. People.Read.All requires admin consent.</span></span>
## <a name="browse-people"></a><span data-ttu-id="edf0c-114">Просмотр людей</span><span class="sxs-lookup"><span data-stu-id="edf0c-114">Browse people</span></span>
<span data-ttu-id="edf0c-p104">С помощью описанных в этом разделе запросов можно получить людей, наиболее релевантных для пользователя, выполнившего вход в систему (`/me`). Для выполнения этих запросов требуется разрешение People.Read. По умолчанию в каждом отклике возвращается 10 записей, но вы можете задать другое количество записей, используя параметр запроса *$top*.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p104">The requests in this section get the people most relevant to the signed-in user (`/me`). These requests require the People.Read permission. By default, each response returns 10 records, but you can change this by using the *$top* query parameter.</span></span> 
### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="edf0c-118">Получение коллекции релевантных людей</span><span class="sxs-lookup"><span data-stu-id="edf0c-118">Get a collection of relevant people</span></span> 
<span data-ttu-id="edf0c-119">С помощью указанного ниже запроса можно получить людей, наиболее релевантных для пользователя, выполнившего вход в систему (`/me`), на основании его шаблонов общения и совместной работы, а также бизнес-отношений.</span><span class="sxs-lookup"><span data-stu-id="edf0c-119">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="edf0c-p105">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра запроса *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p105">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "givenName": "Lorrie",
            "surname": "Frye",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Paralegal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "20/1109",
            "profession": "",
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 980 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "givenName": "Maynard",
            "surname": "Denman",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "givenName": "Darrel",
            "surname": "Halsey",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Attorney",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "14/1102",
            "profession": "",
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 205 555 0103"
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
### <a name="request-a-subsequent-page-of-people"></a><span data-ttu-id="edf0c-124">Запрос последующей страницы с людьми</span><span class="sxs-lookup"><span data-stu-id="edf0c-124">Request a subsequent page of people</span></span>
<span data-ttu-id="edf0c-p106">Если в первом отклике содержится неполный список релевантных людей, вы можете создать второй запрос, используя параметры *$top* и *$skip*, чтобы запросить дополнительные страницы информации. Если в предыдущем запросе есть дополнительная информация, то при последующем запросе будет получена следующая страница с людьми с сервера.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p106">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=3&$skip=10
```

<span data-ttu-id="edf0c-p107">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра запроса *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p107">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "1F28616D-BDFE-4080-8F06-03366A851688",
            "displayName": "Felix Coppola",
            "givenName": "Felix",
            "surname": "Coppola",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "CVP Legal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "19/2109",
            "profession": "",
            "userPrincipalName": "Felixc@contoso.onmicrosoft.com",
            "imAddress": "sip:Felixc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Felixc@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 309 555 0104"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "8A3FC021-6DBB-44AC-8884-B7B500CC260A",
            "displayName": "Lenora Rowland",
            "givenName": "Lenora",
            "surname": "Rowland",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Marketing Assistant",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "18/1106",
            "profession": "",
            "userPrincipalName": "Lenorar@contoso.onmicrosoft.com",
            "imAddress": "sip:Lenorar@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lenorar@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 954 555 0118"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "032C9919-4DF9-4715-8C46-4D0FAE7B3EB2",
            "displayName": "Manuel Collette",
            "givenName": "Manuel",
            "surname": "Collette",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Accountant II",
            "companyName": null,
            "yomiCompany": "",
            "department": "Finance",
            "officeLocation": "98/2202",
            "profession": "",
            "userPrincipalName": "Manuelc@contoso.onmicrosoft.com",
            "imAddress": "sip:Manuelc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Manuelc@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+20 255501070"
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
### <a name="sort-the-response"></a><span data-ttu-id="edf0c-131">Сортировка в отклике</span><span class="sxs-lookup"><span data-stu-id="edf0c-131">Sort the response</span></span> 
<span data-ttu-id="edf0c-p108">По умолчанию люди в отклике отсортированы по их релевантности вашему запросу. Вы можете изменить порядок людей в отклике, используя параметр *$orderby*. Этот запрос выбирает наиболее релевантных для вас людей, сортирует их по полю **displayName**, а затем возвращает первые 10 людей в отсортированном списке.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p108">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter. This query selects the people most relevant to you, sorts them by their **displayName**, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$orderby=displayName
```

<span data-ttu-id="edf0c-p109">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра *$top*. В примере ниже показано, как с помощью параметра *$top* уменьшить количество записей в отклике до трех штук.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p109">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. The following example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "818E29A1-E6BB-4EDA-AB20-8230B4B1E290",
            "displayName": "Adriana Ramos",
            "givenName": "Adriana",
            "surname": "Ramos",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Product Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "18/2111",
            "profession": "",
            "userPrincipalName": "Adrianar@contoso.onmicrosoft.com",
            "imAddress": "sip:Adrianar@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Adrianar@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 425 555 0109"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "62633BAA-1CB9-4FA2-9B8F-55AB1840B69D",
            "displayName": "Alyce Cooley",
            "givenName": "Alyce",
            "surname": "Cooley",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Marketing Assistant",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "131/1104",
            "profession": "",
            "userPrincipalName": "Alycec@contoso.onmicrosoft.com",
            "imAddress": "sip:Alycec@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Alycec@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 858 555 0110"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "6BB54D2C-EF20-48DA-ADD9-AE757DD30C4E",
            "displayName": "Alyssa Clarke",
            "givenName": "Alyssa",
            "surname": "Clarke",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Corporate Security Officer",
            "companyName": null,
            "yomiCompany": "",
            "department": "Operations",
            "officeLocation": "24/1106",
            "profession": "",
            "userPrincipalName": "Alyssac@contoso.onmicrosoft.com",
            "imAddress": "sip:Alyssac@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Alyssac@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 262 555 0106"
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
### <a name="change-the-number-of-people-and-fields-returned"></a><span data-ttu-id="edf0c-139">Изменение количества возвращаемых людей и полей</span><span class="sxs-lookup"><span data-stu-id="edf0c-139">Change the number of people and fields returned</span></span> 
<span data-ttu-id="edf0c-140">Вы можете изменить количество людей, возвращаемых в отклике, настроив параметр *$top*.</span><span class="sxs-lookup"><span data-stu-id="edf0c-140">You can change the number of people returned in the response by setting the *$top* parameter.</span></span> 

<span data-ttu-id="edf0c-p110">В примере ниже показано, как запросить 1000 людей, наиболее релевантных для пользователя `/me`. Кроме того, в запросе можно ограничить количество данных, отправляемых с сервера. Для этого запрашивается только параметр **displayName** человека.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p110">The following example requests the 1,000 people most relevant to `/me`. The request also limits the amount of data sent back from the server by requesting only the **displayName** of the person.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=1000&$Select=displayName
```

<span data-ttu-id="edf0c-143">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="edf0c-143">The following example shows the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye"
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman"
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey"
        },
        {
            "id": "E3C5B235-DE15-4566-B7B1-7A8E32426540",
            "displayName": "Roscoe Seidel"
        },
        {
            "id": "6BB54D2C-EF20-48DA-ADD9-AE757DD30C4E",
            "displayName": "Alyssa Clarke"
        },
        {
            "id": "818E29A1-E6BB-4EDA-AB20-8230B4B1E290",
            "displayName": "Adriana Ramos"
        },
        {
            "id": "62633BAA-1CB9-4FA2-9B8F-55AB1840B69D",
            "displayName": "Alyce Cooley"
        },
        {
            "id": "6BB9CC1F-418D-4DDF-AB0C-6A1C4ABCDBF4",
            "displayName": "Wayne Leeper"
        },
        {
            "id": "E7D40AC5-0078-4575-B1F3-F738124C4BC9",
            "displayName": "Jan Travis"
        },
        {
            "id": "6F99D1CC-4FCC-49E4-9160-E8AB01BF3E83",
            "displayName": "Charlotte Delacruz"
        },
        {
            "id": "1F28616D-BDFE-4080-8F06-03366A851688",
            "displayName": "Felix Coppola"
        },
        {
            "id": "8A3FC021-6DBB-44AC-8884-B7B500CC260A",
            "displayName": "Lenora Rowland"
        },
        {
            "id": "032C9919-4DF9-4715-8C46-4D0FAE7B3EB2",
            "displayName": "Manuel Collette"
        },
      ... etc
}
```
### <a name="select-the-fields-to-return"></a><span data-ttu-id="edf0c-144">Выбор возвращаемых полей</span><span class="sxs-lookup"><span data-stu-id="edf0c-144">Select the fields to return</span></span>
<span data-ttu-id="edf0c-p111">Вы можете ограничить объем данных, возвращаемых с сервера, выбрав одно или несколько полей с помощью параметра *$select*. Поле `@odata.id` возвращается всегда.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p111">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields. The `@odata.id` field is always returned.</span></span>

<span data-ttu-id="edf0c-147">В примере ниже показано, как ограничить перечень полей, возвращаемых в отклике, полями **displayName** и **scoredEmailAddresses** для 10 наиболее релевантных людей.</span><span class="sxs-lookup"><span data-stu-id="edf0c-147">The following example limits the response to the **displayName** and **scoredEmailAddresses** of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses
```

<span data-ttu-id="edf0c-p112">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p112">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
}
```
### <a name="use-a-filter-to-limit-the-response"></a><span data-ttu-id="edf0c-152">Использование фильтра для ограничения количества информации в отклике</span><span class="sxs-lookup"><span data-stu-id="edf0c-152">Use a filter to limit the response</span></span> 
<span data-ttu-id="edf0c-153">Вы можете использовать параметр *$filter*, чтобы ограничить количество информации в отклике и возвращать только тех людей, записи которых содержат указанные критерии.</span><span class="sxs-lookup"><span data-stu-id="edf0c-153">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span> 

<span data-ttu-id="edf0c-154">При выполнении указанного ниже запроса информация в отклике ограничивается экземплярами **person** со свойством **personType**, причем экземпляр **person** назначается как **класс**, а **organizationUser** — как **подкласс**.</span><span class="sxs-lookup"><span data-stu-id="edf0c-154">The following query limits the response to **person** instances with the **personType** property being assigned **person** as **class** and **organizationUser** as **subclass**.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$filter=personType/class eq 'Person' and personType/subclass eq 'OrganizationUser'
```

<span data-ttu-id="edf0c-p113">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p113">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "givenName": "Lorrie",
            "surname": "Frye",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Paralegal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "20/1109",
            "profession": "",
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 980 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "givenName": "Maynard",
            "surname": "Denman",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "givenName": "Darrel",
            "surname": "Halsey",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Attorney",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "14/1102",
            "profession": "",
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 205 555 0103"
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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="edf0c-159">Выбор полей, которые возвращаются в отфильтрованном отклике</span><span class="sxs-lookup"><span data-stu-id="edf0c-159">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="edf0c-160">Сочетая параметры *$select* и *$filter*, вы можете создать настраиваемый список людей, релевантных для пользователя, и получать только те поля, которые необходимы вашему приложению.</span><span class="sxs-lookup"><span data-stu-id="edf0c-160">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="edf0c-p114">В примере ниже показано, как получить значения полей **displayName** и **scoredEmailAddresses** для людей, чьи отображаемые имена совпадают с заданными. В этом примере показано, как возвратить людей c отображаемыми именами Lorrie Frye.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p114">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="edf0c-163">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="edf0c-163">The following example shows the response.</span></span> 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
}
```
## <a name="search-people"></a><span data-ttu-id="edf0c-164">Поиск людей</span><span class="sxs-lookup"><span data-stu-id="edf0c-164">Search people</span></span>
<span data-ttu-id="edf0c-p115">С помощью описанных в этом разделе запросов вы можете выполнить поиск людей, релевантных для пользователя, выполнившего вход в систему (`/me`), а также для других пользователей в организации пользователя, выполнившего вход в систему. Для выполнения таких запросов необходимо разрешение People.Read (за исключением случаев поиска людей, релевантных для другого пользователя, в которых требуется разрешение People.Read.All). По умолчанию в каждом отклике возвращается 10 записей, но вы можете задать другое количество записей с помощью параметра *$top*.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p115">The requests in this section allow you to search for people relevant to the signed-in user (`/me`) and other users in the signed-in user’s organization. These requests require the People.Read permission, with the exception of searching other users’ relevant people, which requires People.Read.All. By default, each response returns 10 records, but you can change this by using the *$top* parameter.</span></span> 
### <a name="use-search-to-select-people"></a><span data-ttu-id="edf0c-168">Использование поиска для выбора людей</span><span class="sxs-lookup"><span data-stu-id="edf0c-168">Use search to select people</span></span> 
<span data-ttu-id="edf0c-169">Используйте параметр *$search* для выбора людей, удовлетворяющих определенному набору критериев.</span><span class="sxs-lookup"><span data-stu-id="edf0c-169">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span> 

<span data-ttu-id="edf0c-170">Указанный ниже поисковый запрос возвращает релевантных для пользователя `/me` людей, чье свойство **displayName** или "emailAddress" содержит слово, начинающееся с буквы j.</span><span class="sxs-lookup"><span data-stu-id="edf0c-170">The following search query returns people relevant to `/me` whose **displayName** has a word that begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search=j
```

<span data-ttu-id="edf0c-p116">В примере ниже показан ответ. По умолчанию в каждом ответе возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в ответе.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p116">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "E3C5B235-DE15-4566-B7B1-7A8E32426540",
            "displayName": "Jan Travis",
            "givenName": "Jan",
            "surname": "Travis",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "VP Sales",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "19/3123",
            "profession": "",
            "userPrincipalName": "jant@contoso.onmicrosoft.com",
            "imAddress": "sip:jant@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "jant@contoso.onmicrosoft.com",
                    "relevanceScore": -12.297347783416837
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 732 555 0102"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "C43BF05E-5B6B-4DCF-B2FC-0837B09E0FA9",
            "displayName": "Jacob Cazares (TAILSPIN)",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "jacobc@tailspintoys.com",
                    "relevanceScore": -12.298154282019846
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "PersonalContact"
            }
        },
        {
            "id": "6BB9CC1F-418D-4DDF-AB0C-6A1C4ABCDBF4",
            "displayName": "Jewell Montgomery",
            "givenName": "Jewell",
            "surname": "Montgomery",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "jewellm@contoso.onmicrosoft.com",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "jewellm@contoso.onmicrosoft.com",
                    "relevanceScore": -12.531408487977451
                }
            ],
            "phones": [],
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
### <a name="perform-a-fuzzy-search"></a><span data-ttu-id="edf0c-175">Нечеткий поиск</span><span class="sxs-lookup"><span data-stu-id="edf0c-175">Perform a fuzzy search</span></span> 

<span data-ttu-id="edf0c-176">Для поиска используется алгоритм нечеткого соответствия.</span><span class="sxs-lookup"><span data-stu-id="edf0c-176">Searches implement a fuzzy matching algorithm.</span></span> <span data-ttu-id="edf0c-177">Возвращаются результаты, основанные на точном совпадении, а также на выводы, связанные с целью поиска.</span><span class="sxs-lookup"><span data-stu-id="edf0c-177">They will return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="edf0c-178">Предположим, в коллекции **people** вошедшего пользователя есть пользователь с отображаемым именем Tyler Lee и электронным адресом tylerle@example.com.</span><span class="sxs-lookup"><span data-stu-id="edf0c-178">For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="edf0c-179">Этот пользователь появится в результатах поиска по всем приведенным ниже запросам.</span><span class="sxs-lookup"><span data-stu-id="edf0c-179">All of the following searches will return this user Tyler as one of the results.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

<span data-ttu-id="edf0c-180">Вы также можете выполнять поиск релевантных для вошедшего пользователя людей, которые при общении с ним выразили интерес к определенным темам, например к пицце, как в следующем примере:</span><span class="sxs-lookup"><span data-stu-id="edf0c-180">You can also perform searches for people who are relevant to the signed-in user and have expressed an interest in communicating with that user over topics such as pizzas in the following example:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

<span data-ttu-id="edf0c-181">Темы в данном контексте — это просто слова, которые пользователи чаще всего использовали в своих сообщениях.</span><span class="sxs-lookup"><span data-stu-id="edf0c-181">Topics in this context are just words that have been used most by users in email conversations.</span></span> <span data-ttu-id="edf0c-182">Майкрософт извлекает и индексирует эти слова, чтобы искать по неточному соответствию было проще.</span><span class="sxs-lookup"><span data-stu-id="edf0c-182">Microsoft extracts such words and creates an index for this data to facilitate fuzzy searches.</span></span> 

<span data-ttu-id="edf0c-183">Обратите внимание, что поисковая фраза заключена в кавычки, а темы извлекаются без контекста.</span><span class="sxs-lookup"><span data-stu-id="edf0c-183">Note that the search phrase is enclosed in quotes, and topics in this data are extracted free of their contexts.</span></span> <span data-ttu-id="edf0c-184">Например, поиск слова "windows" в следующем запросе:</span><span class="sxs-lookup"><span data-stu-id="edf0c-184">As an example, searching for "windows" in the following query:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:windows" 
```
<span data-ttu-id="edf0c-185">— это нечеткий поиск по индексу тем, и результаты могут включать упоминания операционной системы Windows, отверстий в стене здания или другие определения.</span><span class="sxs-lookup"><span data-stu-id="edf0c-185">is a fuzzy search in the topic data index, and the results can include instances that mean the Windows operating system, an opening in a building wall, or other definitions.</span></span>

<span data-ttu-id="edf0c-186">И, наконец, в одном запросе можно объединить поиск людей и тем, используя вместе два вида выражений поиска.</span><span class="sxs-lookup"><span data-stu-id="edf0c-186">Finally, you can combine both people searches and topic searches in the same request by combining the two types of search expression.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```

<span data-ttu-id="edf0c-187">В этом запросе фактически выполняется два поиска: поиск нечетких соответствий по свойствам **displayName** и **emailAddress** в отношении людей, релевантных для вошедшего пользователя, и поиск по теме "pizza" в отношении этих людей.</span><span class="sxs-lookup"><span data-stu-id="edf0c-187">This request essentially conducts two searches: a fuzzy search against **displayName** and **emailAddress** properties of the signed-in user's relevant people, and a topic search for "pizza" against the user's relevant people.</span></span> <span data-ttu-id="edf0c-188">Результаты ранжируются, упорядочиваются и возвращаются.</span><span class="sxs-lookup"><span data-stu-id="edf0c-188">The results are then ranked, ordered, and returned.</span></span> <span data-ttu-id="edf0c-189">Обратите внимание, что поиск не имеет ограничений, поэтому результаты могут содержать список пользователей с нечетким соответствием имени "tyl" или пользователей, интересующихся темой "pizza", или и тех, и других.</span><span class="sxs-lookup"><span data-stu-id="edf0c-189">Note that the search is not restrictive; you might get results that contain people that fuzzy match "tyl", or that are interested in "pizza", or both.</span></span>

### <a name="search-other-users-relevant-people"></a><span data-ttu-id="edf0c-190">Поиск людей, релевантных для другого пользователя</span><span class="sxs-lookup"><span data-stu-id="edf0c-190">Search other user’s relevant people</span></span>
<span data-ttu-id="edf0c-p121">Указанный ниже запрос возвращает людей, наиболее релевантных для другого пользователя в организации пользователя, выполнившего вход в систему. Для выполнения этого запроса требуется разрешение People.Read.All. В этом примере отображаются люди, релевантные для пользователя Roscoe Seidel.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p121">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="edf0c-p122">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра *$top*. В примере ниже параметр запроса *$top* используется для ограничения количества записей в отклике до 3 шт.</span><span class="sxs-lookup"><span data-stu-id="edf0c-p122">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. The example below uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
     "value": [
        {
            "id": "56155636-703F-47F2-B657-C83F01F49BBC",
            "displayName": "Clifton Clemente",
            "givenName": "Clifton",
            "surname": "Clemente",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Director",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "19/2106",
            "profession": "",
            "userPrincipalName": "Cliftonc@contoso.onmicrosoft.com",
            "imAddress": "sip:Cliftonc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Cliftonc@contoso.onmicrosoft.com",
                    "relevanceScore": 20
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 309 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "6BF27D5A-AB4F-4C43-BED0-7DAD9EB0C1C4",
            "displayName": "Sheree Mitchell",
            "givenName": "Sheree",
            "surname": "Mitchell",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Product Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/2107",
            "profession": "",
            "userPrincipalName": "Shereem@contoso.onmicrosoft.com",
            "imAddress": "sip:shereem@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Shereem@contoso.onmicrosoft.com",
                    "relevanceScore": 10
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0107"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "B3E5302D-EAF0-4E8B-8C6C-A2AE64B4B163",
            "displayName": "Vincent Matney",
            "givenName": "Vincent",
            "surname": "Matney",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "CVP Engineering",
            "companyName": null,
            "yomiCompany": "",
            "department": "Engineering",
            "officeLocation": "23/2102",
            "profession": "",
            "userPrincipalName": "Vincentm@contoso.onmicrosoft.com",
            "imAddress": "sip:vincentm@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Vincentm@contoso.onmicrosoft.com",
                    "relevanceScore": 10
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 502 555 0102"
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