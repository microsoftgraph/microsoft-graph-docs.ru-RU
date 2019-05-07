---
title: 'servicePrincipal: getMemberObjects'
description: Получение списка групп и ролей каталогов, членом которых является данный участник службы.  Эта проверка является транзитивным.
localization_priority: Normal
ms.openlocfilehash: 00f49c3b33133dcabeaf08bab1740fe50ea6b662
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638713"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="20cec-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="20cec-104">servicePrincipal: getMemberObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20cec-105">Получение списка групп и ролей каталогов, членом которых является данный участник службы.</span><span class="sxs-lookup"><span data-stu-id="20cec-105">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="20cec-106">Эта проверка является транзитивным.</span><span class="sxs-lookup"><span data-stu-id="20cec-106">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="20cec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20cec-107">Permissions</span></span>
<span data-ttu-id="20cec-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20cec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20cec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20cec-110">Permission type</span></span>      | <span data-ttu-id="20cec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20cec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20cec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20cec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="20cec-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="20cec-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="20cec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20cec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20cec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20cec-115">Not supported.</span></span>    |
|<span data-ttu-id="20cec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20cec-116">Application</span></span> | <span data-ttu-id="20cec-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20cec-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="20cec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20cec-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="20cec-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20cec-119">Request headers</span></span>
| <span data-ttu-id="20cec-120">Имя</span><span class="sxs-lookup"><span data-stu-id="20cec-120">Name</span></span>       | <span data-ttu-id="20cec-121">Тип</span><span class="sxs-lookup"><span data-stu-id="20cec-121">Type</span></span> | <span data-ttu-id="20cec-122">Описание</span><span class="sxs-lookup"><span data-stu-id="20cec-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="20cec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20cec-123">Authorization</span></span>  | <span data-ttu-id="20cec-124">string</span><span class="sxs-lookup"><span data-stu-id="20cec-124">string</span></span>  | <span data-ttu-id="20cec-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20cec-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20cec-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20cec-127">Request body</span></span>
<span data-ttu-id="20cec-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="20cec-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="20cec-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="20cec-129">Parameter</span></span>    | <span data-ttu-id="20cec-130">Тип</span><span class="sxs-lookup"><span data-stu-id="20cec-130">Type</span></span>   |<span data-ttu-id="20cec-131">Описание</span><span class="sxs-lookup"><span data-stu-id="20cec-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20cec-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="20cec-132">securityEnabledOnly</span></span>|<span data-ttu-id="20cec-133">Логическое</span><span class="sxs-lookup"><span data-stu-id="20cec-133">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="20cec-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="20cec-134">Response</span></span>

<span data-ttu-id="20cec-135">В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20cec-135">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20cec-136">Пример</span><span class="sxs-lookup"><span data-stu-id="20cec-136">Example</span></span>
<span data-ttu-id="20cec-137">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="20cec-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="20cec-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="20cec-138">Request</span></span>
<span data-ttu-id="20cec-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20cec-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="20cec-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="20cec-140">Response</span></span>
<span data-ttu-id="20cec-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="20cec-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="20cec-144">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="20cec-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="20cec-145">Языках</span><span class="sxs-lookup"><span data-stu-id="20cec-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/serviceprincipal_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="20cec-146">Язык</span><span class="sxs-lookup"><span data-stu-id="20cec-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/serviceprincipal_getmemberobjects-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
