---
title: 'conversationMember: add'
description: Массовое добавление участников в команду.
author: nkramer
doc_type: apiPageType
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: ffc3d9d36c0f4d22653a961ebe5af4769f286d7d
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658356"
---
# <a name="conversationmember-add"></a><span data-ttu-id="d5866-103">conversationMember: add</span><span class="sxs-lookup"><span data-stu-id="d5866-103">conversationMember: add</span></span>

<span data-ttu-id="d5866-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5866-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5866-105">Добавление нескольких участников в [команду](../resources/team.md) одним запросом.</span><span class="sxs-lookup"><span data-stu-id="d5866-105">Add multiple members in a single request to a [team](../resources/team.md).</span></span> <span data-ttu-id="d5866-106">Отклик предоставляет сведения о том, каких участников можно создать, а каких — нельзя.</span><span class="sxs-lookup"><span data-stu-id="d5866-106">The response provides details about which memberships could and could not be created.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5866-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d5866-107">Permissions</span></span>

<span data-ttu-id="d5866-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5866-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5866-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5866-110">Permission type</span></span>      | <span data-ttu-id="d5866-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5866-111">Permissions (from least to most privileged)</span></span> | 
|:--------------------|:--------------------------|
| <span data-ttu-id="d5866-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5866-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d5866-113">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5866-113">TeamMember.ReadWrite.All</span></span>  |
| <span data-ttu-id="d5866-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5866-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5866-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d5866-115">Not supported</span></span> |
| <span data-ttu-id="d5866-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d5866-116">Application</span></span> | <span data-ttu-id="d5866-117">TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5866-117">TeamMember.ReadWrite.All</span></span>   |


## <a name="http-request"></a><span data-ttu-id="d5866-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5866-118">HTTP Request</span></span>

<span data-ttu-id="d5866-119">Это связывающее действие для добавления нескольких элементов в коллекцию **conversationMember** одним запросом.</span><span class="sxs-lookup"><span data-stu-id="d5866-119">This is a bound action for adding multiple elements to a **conversationMember** collection in a single request.</span></span>
<!-- { "blockType": "ignored" } -->

```http
POST /teams/{team-id}/members/add
```

## <a name="request-headers"></a><span data-ttu-id="d5866-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d5866-120">Request headers</span></span>

| <span data-ttu-id="d5866-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5866-121">Header</span></span>        | <span data-ttu-id="d5866-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d5866-122">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="d5866-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d5866-123">Authorization</span></span> | <span data-ttu-id="d5866-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5866-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5866-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d5866-126">Request body</span></span>
<span data-ttu-id="d5866-127">В тексте запроса укажите в формате JSON представление списка производных `conversationMember`, которые необходимо добавить.</span><span class="sxs-lookup"><span data-stu-id="d5866-127">In the request body, supply the JSON representation of the list of `conversationMember` derivatives that need to be added to the team.</span></span>

<span data-ttu-id="d5866-128">В следующей таблице указаны параметры, которые можно использовать с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d5866-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d5866-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="d5866-129">Parameter</span></span>|<span data-ttu-id="d5866-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d5866-130">Type</span></span>|<span data-ttu-id="d5866-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d5866-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5866-132">values</span><span class="sxs-lookup"><span data-stu-id="d5866-132">values</span></span>|<span data-ttu-id="d5866-133">Коллекция [conversationMember](../resources/conversationmember.md)</span><span class="sxs-lookup"><span data-stu-id="d5866-133">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="d5866-134">Список участников беседы, которых следует добавить.</span><span class="sxs-lookup"><span data-stu-id="d5866-134">List of conversation members that should be added.</span></span>|


## <a name="response"></a><span data-ttu-id="d5866-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5866-135">Response</span></span>

<span data-ttu-id="d5866-136">В случае успеха это действие возвращает код отклика `200 OK` и коллекцию производных ресурса [actionResultPart](../resources/actionresultpart.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d5866-136">If successful, this action returns a `200 OK` response code and a collection of derivatives of [actionResultPart](../resources/actionresultpart.md) in the response body.</span></span>

<span data-ttu-id="d5866-137">Этот API возвращает отклик `200` с указанием, что все предоставленные участники были добавлены в команду, или отклик `207` с указанием, что только некоторые из предоставленных участников были добавлены в команду.</span><span class="sxs-lookup"><span data-stu-id="d5866-137">This API returns a `200` response indicating all members supplied were added to the team or a `207` response indicating that only some of the supplied members were added to the team.</span></span> <span data-ttu-id="d5866-138">Вызывающая сторона должна проверить полезные данные отклика, чтобы определить, какого участника не удалось добавить.</span><span class="sxs-lookup"><span data-stu-id="d5866-138">The caller should inspect the response payload to determine which member additions failed.</span></span> <span data-ttu-id="d5866-139">Текст отклика является коллекцией производных ресурса [actionResultPart](../resources/actionresultpart.md).</span><span class="sxs-lookup"><span data-stu-id="d5866-139">The response body is a collection of derivatives of the [actionResultPart](../resources/actionresultpart.md) resource.</span></span>

## <a name="examples"></a><span data-ttu-id="d5866-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="d5866-140">Examples</span></span>

### <a name="example-1-add-members-in-bulk-to-a-team"></a><span data-ttu-id="d5866-141">Пример 1. Массовое добавление участников в команду</span><span class="sxs-lookup"><span data-stu-id="d5866-141">Example 1: Add members in bulk to a team</span></span>

#### <a name="request"></a><span data-ttu-id="d5866-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5866-142">Request</span></span>

<span data-ttu-id="d5866-143">В следующем примере показан запрос на добавление нескольких участников в команду.</span><span class="sxs-lookup"><span data-stu-id="d5866-143">The following example shows a request to add multiple members to a team.</span></span>
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

#### <a name="response"></a><span data-ttu-id="d5866-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5866-144">Response</span></span>

<span data-ttu-id="d5866-145">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="d5866-145">The following is the response.</span></span>

> <span data-ttu-id="d5866-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d5866-146">**Note:** The response object shown here might be shortened for readability.</span></span> 
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

### <a name="example-2-add-members-in-bulk-and-encounter-partial-failure"></a><span data-ttu-id="d5866-147">Пример 2. Массовое добавление участников с возникновением частичного сбоя</span><span class="sxs-lookup"><span data-stu-id="d5866-147">Example 2: Add members in bulk and encounter partial failure</span></span>

#### <a name="request"></a><span data-ttu-id="d5866-148">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5866-148">Request</span></span>

<span data-ttu-id="d5866-149">В следующем примере показан запрос на добавление нескольких участников в команду, приводящий к частичному сбою.</span><span class="sxs-lookup"><span data-stu-id="d5866-149">The following example shows a request to add multiple members to a team that results in a partial failure.</span></span>

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

#### <a name="response"></a><span data-ttu-id="d5866-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5866-150">Response</span></span>

<span data-ttu-id="d5866-151">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="d5866-151">The following is the response.</span></span>

> <span data-ttu-id="d5866-152">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d5866-152">**Note:** The response object shown here might be shortened for readability.</span></span> 
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


## <a name="see-also"></a><span data-ttu-id="d5866-153">См. также</span><span class="sxs-lookup"><span data-stu-id="d5866-153">See also</span></span>

- [<span data-ttu-id="d5866-154">Добавление участника в команду</span><span class="sxs-lookup"><span data-stu-id="d5866-154">Add member to team</span></span>](team-post-members.md)

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
