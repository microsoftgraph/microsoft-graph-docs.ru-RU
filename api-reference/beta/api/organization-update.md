---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: cae41ed267ea4595134247cf1ac3967ce34141a5
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785937"
---
# <a name="update-organization"></a><span data-ttu-id="780c9-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="780c9-103">Update organization</span></span>

<span data-ttu-id="780c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="780c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="780c9-105">Обновите свойства организации, которая прошла проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="780c9-105">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="780c9-106">В этом случае определяется как коллекция ровно одной записи, поэтому ее ID должен быть указан `organization` в запросе. </span><span class="sxs-lookup"><span data-stu-id="780c9-106">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="780c9-107">**ID** также известен как **tenantId** организации.</span><span class="sxs-lookup"><span data-stu-id="780c9-107">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="780c9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="780c9-108">Permissions</span></span>

<span data-ttu-id="780c9-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="780c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="780c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="780c9-111">Permission type</span></span> | <span data-ttu-id="780c9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="780c9-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="780c9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="780c9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="780c9-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="780c9-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="780c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="780c9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="780c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="780c9-116">Not supported.</span></span> |
|<span data-ttu-id="780c9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="780c9-117">Application</span></span> | <span data-ttu-id="780c9-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="780c9-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="780c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="780c9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="780c9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="780c9-120">Request headers</span></span>

| <span data-ttu-id="780c9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="780c9-121">Name</span></span>       | <span data-ttu-id="780c9-122">Описание</span><span class="sxs-lookup"><span data-stu-id="780c9-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="780c9-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="780c9-123">Authorization</span></span>  | <span data-ttu-id="780c9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="780c9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="780c9-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="780c9-126">Content-Type</span></span>   | <span data-ttu-id="780c9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="780c9-127">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="780c9-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="780c9-128">Request body</span></span>

<span data-ttu-id="780c9-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="780c9-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="780c9-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="780c9-132">Property</span></span>  | <span data-ttu-id="780c9-133">Тип</span><span class="sxs-lookup"><span data-stu-id="780c9-133">Type</span></span> |<span data-ttu-id="780c9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="780c9-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="780c9-135">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="780c9-135">marketingNotificationEmails</span></span>|<span data-ttu-id="780c9-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="780c9-136">String collection</span></span>|                                        <span data-ttu-id="780c9-137">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="780c9-137">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="780c9-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="780c9-138">privacyProfile</span></span>|[<span data-ttu-id="780c9-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="780c9-139">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="780c9-140">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="780c9-140">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="780c9-141">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="780c9-141">securityComplianceNotificationMails</span></span>|<span data-ttu-id="780c9-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="780c9-142">String collection</span></span>||
|<span data-ttu-id="780c9-143">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="780c9-143">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="780c9-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="780c9-144">String collection</span></span>||
|<span data-ttu-id="780c9-145">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="780c9-145">technicalNotificationMails</span></span>|<span data-ttu-id="780c9-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="780c9-146">String collection</span></span>|                                        <span data-ttu-id="780c9-147">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="780c9-147">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="780c9-148">Так как ресурс **организации** поддерживает [расширения,](/graph/extensibility-overview)операцию можно использовать для добавления, обновления или удаления собственных данных, определенных для приложения, в настраиваемом свойстве расширения в существующем экземпляре `PATCH` организации. </span><span class="sxs-lookup"><span data-stu-id="780c9-148">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="780c9-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="780c9-149">Response</span></span>

<span data-ttu-id="780c9-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="780c9-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="780c9-152">Пример</span><span class="sxs-lookup"><span data-stu-id="780c9-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="780c9-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="780c9-153">Request</span></span>
<span data-ttu-id="780c9-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="780c9-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="780c9-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="780c9-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{id}
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
# <a name="c"></a>[<span data-ttu-id="780c9-156">C#</span><span class="sxs-lookup"><span data-stu-id="780c9-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="780c9-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="780c9-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="780c9-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="780c9-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="780c9-159">Java</span><span class="sxs-lookup"><span data-stu-id="780c9-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="780c9-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="780c9-160">Response</span></span>

<span data-ttu-id="780c9-161">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="780c9-161">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="780c9-162">См. также</span><span class="sxs-lookup"><span data-stu-id="780c9-162">See also</span></span>

- [<span data-ttu-id="780c9-163">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="780c9-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="780c9-164">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="780c9-164">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


