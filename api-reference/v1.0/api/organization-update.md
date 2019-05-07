---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: de9b712c31c76b8906f2123f85943f2e4e962bab
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33611856"
---
# <a name="update-organization"></a><span data-ttu-id="9ddff-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="9ddff-103">Update organization</span></span>

<span data-ttu-id="9ddff-104">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="9ddff-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="9ddff-105">В этом случае `organization` определяется как коллекция только одной записи, поэтому ее **идентификатор** должен быть указан в запросе.</span><span class="sxs-lookup"><span data-stu-id="9ddff-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="9ddff-106">**Идентификатор** также называется **tenantId** Организации.</span><span class="sxs-lookup"><span data-stu-id="9ddff-106">The **ID** is also known as the **tenantId** of the organization.</span></span>


## <a name="permissions"></a><span data-ttu-id="9ddff-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ddff-107">Permissions</span></span>

<span data-ttu-id="9ddff-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ddff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ddff-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ddff-110">Permission type</span></span> | <span data-ttu-id="9ddff-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ddff-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ddff-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ddff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9ddff-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ddff-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9ddff-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ddff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ddff-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ddff-115">Not supported.</span></span>    |
|<span data-ttu-id="9ddff-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ddff-116">Application</span></span> | <span data-ttu-id="9ddff-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ddff-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ddff-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ddff-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}

```

## <a name="request-headers"></a><span data-ttu-id="9ddff-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ddff-119">Request headers</span></span>

| <span data-ttu-id="9ddff-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9ddff-120">Name</span></span>       | <span data-ttu-id="9ddff-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9ddff-121">Type</span></span> | <span data-ttu-id="9ddff-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9ddff-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9ddff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ddff-123">Authorization</span></span>  | <span data-ttu-id="9ddff-124">string</span><span class="sxs-lookup"><span data-stu-id="9ddff-124">string</span></span>  | <span data-ttu-id="9ddff-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ddff-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ddff-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ddff-127">Request body</span></span>

<span data-ttu-id="9ddff-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="9ddff-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="9ddff-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="9ddff-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9ddff-130">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9ddff-130">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9ddff-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="9ddff-131">Property</span></span>     | <span data-ttu-id="9ddff-132">Тип</span><span class="sxs-lookup"><span data-stu-id="9ddff-132">Type</span></span>   |<span data-ttu-id="9ddff-133">Описание</span><span class="sxs-lookup"><span data-stu-id="9ddff-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ddff-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="9ddff-134">marketingNotificationEmails</span></span>|<span data-ttu-id="9ddff-135">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9ddff-135">String collection</span></span>|                                        <span data-ttu-id="9ddff-136">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="9ddff-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="9ddff-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="9ddff-137">privacyProfile</span></span>|[<span data-ttu-id="9ddff-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="9ddff-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="9ddff-139">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="9ddff-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="9ddff-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="9ddff-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="9ddff-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9ddff-141">String collection</span></span>||
|<span data-ttu-id="9ddff-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="9ddff-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="9ddff-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9ddff-143">String collection</span></span>||
|<span data-ttu-id="9ddff-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="9ddff-144">technicalNotificationMails</span></span>|<span data-ttu-id="9ddff-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="9ddff-145">String collection</span></span>|                                        <span data-ttu-id="9ddff-146">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="9ddff-146">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="9ddff-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ddff-147">Response</span></span>

<span data-ttu-id="9ddff-148">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9ddff-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9ddff-149">Пример</span><span class="sxs-lookup"><span data-stu-id="9ddff-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ddff-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ddff-150">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/{id}
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

### <a name="response"></a><span data-ttu-id="9ddff-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="9ddff-151">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9ddff-152">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9ddff-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="9ddff-153">Языках</span><span class="sxs-lookup"><span data-stu-id="9ddff-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_organization-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ddff-154">Язык</span><span class="sxs-lookup"><span data-stu-id="9ddff-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_organization-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/organization-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
