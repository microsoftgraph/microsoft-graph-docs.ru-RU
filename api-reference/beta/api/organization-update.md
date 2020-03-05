---
title: Обновление организации
description: Обновление свойств объекта organization, для которого выполнена проверка подлинности.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c1d162f3511e49ab3d5462dfca2c033a75c56342
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456339"
---
# <a name="update-organization"></a><span data-ttu-id="95d0c-103">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="95d0c-103">Update organization</span></span>

<span data-ttu-id="95d0c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="95d0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95d0c-105">Обновите свойства организации, которая прошла проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="95d0c-105">Update the properties of the currently authenticated organization.</span></span> <span data-ttu-id="95d0c-106">В этом случае `organization` определяется как коллекция только одной записи, поэтому ее **идентификатор** должен быть указан в запросе.</span><span class="sxs-lookup"><span data-stu-id="95d0c-106">In this case, `organization` is defined as a collection of exactly one record, and so its **ID** must be specified in the request.</span></span>  <span data-ttu-id="95d0c-107">**Идентификатор** также называется **tenantId** Организации.</span><span class="sxs-lookup"><span data-stu-id="95d0c-107">The **ID** is also known as the **tenantId** of the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="95d0c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="95d0c-108">Permissions</span></span>

<span data-ttu-id="95d0c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95d0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95d0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="95d0c-111">Permission type</span></span> | <span data-ttu-id="95d0c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="95d0c-112">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="95d0c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="95d0c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="95d0c-114">Организация. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="95d0c-114">Organization.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="95d0c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="95d0c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="95d0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95d0c-116">Not supported.</span></span> |
|<span data-ttu-id="95d0c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="95d0c-117">Application</span></span> | <span data-ttu-id="95d0c-118">Organization.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95d0c-118">Organization.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="95d0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="95d0c-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}
```

## <a name="request-headers"></a><span data-ttu-id="95d0c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="95d0c-120">Request headers</span></span>

| <span data-ttu-id="95d0c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="95d0c-121">Name</span></span>       | <span data-ttu-id="95d0c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="95d0c-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="95d0c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="95d0c-123">Authorization</span></span>  | <span data-ttu-id="95d0c-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95d0c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="95d0c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="95d0c-126">Content-Type</span></span>   | <span data-ttu-id="95d0c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="95d0c-127">application/json</span></span> |


## <a name="request-body"></a><span data-ttu-id="95d0c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="95d0c-128">Request body</span></span>

<span data-ttu-id="95d0c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="95d0c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="95d0c-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="95d0c-132">Property</span></span>  | <span data-ttu-id="95d0c-133">Тип</span><span class="sxs-lookup"><span data-stu-id="95d0c-133">Type</span></span> |<span data-ttu-id="95d0c-134">Описание</span><span class="sxs-lookup"><span data-stu-id="95d0c-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95d0c-135">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="95d0c-135">marketingNotificationEmails</span></span>|<span data-ttu-id="95d0c-136">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95d0c-136">String collection</span></span>|                                        <span data-ttu-id="95d0c-137">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="95d0c-137">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="95d0c-138">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="95d0c-138">privacyProfile</span></span>|[<span data-ttu-id="95d0c-139">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="95d0c-139">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="95d0c-140">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="95d0c-140">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="95d0c-141">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="95d0c-141">securityComplianceNotificationMails</span></span>|<span data-ttu-id="95d0c-142">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95d0c-142">String collection</span></span>||
|<span data-ttu-id="95d0c-143">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="95d0c-143">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="95d0c-144">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95d0c-144">String collection</span></span>||
|<span data-ttu-id="95d0c-145">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="95d0c-145">technicalNotificationMails</span></span>|<span data-ttu-id="95d0c-146">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95d0c-146">String collection</span></span>|                                        <span data-ttu-id="95d0c-147">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="95d0c-147">**Notes**: not nullable.</span></span>            |

<span data-ttu-id="95d0c-148">Так как ресурс **Организации** поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, зависящие от приложения, в пользовательских свойствах расширения в существующем экземпляре **Организации** .</span><span class="sxs-lookup"><span data-stu-id="95d0c-148">Since the **organization** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **organization** instance.</span></span>

## <a name="response"></a><span data-ttu-id="95d0c-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d0c-149">Response</span></span>

<span data-ttu-id="95d0c-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="95d0c-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95d0c-152">Пример</span><span class="sxs-lookup"><span data-stu-id="95d0c-152">Example</span></span>
##### <a name="request"></a><span data-ttu-id="95d0c-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="95d0c-153">Request</span></span>
<span data-ttu-id="95d0c-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="95d0c-154">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="95d0c-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="95d0c-155">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="95d0c-156">C#</span><span class="sxs-lookup"><span data-stu-id="95d0c-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="95d0c-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="95d0c-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="95d0c-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="95d0c-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="95d0c-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="95d0c-159">Response</span></span>

<span data-ttu-id="95d0c-160">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="95d0c-160">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="95d0c-161">См. также</span><span class="sxs-lookup"><span data-stu-id="95d0c-161">See also</span></span>

- [<span data-ttu-id="95d0c-162">Добавление пользовательских данных в ресурсы с помощью расширений</span><span class="sxs-lookup"><span data-stu-id="95d0c-162">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="95d0c-163">Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="95d0c-163">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)

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
