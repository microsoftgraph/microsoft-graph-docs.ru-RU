---
title: 'orgContact: checkMemberGroups'
description: Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье Разрешения.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 15fef20514d63a2009f943ca5956af5f026b2fa5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973344"
---
# <a name="orgcontact-checkmembergroups"></a><span data-ttu-id="2020a-104">orgContact: checkMemberGroups</span><span class="sxs-lookup"><span data-stu-id="2020a-104">orgContact: checkMemberGroups</span></span>

> <span data-ttu-id="2020a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2020a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2020a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2020a-106">Use of these APIs in production applications is not supported.</span></span>

## <a name="permissions"></a><span data-ttu-id="2020a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2020a-107">Permissions</span></span>
<span data-ttu-id="2020a-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2020a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2020a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2020a-110">Permission type</span></span>      | <span data-ttu-id="2020a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2020a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2020a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2020a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2020a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2020a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2020a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2020a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2020a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2020a-115">Not supported.</span></span>    |
|<span data-ttu-id="2020a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2020a-116">Application</span></span> | <span data-ttu-id="2020a-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2020a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2020a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2020a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /contacts/{id}/checkMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="2020a-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2020a-119">Request headers</span></span>
| <span data-ttu-id="2020a-120">Имя</span><span class="sxs-lookup"><span data-stu-id="2020a-120">Name</span></span>       | <span data-ttu-id="2020a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="2020a-121">Type</span></span> | <span data-ttu-id="2020a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="2020a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2020a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2020a-123">Authorization</span></span>  | <span data-ttu-id="2020a-124">строка</span><span class="sxs-lookup"><span data-stu-id="2020a-124">string</span></span>  | <span data-ttu-id="2020a-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2020a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2020a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2020a-127">Request body</span></span>
<span data-ttu-id="2020a-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="2020a-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2020a-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="2020a-129">Parameter</span></span>    | <span data-ttu-id="2020a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="2020a-130">Type</span></span>   |<span data-ttu-id="2020a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2020a-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2020a-132">groupIds</span><span class="sxs-lookup"><span data-stu-id="2020a-132">groupIds</span></span>|<span data-ttu-id="2020a-133">String</span><span class="sxs-lookup"><span data-stu-id="2020a-133">String</span></span>||

## <a name="response"></a><span data-ttu-id="2020a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2020a-134">Response</span></span>

<span data-ttu-id="2020a-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2020a-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2020a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="2020a-136">Example</span></span>
<span data-ttu-id="2020a-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="2020a-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2020a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="2020a-138">Request</span></span>
<span data-ttu-id="2020a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2020a-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "orgcontact_checkmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/contacts/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="2020a-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2020a-140">Response</span></span>
<span data-ttu-id="2020a-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2020a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "orgContact: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
