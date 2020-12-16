---
title: 'conversationMember: add'
description: Массовое добавление участников в команду.
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 2af435ac7dd430a0d006df609991f0c0a83b02ca
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689711"
---
# <a name="conversationmember-add"></a><span data-ttu-id="aa0b1-103">conversationMember: add</span><span class="sxs-lookup"><span data-stu-id="aa0b1-103">conversationMember: add</span></span>

<span data-ttu-id="aa0b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa0b1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa0b1-105">Добавление нескольких участников в [команду](../resources/team.md) одним запросом.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-105">Add multiple members in a single request to a [team](../resources/team.md).</span></span> <span data-ttu-id="aa0b1-106">Отклик предоставляет сведения о том, каких участников можно создать, а каких — нельзя.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-106">The response provides details about which memberships could and could not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="aa0b1-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aa0b1-107">Permissions</span></span>

<span data-ttu-id="aa0b1-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aa0b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa0b1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aa0b1-110">Permission type</span></span>      | <span data-ttu-id="aa0b1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aa0b1-111">Permissions (from least to most privileged)</span></span> | 
|:--------------------|:--------------------------|
| <span data-ttu-id="aa0b1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aa0b1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aa0b1-113">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa0b1-113">TeamMember.ReadWrite.All</span></span>  |
| <span data-ttu-id="aa0b1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aa0b1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aa0b1-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="aa0b1-115">Not supported</span></span> |
| <span data-ttu-id="aa0b1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="aa0b1-116">Application</span></span> | <span data-ttu-id="aa0b1-117">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa0b1-117">TeamMember.ReadWrite.All</span></span>   |


## <a name="http-request"></a><span data-ttu-id="aa0b1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aa0b1-118">HTTP Request</span></span>

<span data-ttu-id="aa0b1-119">Это связывающее действие для добавления нескольких элементов в коллекцию **conversationMember** одним запросом.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-119">This is a bound action for adding multiple elements to a **conversationMember** collection in a single request.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/members/add
```

## <a name="request-headers"></a><span data-ttu-id="aa0b1-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aa0b1-120">Request headers</span></span>

| <span data-ttu-id="aa0b1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="aa0b1-121">Header</span></span>        | <span data-ttu-id="aa0b1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="aa0b1-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="aa0b1-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aa0b1-123">Authorization</span></span> | <span data-ttu-id="aa0b1-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aa0b1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aa0b1-126">Request body</span></span>
<span data-ttu-id="aa0b1-127">В тексте запроса укажите в формате JSON представление списка производных `conversationMember`, которые необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-127">In the request body, supply the JSON representation of the list of `conversationMember` derivatives that need to be added to the team.</span></span>

<span data-ttu-id="aa0b1-128">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="aa0b1-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="aa0b1-129">Parameter</span></span>|<span data-ttu-id="aa0b1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="aa0b1-130">Type</span></span>|<span data-ttu-id="aa0b1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="aa0b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa0b1-132">values</span><span class="sxs-lookup"><span data-stu-id="aa0b1-132">values</span></span>|<span data-ttu-id="aa0b1-133">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="aa0b1-133">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="aa0b1-134">Список участников беседы, которых следует добавить.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-134">List of conversation members that should be added.</span></span>|


## <a name="response"></a><span data-ttu-id="aa0b1-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa0b1-135">Response</span></span>

<span data-ttu-id="aa0b1-136">В случае успеха это действие возвращает код отклика `200 OK` и коллекцию производных ресурса [actionResultPart](../resources/actionresultpart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-136">If successful, this action returns a `200 OK` response code and a collection of derivatives of [actionResultPart](../resources/actionresultpart.md) in the response body.</span></span>

<span data-ttu-id="aa0b1-137">Этот API возвращает отклик `200` с указанием, что все предоставленные участники были добавлены в команду, или отклик `207` с указанием, что только некоторые из предоставленных участников были добавлены в команду.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-137">This API returns a `200` response indicating all members supplied were added to the team or a `207` response indicating that only some of the supplied members were added to the team.</span></span> <span data-ttu-id="aa0b1-138">Вызывающая сторона должна проверить полезные данные отклика, чтобы определить, какого участника не удалось добавить.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-138">The caller should inspect the response payload to determine which member additions failed.</span></span> <span data-ttu-id="aa0b1-139">Текст отклика является коллекцией производных ресурса [actionResultPart](../resources/actionresultpart.md).</span><span class="sxs-lookup"><span data-stu-id="aa0b1-139">The response body is a collection of derivatives of the [actionResultPart](../resources/actionresultpart.md) resource.</span></span>

## <a name="examples"></a><span data-ttu-id="aa0b1-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="aa0b1-140">Examples</span></span>

### <a name="example-1-add-members-in-bulk-to-a-team"></a><span data-ttu-id="aa0b1-141">Пример 1. Массовое добавление участников в команду</span><span class="sxs-lookup"><span data-stu-id="aa0b1-141">Example 1: Add members in bulk to a team</span></span>

#### <a name="request"></a><span data-ttu-id="aa0b1-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa0b1-142">Request</span></span>

<span data-ttu-id="aa0b1-143">В следующем примере показан запрос на добавление нескольких участников в команду.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-143">The following example shows a request to add multiple members to a team.</span></span>

# <a name="http"></a>[<span data-ttu-id="aa0b1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa0b1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team"
}-->

```http
POST https://graph.microsoft.com/beta/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="aa0b1-145">C#</span><span class="sxs-lookup"><span data-stu-id="aa0b1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bulkaddmembers-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa0b1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa0b1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bulkaddmembers-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa0b1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa0b1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bulkaddmembers-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa0b1-148">Java</span><span class="sxs-lookup"><span data-stu-id="aa0b1-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bulkaddmembers-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aa0b1-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa0b1-149">Response</span></span>

<span data-ttu-id="aa0b1-150">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-150">The following is the response.</span></span>

> <span data-ttu-id="aa0b1-151">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-151">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.actionResultPart)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.aadUserConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": null
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```

### <a name="example-2-add-members-in-bulk-and-encounter-partial-failure"></a><span data-ttu-id="aa0b1-152">Пример 2. Массовое добавление участников с возникновением частичного сбоя</span><span class="sxs-lookup"><span data-stu-id="aa0b1-152">Example 2: Add members in bulk and encounter partial failure</span></span>

#### <a name="request"></a><span data-ttu-id="aa0b1-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="aa0b1-153">Request</span></span>

<span data-ttu-id="aa0b1-154">В следующем примере показан запрос на добавление нескольких участников в команду, приводящий к частичному сбою.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-154">The following example shows a request to add multiple members to a team that results in a partial failure.</span></span>


# <a name="http"></a>[<span data-ttu-id="aa0b1-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="aa0b1-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bulkaddmembers_team_partial_failure"
}-->

```http
POST https://graph.microsoft.com/beta/teams/e4183b04-c9a2-417c-bde4-70e3ee46a6dc/members/add
Content-Type: application/json

{
    "values": [
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":[],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('18a80140-b0fb-4489-b360-2f6efaf225a0')"
        },
        {
            "@odata.type": "microsoft.graph.aadUserConversationMember",
            "roles":["owner"],
            "user@odata.bind": "https://graph.microsoft.com/beta/users('86503198-b81b-43fe-81ee-ad45b8848ac9')"
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="aa0b1-156">C#</span><span class="sxs-lookup"><span data-stu-id="aa0b1-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bulkaddmembers-team-partial-failure-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aa0b1-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aa0b1-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bulkaddmembers-team-partial-failure-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aa0b1-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aa0b1-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bulkaddmembers-team-partial-failure-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aa0b1-159">Java</span><span class="sxs-lookup"><span data-stu-id="aa0b1-159">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bulkaddmembers-team-partial-failure-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aa0b1-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="aa0b1-160">Response</span></span>

<span data-ttu-id="aa0b1-161">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-161">The following is the response.</span></span>

> <span data-ttu-id="aa0b1-162">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="aa0b1-162">**Note:** The response object shown here might be shortened for readability.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.actionResultPart)"
} -->

```http
HTTP/1.1 207 MULTI-STATUS
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.addConversationMemberResult)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "18a80140-b0fb-4489-b360-2f6efaf225a0",
            "error": {
                "code": "NotFound",
                "message": ""
            }
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMemberResult",
            "userId": "86503198-b81b-43fe-81ee-ad45b8848ac9",
            "error": null
        }
    ]
}
```


## <a name="see-also"></a><span data-ttu-id="aa0b1-163">См. также</span><span class="sxs-lookup"><span data-stu-id="aa0b1-163">See also</span></span>

- [<span data-ttu-id="aa0b1-164">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="aa0b1-164">Add member to team</span></span>](team-post-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add members to team in bulk",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
