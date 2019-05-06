---
title: 'Пользователь: Експортперсоналдата'
description: Передает запрос операции политики данных, сделанный администратором компании для экспорта данных пользователя организации.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: adc6e35609b27a8353d24585b5542d3e9a704bd6
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33609595"
---
# <a name="user-exportpersonaldata"></a><span data-ttu-id="bd5b9-103">Пользователь: Експортперсоналдата</span><span class="sxs-lookup"><span data-stu-id="bd5b9-103">user: exportPersonalData</span></span>

<span data-ttu-id="bd5b9-104">Передает запрос операции политики данных, сделанный администратором компании для экспорта данных пользователя организации.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-104">Submits a data policy operation request, made by a company administrator to export an organizational user's data.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd5b9-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bd5b9-105">Permissions</span></span>
<span data-ttu-id="bd5b9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd5b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd5b9-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd5b9-108">Permission type</span></span>      | <span data-ttu-id="bd5b9-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd5b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd5b9-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd5b9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="bd5b9-111">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="bd5b9-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="bd5b9-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd5b9-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bd5b9-113">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="bd5b9-113">Not applicable</span></span>  |
|<span data-ttu-id="bd5b9-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bd5b9-114">Application</span></span> | <span data-ttu-id="bd5b9-115">User. Export. ALL и User. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="bd5b9-115">User.Export.All and User.Read.All</span></span> |

><span data-ttu-id="bd5b9-116">**Примечание:** Экспорт может выполняться только администратором компании при использовании делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-116">**Note:** Export can only be performed by a company administrator when the delegated permission is used.</span></span>

## <a name="http-request"></a><span data-ttu-id="bd5b9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd5b9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/exportPersonalData

```
## <a name="request-headers"></a><span data-ttu-id="bd5b9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bd5b9-118">Request headers</span></span>
| <span data-ttu-id="bd5b9-119">Имя</span><span class="sxs-lookup"><span data-stu-id="bd5b9-119">Name</span></span>       | <span data-ttu-id="bd5b9-120">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5b9-120">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bd5b9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd5b9-121">Authorization</span></span>  | <span data-ttu-id="bd5b9-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="bd5b9-122">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd5b9-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd5b9-123">Request body</span></span>
<span data-ttu-id="bd5b9-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bd5b9-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="bd5b9-125">Parameter</span></span>    | <span data-ttu-id="bd5b9-126">Тип</span><span class="sxs-lookup"><span data-stu-id="bd5b9-126">Type</span></span>   |<span data-ttu-id="bd5b9-127">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5b9-127">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bd5b9-128">Сторажелокатион</span><span class="sxs-lookup"><span data-stu-id="bd5b9-128">storageLocation</span></span>|<span data-ttu-id="bd5b9-129">String</span><span class="sxs-lookup"><span data-stu-id="bd5b9-129">String</span></span>|<span data-ttu-id="bd5b9-130">Это URL-адрес учетной записи службы хранилища Azure, в которую будут экспортироваться данные.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-130">This is a shared access signature (SAS) URL to an Azure Storage account, to where data should be exported.</span></span>|

## <a name="response"></a><span data-ttu-id="bd5b9-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd5b9-131">Response</span></span>
<span data-ttu-id="bd5b9-132">В случае успешного выполнения этот метод возвращает код отклика `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-132">If successful, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="bd5b9-133">В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-133">It does not return anything in the response body.</span></span> <span data-ttu-id="bd5b9-134">Ответ содержит следующие заголовки.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-134">The response contains the following headers.</span></span>

| <span data-ttu-id="bd5b9-135">Имя</span><span class="sxs-lookup"><span data-stu-id="bd5b9-135">Name</span></span>       | <span data-ttu-id="bd5b9-136">Описание</span><span class="sxs-lookup"><span data-stu-id="bd5b9-136">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="bd5b9-137">Расположение</span><span class="sxs-lookup"><span data-stu-id="bd5b9-137">Location</span></span>  | <span data-ttu-id="bd5b9-138">URL-адрес для проверки состояния запроса.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-138">URL to check on the status of the Request.</span></span> |
| <span data-ttu-id="bd5b9-139">Retry — после</span><span class="sxs-lookup"><span data-stu-id="bd5b9-139">Retry-After</span></span>  | <span data-ttu-id="bd5b9-140">Период времени в секундах.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-140">Time period in seconds.</span></span> <span data-ttu-id="bd5b9-141">Запрос должен подождать этого времени после отправки запроса на проверку состояния.</span><span class="sxs-lookup"><span data-stu-id="bd5b9-141">Request maker should wait this long after submitting a request to check for the status.</span></span> |


## <a name="example"></a><span data-ttu-id="bd5b9-142">Пример</span><span class="sxs-lookup"><span data-stu-id="bd5b9-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bd5b9-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd5b9-143">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="bd5b9-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd5b9-144">Response</span></span>

```
#### SDK sample code
# [C#](#tab/cs)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Cs-snippets.md)]

# [Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_exportpersonaldata-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
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
    "Error: /api-reference/beta/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-exportpersonaldata.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
