---
title: 'пользователь: exportPersonalData'
description: Представляет запрос на операцию политики данных, сделанный администратором компании для экспорта данных пользователя организации.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: bf03a21660a29172d1b55364bbb14d7770414f4a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721756"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="d3f4f-103">пользователь: exportPersonalData</span><span class="sxs-lookup"><span data-stu-id="d3f4f-103">user: exportPersonalData</span></span>

<span data-ttu-id="d3f4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3f4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d3f4f-105">Отправка запроса операции политики данных, направленного администратором компании для экспорта данных пользователя организации.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-105">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3f4f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3f4f-106">Permissions</span></span>
<span data-ttu-id="d3f4f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3f4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f4f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3f4f-109">Permission type</span></span>      | <span data-ttu-id="d3f4f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3f4f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3f4f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3f4f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="d3f4f-112">User.Export.All и User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3f4f-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="d3f4f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3f4f-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="d3f4f-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="d3f4f-114">Not applicable</span></span>  |
|<span data-ttu-id="d3f4f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3f4f-115">Application</span></span> | <span data-ttu-id="d3f4f-116">User.Export.All и User.Read.All</span><span class="sxs-lookup"><span data-stu-id="d3f4f-116">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="d3f4f-117">**Примечание:** Экспорт может выполняться администратором компании только при делегировании разрешения.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-117">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="d3f4f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3f4f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="d3f4f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3f4f-119">Request headers</span></span>
| <span data-ttu-id="d3f4f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="d3f4f-120">Name</span></span>       | <span data-ttu-id="d3f4f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d3f4f-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d3f4f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3f4f-122">Authorization</span></span>  | <span data-ttu-id="d3f4f-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="d3f4f-123">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3f4f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3f4f-124">Request body</span></span>
<span data-ttu-id="d3f4f-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d3f4f-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="d3f4f-126">Parameter</span></span>    | <span data-ttu-id="d3f4f-127">Тип</span><span class="sxs-lookup"><span data-stu-id="d3f4f-127">Type</span></span>   |<span data-ttu-id="d3f4f-128">Описание</span><span class="sxs-lookup"><span data-stu-id="d3f4f-128">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d3f4f-129">storageLocation</span><span class="sxs-lookup"><span data-stu-id="d3f4f-129">storageLocation</span></span>|<span data-ttu-id="d3f4f-130">String</span><span class="sxs-lookup"><span data-stu-id="d3f4f-130">String</span></span>|<span data-ttu-id="d3f4f-131">Это URL-адрес подписи общего доступа (SAS) к учетной записи Azure Storage, куда следует экспортировать данные.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-131">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="d3f4f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3f4f-132">Response</span></span>
<span data-ttu-id="d3f4f-133">При успешном выполнении этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-133">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="d3f4f-134">Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-134">It does not return anything in the response body.</span></span> <span data-ttu-id="d3f4f-135">Ответ содержит следующие заглавные.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-135">The response contains the following headers.</span></span>

| <span data-ttu-id="d3f4f-136">Имя</span><span class="sxs-lookup"><span data-stu-id="d3f4f-136">Name</span></span>       | <span data-ttu-id="d3f4f-137">Описание</span><span class="sxs-lookup"><span data-stu-id="d3f4f-137">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="d3f4f-138">Location</span><span class="sxs-lookup"><span data-stu-id="d3f4f-138">Location</span></span>  | <span data-ttu-id="d3f4f-139">URL-адрес для проверки состояния запроса.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-139">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="d3f4f-140">Retry-After</span><span class="sxs-lookup"><span data-stu-id="d3f4f-140">Retry-After</span></span>  | <span data-ttu-id="d3f4f-141">Период времени в секундах.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-141">Time period in seconds.</span></span> <span data-ttu-id="d3f4f-142">Производитель запросов должен ждать этого долго после отправки запроса для проверки состояния.</span><span class="sxs-lookup"><span data-stu-id="d3f4f-142">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="d3f4f-143">Пример</span><span class="sxs-lookup"><span data-stu-id="d3f4f-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3f4f-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3f4f-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d3f4f-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3f4f-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d3f4f-146">C#</span><span class="sxs-lookup"><span data-stu-id="d3f4f-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d3f4f-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3f4f-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3f4f-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3f4f-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d3f4f-149">Java</span><span class="sxs-lookup"><span data-stu-id="d3f4f-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-exportpersonaldata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3f4f-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3f4f-150">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/beta/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
  Retry-After: 60
}
```

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
  ]
}-->


