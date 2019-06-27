---
title: 'Пользователь: Експортперсоналдата'
description: Передает запрос операции политики данных, сделанный администратором компании для экспорта данных пользователя организации.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 58b8d8900a7323b12c17de5bb083e4a181abe68e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270387"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="50851-103">Пользователь: Експортперсоналдата</span><span class="sxs-lookup"><span data-stu-id="50851-103">user: exportPersonalData</span></span>

<span data-ttu-id="50851-104">Передает запрос операции политики данных, сделанный администратором компании для экспорта данных пользователя организации.</span><span class="sxs-lookup"><span data-stu-id="50851-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="50851-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50851-105">Permissions</span></span>
<span data-ttu-id="50851-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50851-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50851-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50851-108">Permission type</span></span>      | <span data-ttu-id="50851-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50851-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50851-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50851-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="50851-111">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="50851-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="50851-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50851-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="50851-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="50851-113">Not applicable</span></span>  |
|<span data-ttu-id="50851-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50851-114">Application</span></span> | <span data-ttu-id="50851-115">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="50851-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="50851-116">**Примечание:** Экспорт может выполняться только администратором компании при использовании делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="50851-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="50851-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50851-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="50851-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50851-118">Request headers</span></span>
| <span data-ttu-id="50851-119">Имя</span><span class="sxs-lookup"><span data-stu-id="50851-119">Name</span></span>       | <span data-ttu-id="50851-120">Описание</span><span class="sxs-lookup"><span data-stu-id="50851-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="50851-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50851-121">Authorization</span></span>  | <span data-ttu-id="50851-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="50851-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="50851-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50851-123">Request body</span></span>
<span data-ttu-id="50851-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="50851-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="50851-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="50851-125">Parameter</span></span>    | <span data-ttu-id="50851-126">Тип</span><span class="sxs-lookup"><span data-stu-id="50851-126">Type</span></span>   |<span data-ttu-id="50851-127">Описание</span><span class="sxs-lookup"><span data-stu-id="50851-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="50851-128">Сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="50851-128">storageLocation</span></span>|<span data-ttu-id="50851-129">String</span><span class="sxs-lookup"><span data-stu-id="50851-129">String</span></span>|<span data-ttu-id="50851-130">Это URL-адрес учетной записи службы хранилища Azure, в которую будут экспортироваться данные.</span><span class="sxs-lookup"><span data-stu-id="50851-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="50851-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="50851-131">Response</span></span>
<span data-ttu-id="50851-132">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="50851-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="50851-133">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="50851-133">It does not return anything in the response body.</span></span> <span data-ttu-id="50851-134">Ответ содержит следующие заголовки.</span><span class="sxs-lookup"><span data-stu-id="50851-134">The response contains the following headers.</span></span>

| <span data-ttu-id="50851-135">Имя</span><span class="sxs-lookup"><span data-stu-id="50851-135">Name</span></span>       | <span data-ttu-id="50851-136">Описание</span><span class="sxs-lookup"><span data-stu-id="50851-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="50851-137">Расположение</span><span class="sxs-lookup"><span data-stu-id="50851-137">Location</span></span>  | <span data-ttu-id="50851-138">URL-адрес для проверки состояния запроса.</span><span class="sxs-lookup"><span data-stu-id="50851-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="50851-139">Retry — после</span><span class="sxs-lookup"><span data-stu-id="50851-139">Retry-After</span></span>  | <span data-ttu-id="50851-140">Период времени в секундах.</span><span class="sxs-lookup"><span data-stu-id="50851-140">Time period in seconds.</span></span> <span data-ttu-id="50851-141">Запрос должен подождать этого времени после отправки запроса на проверку состояния.</span><span class="sxs-lookup"><span data-stu-id="50851-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="50851-142">Пример</span><span class="sxs-lookup"><span data-stu-id="50851-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50851-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="50851-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/beta/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
##### <a name="response"></a><span data-ttu-id="50851-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="50851-144">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="50851-145">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="50851-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="50851-146">C#</span><span class="sxs-lookup"><span data-stu-id="50851-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50851-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="50851-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="50851-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="50851-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: exportPersonalData",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
