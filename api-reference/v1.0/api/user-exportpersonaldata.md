---
title: 'Пользователь: Експортперсоналдата'
description: Передает запрос операции политики данных, сделанный администратором компании для экспорта данных пользователя организации.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9cdb8a19d229d308d0853223d23513daa51bec3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027155"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="69017-103">Пользователь: Експортперсоналдата</span><span class="sxs-lookup"><span data-stu-id="69017-103">user: exportPersonalData</span></span>

<span data-ttu-id="69017-104">Отправьте запрос операции политики данных от администратора организации или приложения для экспорта данных пользователя организации.</span><span class="sxs-lookup"><span data-stu-id="69017-104">Submit a data policy operation request from a company administrator or an application to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="69017-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69017-105">Permissions</span></span>
<span data-ttu-id="69017-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69017-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69017-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69017-108">Permission type</span></span>      | <span data-ttu-id="69017-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69017-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69017-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69017-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="69017-111">User. Export. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="69017-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="69017-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69017-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="69017-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="69017-113">Not applicable</span></span>  |
|<span data-ttu-id="69017-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69017-114">Application</span></span> | <span data-ttu-id="69017-115">User. Export. ALL, User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="69017-115">User.Export.All, User.Read.All</span></span> |

><span data-ttu-id="69017-116">**Примечание:** Экспорт может выполняться только администратором компании, когда используются делегированные разрешения.</span><span class="sxs-lookup"><span data-stu-id="69017-116">**Note:** The export can only be performed by a company administrator when delegated permissions are used.</span></span>

## <a name="http-request"></a><span data-ttu-id="69017-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69017-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="69017-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69017-118">Request headers</span></span>
| <span data-ttu-id="69017-119">Имя</span><span class="sxs-lookup"><span data-stu-id="69017-119">Name</span></span>       | <span data-ttu-id="69017-120">Описание</span><span class="sxs-lookup"><span data-stu-id="69017-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69017-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69017-121">Authorization</span></span>  | <span data-ttu-id="69017-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="69017-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="69017-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69017-123">Request body</span></span>
<span data-ttu-id="69017-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="69017-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="69017-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="69017-125">Parameter</span></span>    | <span data-ttu-id="69017-126">Тип</span><span class="sxs-lookup"><span data-stu-id="69017-126">Type</span></span>   |<span data-ttu-id="69017-127">Описание</span><span class="sxs-lookup"><span data-stu-id="69017-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69017-128">Сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="69017-128">storageLocation</span></span>|<span data-ttu-id="69017-129">String</span><span class="sxs-lookup"><span data-stu-id="69017-129">String</span></span>|<span data-ttu-id="69017-130">Это URL-адрес учетной записи службы хранилища Azure, в которую будут экспортироваться данные.</span><span class="sxs-lookup"><span data-stu-id="69017-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="69017-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="69017-131">Response</span></span>
<span data-ttu-id="69017-132">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="69017-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="69017-133">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="69017-133">It does not return anything in the response body.</span></span> <span data-ttu-id="69017-134">Ответ содержит следующие заголовки ответа.</span><span class="sxs-lookup"><span data-stu-id="69017-134">The response contains the following response headers.</span></span>

| <span data-ttu-id="69017-135">Имя</span><span class="sxs-lookup"><span data-stu-id="69017-135">Name</span></span>       | <span data-ttu-id="69017-136">Описание</span><span class="sxs-lookup"><span data-stu-id="69017-136">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="69017-137">Расположение</span><span class="sxs-lookup"><span data-stu-id="69017-137">Location</span></span>  | <span data-ttu-id="69017-138">URL-адрес для проверки состояния запроса.</span><span class="sxs-lookup"><span data-stu-id="69017-138">URL to check on the status of the request.</span></span> |
| <span data-ttu-id="69017-139">Retry — после</span><span class="sxs-lookup"><span data-stu-id="69017-139">Retry-After</span></span>  | <span data-ttu-id="69017-140">Период времени в секундах.</span><span class="sxs-lookup"><span data-stu-id="69017-140">Time period in seconds.</span></span> <span data-ttu-id="69017-141">Запрос должен подождать этого времени после отправки запроса на проверку состояния.</span><span class="sxs-lookup"><span data-stu-id="69017-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |

## <a name="example"></a><span data-ttu-id="69017-142">Пример</span><span class="sxs-lookup"><span data-stu-id="69017-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69017-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="69017-143">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="69017-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="69017-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_exportpersonaldata"
}-->
```http
POST https://graph.microsoft.com/v1.0/users/{id}/exportPersonalData
Content-type: application/json
Content-length: 48

{
  "storageLocation": "storageLocation-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="69017-145">C#</span><span class="sxs-lookup"><span data-stu-id="69017-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69017-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="69017-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69017-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="69017-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="69017-148">Java</span><span class="sxs-lookup"><span data-stu-id="69017-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-exportpersonaldata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="69017-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="69017-149">Response</span></span>

```http
{
  Location: https://graph.microsoft.com/v1.0/dataPolicyOperations/d007e3da-cd9b-4b02-8d66-422403c53e3f
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
