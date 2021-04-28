---
title: Обновление правила
description: Изменение записываемых свойств объекта messageRule и сохранение изменений.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2b4aa70734a0dad302433f33b6f1ab2de888414a
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039379"
---
# <a name="update-rule"></a><span data-ttu-id="98912-103">Обновление правила</span><span class="sxs-lookup"><span data-stu-id="98912-103">Update rule</span></span>

<span data-ttu-id="98912-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98912-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="98912-105">Изменение записываемых свойств объекта [messageRule](../resources/messagerule.md) и сохранение изменений.</span><span class="sxs-lookup"><span data-stu-id="98912-105">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="98912-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98912-106">Permissions</span></span>
<span data-ttu-id="98912-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98912-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98912-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98912-109">Permission type</span></span>      | <span data-ttu-id="98912-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98912-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98912-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98912-111">Delegated (work or school account)</span></span> | <span data-ttu-id="98912-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98912-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="98912-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98912-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98912-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98912-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="98912-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98912-115">Application</span></span> | <span data-ttu-id="98912-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98912-116">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="98912-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98912-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messageRules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="98912-118">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98912-118">Optional request headers</span></span>
| <span data-ttu-id="98912-119">Имя</span><span class="sxs-lookup"><span data-stu-id="98912-119">Name</span></span>       | <span data-ttu-id="98912-120">Описание</span><span class="sxs-lookup"><span data-stu-id="98912-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="98912-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98912-121">Authorization</span></span>  | <span data-ttu-id="98912-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98912-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="98912-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98912-124">Request body</span></span>
<span data-ttu-id="98912-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="98912-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="98912-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="98912-128">Property</span></span>     | <span data-ttu-id="98912-129">Тип</span><span class="sxs-lookup"><span data-stu-id="98912-129">Type</span></span>   |<span data-ttu-id="98912-130">Описание</span><span class="sxs-lookup"><span data-stu-id="98912-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="98912-131">actions</span><span class="sxs-lookup"><span data-stu-id="98912-131">actions</span></span> | [<span data-ttu-id="98912-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="98912-132">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="98912-133">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="98912-133">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="98912-134">conditions</span><span class="sxs-lookup"><span data-stu-id="98912-134">conditions</span></span> | [<span data-ttu-id="98912-135">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="98912-135">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="98912-136">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="98912-136">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="98912-137">displayName</span><span class="sxs-lookup"><span data-stu-id="98912-137">displayName</span></span> | <span data-ttu-id="98912-138">String</span><span class="sxs-lookup"><span data-stu-id="98912-138">String</span></span> | <span data-ttu-id="98912-139">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="98912-139">The display name of the rule.</span></span> |
| <span data-ttu-id="98912-140">exceptions</span><span class="sxs-lookup"><span data-stu-id="98912-140">exceptions</span></span> | [<span data-ttu-id="98912-141">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="98912-141">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="98912-142">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="98912-142">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="98912-143">isEnabled</span><span class="sxs-lookup"><span data-stu-id="98912-143">isEnabled</span></span> | <span data-ttu-id="98912-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="98912-144">Boolean</span></span> | <span data-ttu-id="98912-145">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="98912-145">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="98912-146">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="98912-146">isReadOnly</span></span> | <span data-ttu-id="98912-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="98912-147">Boolean</span></span> | <span data-ttu-id="98912-148">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="98912-148">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="98912-149">sequence</span><span class="sxs-lookup"><span data-stu-id="98912-149">sequence</span></span> | <span data-ttu-id="98912-150">Int32</span><span class="sxs-lookup"><span data-stu-id="98912-150">Int32</span></span> | <span data-ttu-id="98912-151">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="98912-151">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="98912-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="98912-152">Response</span></span>
<span data-ttu-id="98912-153">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="98912-153">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98912-154">Пример</span><span class="sxs-lookup"><span data-stu-id="98912-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98912-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="98912-155">Request</span></span>
<span data-ttu-id="98912-156">В приведенном ниже примере меняется имя правила, а также действия, выполняемые с этим правилом в [примере](messagerule-get.md#example) [получения правила](messagerule-get.md), — вместо пересылки на указанный адрес устанавливается высокая важность.</span><span class="sxs-lookup"><span data-stu-id="98912-156">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 

# <a name="http"></a>[<span data-ttu-id="98912-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="98912-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZqA="],
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=
Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
# <a name="c"></a>[<span data-ttu-id="98912-158">C#</span><span class="sxs-lookup"><span data-stu-id="98912-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="98912-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="98912-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="98912-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="98912-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="98912-161">Java</span><span class="sxs-lookup"><span data-stu-id="98912-161">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-messagerule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="98912-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="98912-162">Response</span></span>
<span data-ttu-id="98912-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98912-163">Here is an example of the response.</span></span> <span data-ttu-id="98912-164">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="98912-164">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"Important from partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "markImportance": "high"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

