# <a name="list-apps-in-team"></a><span data-ttu-id="1356f-101">Список приложений в группы</span><span class="sxs-lookup"><span data-stu-id="1356f-101">List apps in team</span></span>



<span data-ttu-id="1356f-102">Извлечь список [приложений установлен](../resources/teamsappinstallation.md) в указанной [группы](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1356f-102">Retrieve the list of [apps installed](../resources/teamsappinstallation.md) in the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1356f-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1356f-103">Permissions</span></span>

<span data-ttu-id="1356f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1356f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1356f-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1356f-106">Permission type</span></span>      | <span data-ttu-id="1356f-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1356f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1356f-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1356f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1356f-109">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1356f-109">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1356f-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1356f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1356f-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1356f-111">Not supported.</span></span>    |
|<span data-ttu-id="1356f-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1356f-112">Application</span></span> | <span data-ttu-id="1356f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1356f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1356f-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1356f-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{id}/installedApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1356f-115">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="1356f-115">Optional query parameters</span></span>

<span data-ttu-id="1356f-116">Этот метод поддерживает $filter $select, и $разверните [Параметры запроса OData](../../../concepts/query_parameters.md) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="1356f-116">This method supports the $filter, $select, and $expand [OData Query Parameters](../../../concepts/query_parameters.md) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1356f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1356f-117">Request headers</span></span>

| <span data-ttu-id="1356f-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1356f-118">Header</span></span>       | <span data-ttu-id="1356f-119">Значение</span><span class="sxs-lookup"><span data-stu-id="1356f-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1356f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1356f-120">Authorization</span></span>  | <span data-ttu-id="1356f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1356f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1356f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1356f-123">Request body</span></span>

<span data-ttu-id="1356f-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1356f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1356f-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="1356f-125">Response</span></span>

<span data-ttu-id="1356f-126">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [teamsApp](../resources/teamsapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="1356f-126">If successful, this method returns a `200 OK` response code and collection of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1356f-127">Пример</span><span class="sxs-lookup"><span data-stu-id="1356f-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="1356f-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="1356f-128">Request</span></span>

<span data-ttu-id="1356f-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1356f-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps
```

### <a name="response"></a><span data-ttu-id="1356f-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1356f-130">Response</span></span>

<span data-ttu-id="1356f-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1356f-131">The following is an example of the response.</span></span>
><span data-ttu-id="1356f-132">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1356f-132">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1356f-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1356f-133">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

## <a name="example----getting-the-names-of-the-installed-apps"></a><span data-ttu-id="1356f-134">Пример — начало имен установленные приложения</span><span class="sxs-lookup"><span data-stu-id="1356f-134">Example -- getting the names of the installed apps</span></span>

### <a name="request"></a><span data-ttu-id="1356f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="1356f-135">Request</span></span>

<span data-ttu-id="1356f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1356f-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->

```http
GET https://graph.microsoft.com/beta/teams/{id}/installedApps?$expand=teamsAppDefinition
```

### <a name="response"></a><span data-ttu-id="1356f-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="1356f-137">Response</span></span>

<span data-ttu-id="1356f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="1356f-138">The following is an example of the response.</span></span>

><span data-ttu-id="1356f-139">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1356f-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1356f-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1356f-140">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
    "value": [
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZDgyMGVjZC1kZWYyLTQyOTctYWRhZC03ODA1NmNkZTdjNzg=",
            "teamsAppDefinition": {
                "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
                "teamsAppId": "0d820ecd-def2-4297-adad-78056cde7c78",
                "displayName": "OneNote",
                "version": "1.0.0"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMwZmQ5MjVhMC0zNTdmLTRkMjUtODQ1Ni1iMzAyMmFhYTQxYTk=",
            "teamsAppDefinition": {
                "id": "MGZkOTI1YTAtMzU3Zi00ZDI1LTg0NTYtYjMwMjJhYWE0MWE5IyMxLjc=",
                "teamsAppId": "0fd925a0-357f-4d25-8456-b3022aaa41a9",
                "displayName": "SurveyMonkey",
                "version": "1.7"
            }
        },
        {
            "id": "NjRiOWM3NDYtYjE1NS00MDQyLThkNDctOTQxYmQzODE2ODFiIyMyYTUyNzcwMy0xZjZmLTQ1NTktYTMzMi1kOGE3ZDI4OGNkODg=",
            "teamsAppDefinition": {
                "id": "MmE1Mjc3MDMtMWY2Zi00NTU5LWEzMzItZDhhN2QyODhjZDg4IyMxLjA=",
                "teamsAppId": "2a527703-1f6f-4559-a332-d8a7d288cd88",
                "displayName": "SharePoint",
                "version": "1.0"
            }
        }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->