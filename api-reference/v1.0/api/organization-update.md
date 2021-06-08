---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6e848342b2a14d836f2fc9c0df68db2f44e0531b
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787452"
---
# <a name="update-organization"></a><span data-ttu-id="1d750-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="1d750-103">Update organization</span></span>

<span data-ttu-id="1d750-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d750-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1d750-105">Обновите свойства организации, которая прошла проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="1d750-105">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="1d750-106">В этом случае определяется как коллекция ровно одной записи, поэтому ее ID должен быть указан `organization` в запросе. </span><span class="sxs-lookup"><span data-stu-id="1d750-106">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="1d750-107">**ID** также известен как **tenantId** организации.</span><span class="sxs-lookup"><span data-stu-id="1d750-107">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d750-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1d750-108">Permissions</span></span>

<span data-ttu-id="1d750-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d750-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d750-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d750-111">Permission type</span></span> | <span data-ttu-id="1d750-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d750-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d750-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d750-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1d750-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d750-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d750-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d750-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d750-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d750-116">Not supported.</span></span>    |
|<span data-ttu-id="1d750-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d750-117">Application</span></span> | <span data-ttu-id="1d750-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d750-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d750-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d750-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1d750-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d750-120">Request headers</span></span>

| <span data-ttu-id="1d750-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1d750-121">Name</span></span>       | <span data-ttu-id="1d750-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1d750-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="1d750-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1d750-123">Authorization</span></span>  | <span data-ttu-id="1d750-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1d750-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d750-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d750-126">Content-Type</span></span>   | <span data-ttu-id="1d750-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1d750-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1d750-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1d750-128">Request body</span></span>

<span data-ttu-id="1d750-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="1d750-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="1d750-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="1d750-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="1d750-131">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1d750-131">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1d750-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d750-132">Property</span></span>     | <span data-ttu-id="1d750-133">Тип</span><span class="sxs-lookup"><span data-stu-id="1d750-133">Type</span></span>   |<span data-ttu-id="1d750-134">Описание</span><span class="sxs-lookup"><span data-stu-id="1d750-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d750-135">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="1d750-135">marketingNotificationEmails</span></span>|<span data-ttu-id="1d750-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1d750-136">String collection</span></span>|                                        <span data-ttu-id="1d750-137">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="1d750-137">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="1d750-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="1d750-138">privacyProfile</span></span>|[<span data-ttu-id="1d750-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="1d750-139">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="1d750-140">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="1d750-140">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="1d750-141">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="1d750-141">securityComplianceNotificationMails</span></span>|<span data-ttu-id="1d750-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1d750-142">String collection</span></span>||
|<span data-ttu-id="1d750-143">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="1d750-143">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="1d750-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1d750-144">String collection</span></span>||
|<span data-ttu-id="1d750-145">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="1d750-145">technicalNotificationMails</span></span>|<span data-ttu-id="1d750-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1d750-146">String collection</span></span>|                                        <span data-ttu-id="1d750-147">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="1d750-147">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="1d750-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d750-148">Response</span></span>

<span data-ttu-id="1d750-149">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1d750-149">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1d750-150">Пример</span><span class="sxs-lookup"><span data-stu-id="1d750-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d750-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d750-151">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1d750-152">HTTP</span><span class="sxs-lookup"><span data-stu-id="1d750-152">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1d750-153">C#</span><span class="sxs-lookup"><span data-stu-id="1d750-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1d750-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1d750-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1d750-155">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1d750-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1d750-156">Java</span><span class="sxs-lookup"><span data-stu-id="1d750-156">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1d750-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d750-157">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

