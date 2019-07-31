---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93e6c9073488278758f9a5a35e5528e113fc3c87
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35988827"
---
# <a name="update-organization"></a><span data-ttu-id="baec8-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="baec8-103">Update organization</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baec8-104">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="baec8-104">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="baec8-105">В этом случае `organization` определяется как коллекция только одной записи, поэтому ее **идентификатор** должен быть указан в запросе.</span><span class="sxs-lookup"><span data-stu-id="baec8-105">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="baec8-106">**Идентификатор** также называется **tenantId** Организации.</span><span class="sxs-lookup"><span data-stu-id="baec8-106">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="baec8-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="baec8-107">Permissions</span></span>

<span data-ttu-id="baec8-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="baec8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baec8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="baec8-110">Permission type</span></span> | <span data-ttu-id="baec8-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="baec8-111">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baec8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="baec8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="baec8-113">Организация. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="baec8-113">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="baec8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="baec8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baec8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baec8-115">Not supported.</span></span> |
|<span data-ttu-id="baec8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="baec8-116">Application</span></span> | <span data-ttu-id="baec8-117">Организация. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="baec8-117">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="baec8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="baec8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="baec8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="baec8-119">Request headers</span></span>

| <span data-ttu-id="baec8-120">Имя</span><span class="sxs-lookup"><span data-stu-id="baec8-120">Name</span></span>       | <span data-ttu-id="baec8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="baec8-121">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="baec8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="baec8-122">Authorization</span></span>  | <span data-ttu-id="baec8-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="baec8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="baec8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="baec8-125">Content-Type</span></span>   | <span data-ttu-id="baec8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="baec8-126">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="baec8-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="baec8-127">Request body</span></span>

<span data-ttu-id="baec8-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="baec8-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="baec8-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="baec8-131">Property</span></span>  | <span data-ttu-id="baec8-132">Тип</span><span class="sxs-lookup"><span data-stu-id="baec8-132">Type</span></span> |<span data-ttu-id="baec8-133">Описание</span><span class="sxs-lookup"><span data-stu-id="baec8-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baec8-134">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="baec8-134">marketingNotificationEmails</span></span>|<span data-ttu-id="baec8-135">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="baec8-135">String collection</span></span>|                                        <span data-ttu-id="baec8-136">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="baec8-136">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="baec8-137">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="baec8-137">privacyProfile</span></span>|[<span data-ttu-id="baec8-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="baec8-138">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="baec8-139">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="baec8-139">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="baec8-140">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="baec8-140">securityComplianceNotificationMails</span></span>|<span data-ttu-id="baec8-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="baec8-141">String collection</span></span>||
|<span data-ttu-id="baec8-142">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="baec8-142">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="baec8-143">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="baec8-143">String collection</span></span>||
|<span data-ttu-id="baec8-144">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="baec8-144">technicalNotificationMails</span></span>|<span data-ttu-id="baec8-145">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="baec8-145">String collection</span></span>|                                        <span data-ttu-id="baec8-146">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="baec8-146">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="baec8-147">Так как ресурс **Организации** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **Организации** .</span><span class="sxs-lookup"><span data-stu-id="baec8-147">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="baec8-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="baec8-148">Response</span></span>

<span data-ttu-id="baec8-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="baec8-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baec8-151">Пример</span><span class="sxs-lookup"><span data-stu-id="baec8-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="baec8-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="baec8-152">Request</span></span>
<span data-ttu-id="baec8-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="baec8-153">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="baec8-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="baec8-154">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="baec8-155">C#</span><span class="sxs-lookup"><span data-stu-id="baec8-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="baec8-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="baec8-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="baec8-157">Цель — C</span><span class="sxs-lookup"><span data-stu-id="baec8-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="baec8-158">Java</span><span class="sxs-lookup"><span data-stu-id="baec8-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="baec8-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="baec8-159">Response</span></span>

<span data-ttu-id="baec8-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="baec8-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="baec8-161">См. также</span><span class="sxs-lookup"><span data-stu-id="baec8-161">See also</span></span>

- [<span data-ttu-id="baec8-162">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="baec8-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="baec8-163">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="baec8-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
