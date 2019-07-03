---
title: Обновление правила
description: Изменение записываемых свойств объекта messageRule и сохранение изменений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: b6371057d92fddaecfb5c26aad70054114749ab3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447909"
---
# <a name="update-rule"></a><span data-ttu-id="69ce8-103">Обновление правила</span><span class="sxs-lookup"><span data-stu-id="69ce8-103">Update rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69ce8-104">Изменение записываемых свойств объекта [messageRule](../resources/messagerule.md) и сохранение изменений.</span><span class="sxs-lookup"><span data-stu-id="69ce8-104">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="69ce8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="69ce8-105">Permissions</span></span>
<span data-ttu-id="69ce8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69ce8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69ce8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="69ce8-108">Permission type</span></span>      | <span data-ttu-id="69ce8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="69ce8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69ce8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="69ce8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69ce8-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69ce8-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="69ce8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="69ce8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69ce8-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69ce8-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="69ce8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="69ce8-114">Application</span></span> | <span data-ttu-id="69ce8-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="69ce8-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="69ce8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="69ce8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="69ce8-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="69ce8-117">Optional request headers</span></span>
| <span data-ttu-id="69ce8-118">Имя</span><span class="sxs-lookup"><span data-stu-id="69ce8-118">Name</span></span>       | <span data-ttu-id="69ce8-119">Описание</span><span class="sxs-lookup"><span data-stu-id="69ce8-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="69ce8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="69ce8-120">Authorization</span></span>  | <span data-ttu-id="69ce8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="69ce8-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="69ce8-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="69ce8-123">Request body</span></span>
<span data-ttu-id="69ce8-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="69ce8-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="69ce8-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="69ce8-127">Property</span></span>     | <span data-ttu-id="69ce8-128">Тип</span><span class="sxs-lookup"><span data-stu-id="69ce8-128">Type</span></span>   |<span data-ttu-id="69ce8-129">Описание</span><span class="sxs-lookup"><span data-stu-id="69ce8-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="69ce8-130">actions</span><span class="sxs-lookup"><span data-stu-id="69ce8-130">actions</span></span> | [<span data-ttu-id="69ce8-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="69ce8-131">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="69ce8-132">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="69ce8-132">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="69ce8-133">conditions</span><span class="sxs-lookup"><span data-stu-id="69ce8-133">conditions</span></span> | [<span data-ttu-id="69ce8-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="69ce8-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="69ce8-135">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="69ce8-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="69ce8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="69ce8-136">displayName</span></span> | <span data-ttu-id="69ce8-137">String</span><span class="sxs-lookup"><span data-stu-id="69ce8-137">String</span></span> | <span data-ttu-id="69ce8-138">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="69ce8-138">The display name of the rule.</span></span> |
| <span data-ttu-id="69ce8-139">exceptions</span><span class="sxs-lookup"><span data-stu-id="69ce8-139">exceptions</span></span> | [<span data-ttu-id="69ce8-140">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="69ce8-140">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="69ce8-141">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="69ce8-141">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="69ce8-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="69ce8-142">isEnabled</span></span> | <span data-ttu-id="69ce8-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="69ce8-143">Boolean</span></span> | <span data-ttu-id="69ce8-144">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="69ce8-144">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="69ce8-145">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="69ce8-145">isReadOnly</span></span> | <span data-ttu-id="69ce8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="69ce8-146">Boolean</span></span> | <span data-ttu-id="69ce8-147">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="69ce8-147">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="69ce8-148">sequence</span><span class="sxs-lookup"><span data-stu-id="69ce8-148">sequence</span></span> | <span data-ttu-id="69ce8-149">Int32</span><span class="sxs-lookup"><span data-stu-id="69ce8-149">Int32</span></span> | <span data-ttu-id="69ce8-150">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="69ce8-150">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="69ce8-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="69ce8-151">Response</span></span>
<span data-ttu-id="69ce8-152">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="69ce8-152">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69ce8-153">Пример</span><span class="sxs-lookup"><span data-stu-id="69ce8-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69ce8-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="69ce8-154">Request</span></span>
<span data-ttu-id="69ce8-155">В приведенном ниже примере меняется имя правила, а также действия, выполняемые с этим правилом в [примере](messagerule-get.md#example) [получения правила](messagerule-get.md), — вместо пересылки на указанный адрес устанавливается высокая важность.</span><span class="sxs-lookup"><span data-stu-id="69ce8-155">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 

# <a name="httptabhttp"></a>[<span data-ttu-id="69ce8-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="69ce8-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')
Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="69ce8-157">C#</span><span class="sxs-lookup"><span data-stu-id="69ce8-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-messagerule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69ce8-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="69ce8-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-messagerule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69ce8-159">Цель — C</span><span class="sxs-lookup"><span data-stu-id="69ce8-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-messagerule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="69ce8-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="69ce8-160">Response</span></span>
<span data-ttu-id="69ce8-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="69ce8-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
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
<!--
{
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
