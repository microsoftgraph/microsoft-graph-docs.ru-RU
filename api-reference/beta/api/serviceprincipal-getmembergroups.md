---
title: 'servicePrincipal: getMemberGroups'
description: Получение списка групп, участника-службы является членом.  Проверка доверия транзитивных.
localization_priority: Normal
ms.openlocfilehash: 6d552b410da23e5675257340ddc61cb4abbcd5e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817649"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="51c28-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="51c28-104">servicePrincipal: getMemberGroups</span></span>

> <span data-ttu-id="51c28-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="51c28-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51c28-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51c28-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="51c28-107">Получение списка групп, участника-службы является членом.</span><span class="sxs-lookup"><span data-stu-id="51c28-107">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="51c28-108">Проверка доверия транзитивных.</span><span class="sxs-lookup"><span data-stu-id="51c28-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="51c28-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="51c28-109">Permissions</span></span>
<span data-ttu-id="51c28-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51c28-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="51c28-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51c28-112">Permission type</span></span>      | <span data-ttu-id="51c28-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51c28-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51c28-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51c28-114">Delegated (work or school account)</span></span> | <span data-ttu-id="51c28-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51c28-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="51c28-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51c28-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51c28-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51c28-117">Not supported.</span></span>    |
|<span data-ttu-id="51c28-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51c28-118">Application</span></span> | <span data-ttu-id="51c28-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51c28-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="51c28-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51c28-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="51c28-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="51c28-121">Request headers</span></span>
| <span data-ttu-id="51c28-122">Имя</span><span class="sxs-lookup"><span data-stu-id="51c28-122">Name</span></span>       | <span data-ttu-id="51c28-123">Тип</span><span class="sxs-lookup"><span data-stu-id="51c28-123">Type</span></span> | <span data-ttu-id="51c28-124">Описание</span><span class="sxs-lookup"><span data-stu-id="51c28-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="51c28-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="51c28-125">Authorization</span></span>  | <span data-ttu-id="51c28-126">string</span><span class="sxs-lookup"><span data-stu-id="51c28-126">string</span></span>  | <span data-ttu-id="51c28-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51c28-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="51c28-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="51c28-129">Request body</span></span>
<span data-ttu-id="51c28-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="51c28-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="51c28-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="51c28-131">Parameter</span></span>    | <span data-ttu-id="51c28-132">Тип</span><span class="sxs-lookup"><span data-stu-id="51c28-132">Type</span></span>   |<span data-ttu-id="51c28-133">Описание</span><span class="sxs-lookup"><span data-stu-id="51c28-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="51c28-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="51c28-134">securityEnabledOnly</span></span>|<span data-ttu-id="51c28-135">Логическое</span><span class="sxs-lookup"><span data-stu-id="51c28-135">Boolean</span></span>|<span data-ttu-id="51c28-p106">Задано значение **false**. Возвращение лишь защищенных групп поддерживается только для пользователей.</span><span class="sxs-lookup"><span data-stu-id="51c28-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="51c28-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="51c28-138">Response</span></span>

<span data-ttu-id="51c28-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="51c28-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51c28-140">Пример</span><span class="sxs-lookup"><span data-stu-id="51c28-140">Example</span></span>
<span data-ttu-id="51c28-141">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="51c28-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="51c28-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="51c28-142">Request</span></span>
<span data-ttu-id="51c28-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51c28-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="51c28-144">Ответ</span><span class="sxs-lookup"><span data-stu-id="51c28-144">Response</span></span>
<span data-ttu-id="51c28-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="51c28-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
