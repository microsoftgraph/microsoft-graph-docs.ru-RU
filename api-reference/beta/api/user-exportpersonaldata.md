---
title: 'Пользователь: Експортперсоналдата'
description: Передает запрос операции политики данных, сделанный администратором компании для экспорта данных пользователя организации.
localization_priority: Normal
author: krbain
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: afd5ba023d78fa969936915bb28187bb5fd17f1f
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2020
ms.locfileid: "43107880"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="b756a-103">Пользователь: Експортперсоналдата</span><span class="sxs-lookup"><span data-stu-id="b756a-103">user: exportPersonalData</span></span>

<span data-ttu-id="b756a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b756a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b756a-105">Отправка запроса операции политики данных, направленного администратором компании для экспорта данных пользователя организации.</span><span class="sxs-lookup"><span data-stu-id="b756a-105">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="b756a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b756a-106">Permissions</span></span>
<span data-ttu-id="b756a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b756a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b756a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b756a-109">Permission type</span></span>      | <span data-ttu-id="b756a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b756a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b756a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b756a-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="b756a-112">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b756a-112">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="b756a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b756a-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b756a-114">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="b756a-114">Not applicable</span></span>  |
|<span data-ttu-id="b756a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b756a-115">Application</span></span> | <span data-ttu-id="b756a-116">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="b756a-116">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="b756a-117">**Примечание:** Экспорт может выполняться только администратором компании при использовании делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="b756a-117">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="b756a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b756a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="b756a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b756a-119">Request headers</span></span>
| <span data-ttu-id="b756a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b756a-120">Name</span></span>       | <span data-ttu-id="b756a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b756a-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b756a-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b756a-122">Authorization</span></span>  | <span data-ttu-id="b756a-123">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b756a-123">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b756a-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b756a-124">Request body</span></span>
<span data-ttu-id="b756a-125">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b756a-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b756a-126">Параметр</span><span class="sxs-lookup"><span data-stu-id="b756a-126">Parameter</span></span>    | <span data-ttu-id="b756a-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b756a-127">Type</span></span>   |<span data-ttu-id="b756a-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b756a-128">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b756a-129">сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="b756a-129">storageLocation</span></span>|<span data-ttu-id="b756a-130">String</span><span class="sxs-lookup"><span data-stu-id="b756a-130">String</span></span>|<span data-ttu-id="b756a-131">Это URL-адрес учетной записи службы хранилища Azure, в которую будут экспортироваться данные.</span><span class="sxs-lookup"><span data-stu-id="b756a-131">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="b756a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="b756a-132">Response</span></span>
<span data-ttu-id="b756a-133">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="b756a-133">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="b756a-134">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b756a-134">It does not return anything in the response body.</span></span> <span data-ttu-id="b756a-135">Ответ содержит следующие заголовки.</span><span class="sxs-lookup"><span data-stu-id="b756a-135">The response contains the following headers.</span></span>

| <span data-ttu-id="b756a-136">Имя</span><span class="sxs-lookup"><span data-stu-id="b756a-136">Name</span></span>       | <span data-ttu-id="b756a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="b756a-137">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="b756a-138">Расположение</span><span class="sxs-lookup"><span data-stu-id="b756a-138">Location</span></span>  | <span data-ttu-id="b756a-139">URL-адрес для проверки состояния запроса.</span><span class="sxs-lookup"><span data-stu-id="b756a-139">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="b756a-140">Retry — после</span><span class="sxs-lookup"><span data-stu-id="b756a-140">Retry-After</span></span>  | <span data-ttu-id="b756a-141">Период времени в секундах.</span><span class="sxs-lookup"><span data-stu-id="b756a-141">Time period in seconds.</span></span> <span data-ttu-id="b756a-142">Запрос должен подождать этого времени после отправки запроса на проверку состояния.</span><span class="sxs-lookup"><span data-stu-id="b756a-142">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="b756a-143">Пример</span><span class="sxs-lookup"><span data-stu-id="b756a-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b756a-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="b756a-144">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b756a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="b756a-145">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b756a-146">C#</span><span class="sxs-lookup"><span data-stu-id="b756a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-exportpersonaldata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b756a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b756a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-exportpersonaldata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b756a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b756a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-exportpersonaldata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b756a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b756a-149">Response</span></span>

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
