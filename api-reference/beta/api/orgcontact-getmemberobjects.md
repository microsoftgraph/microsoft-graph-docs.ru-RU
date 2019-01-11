---
title: 'orgContact: getMemberObjects'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
ms.openlocfilehash: ac6c8fddf4cedae156ec25933ea8d9f95bf8020a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856576"
---
# <a name="orgcontact-getmemberobjects"></a><span data-ttu-id="a9ad6-104">orgContact: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a9ad6-104">orgContact: getMemberObjects</span></span>

> <span data-ttu-id="a9ad6-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9ad6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9ad6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a9ad6-107">Permissions</span></span>
<span data-ttu-id="a9ad6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9ad6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9ad6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9ad6-110">Permission type</span></span>      | <span data-ttu-id="a9ad6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9ad6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9ad6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9ad6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a9ad6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a9ad6-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a9ad6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9ad6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9ad6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-115">Not supported.</span></span>    |
|<span data-ttu-id="a9ad6-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9ad6-116">Application</span></span> | <span data-ttu-id="a9ad6-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9ad6-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a9ad6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9ad6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="a9ad6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9ad6-119">Request headers</span></span>
| <span data-ttu-id="a9ad6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a9ad6-120">Name</span></span>       | <span data-ttu-id="a9ad6-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a9ad6-121">Type</span></span> | <span data-ttu-id="a9ad6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a9ad6-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a9ad6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9ad6-123">Authorization</span></span>  | <span data-ttu-id="a9ad6-124">string</span><span class="sxs-lookup"><span data-stu-id="a9ad6-124">string</span></span>  | <span data-ttu-id="a9ad6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a9ad6-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a9ad6-127">Request body</span></span>
<span data-ttu-id="a9ad6-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a9ad6-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="a9ad6-129">Parameter</span></span>    | <span data-ttu-id="a9ad6-130">Тип</span><span class="sxs-lookup"><span data-stu-id="a9ad6-130">Type</span></span>   |<span data-ttu-id="a9ad6-131">Описание</span><span class="sxs-lookup"><span data-stu-id="a9ad6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9ad6-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a9ad6-132">securityEnabledOnly</span></span>|<span data-ttu-id="a9ad6-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9ad6-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="a9ad6-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a9ad6-134">Response</span></span>

<span data-ttu-id="a9ad6-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9ad6-136">Пример</span><span class="sxs-lookup"><span data-stu-id="a9ad6-136">Example</span></span>
<span data-ttu-id="a9ad6-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a9ad6-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9ad6-138">Request</span></span>
<span data-ttu-id="a9ad6-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="a9ad6-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9ad6-140">Response</span></span>
<span data-ttu-id="a9ad6-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a9ad6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
