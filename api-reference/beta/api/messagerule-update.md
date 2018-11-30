---
title: Обновление правила
description: Изменение записываемых свойств объекта messageRule и сохранение изменений.
ms.openlocfilehash: ab59d0687f80ade06416ab5c4926fbde52754449
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079464"
---
# <a name="update-rule"></a><span data-ttu-id="387cc-103">Обновление правила</span><span class="sxs-lookup"><span data-stu-id="387cc-103">Update rule</span></span>

> <span data-ttu-id="387cc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="387cc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="387cc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="387cc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="387cc-106">Изменение записываемых свойств объекта [messageRule](../resources/messagerule.md) и сохранение изменений.</span><span class="sxs-lookup"><span data-stu-id="387cc-106">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="387cc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="387cc-107">Permissions</span></span>
<span data-ttu-id="387cc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="387cc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="387cc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="387cc-110">Permission type</span></span>      | <span data-ttu-id="387cc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="387cc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="387cc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="387cc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="387cc-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="387cc-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="387cc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="387cc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="387cc-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="387cc-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="387cc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="387cc-116">Application</span></span> | <span data-ttu-id="387cc-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="387cc-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="387cc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="387cc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="387cc-119">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="387cc-119">Optional request headers</span></span>
| <span data-ttu-id="387cc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="387cc-120">Name</span></span>       | <span data-ttu-id="387cc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="387cc-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="387cc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="387cc-122">Authorization</span></span>  | <span data-ttu-id="387cc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="387cc-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="387cc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="387cc-125">Request body</span></span>
<span data-ttu-id="387cc-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="387cc-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="387cc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="387cc-129">Property</span></span>     | <span data-ttu-id="387cc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="387cc-130">Type</span></span>   |<span data-ttu-id="387cc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="387cc-131">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="387cc-132">actions</span><span class="sxs-lookup"><span data-stu-id="387cc-132">actions</span></span> | [<span data-ttu-id="387cc-133">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="387cc-133">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="387cc-134">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="387cc-134">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="387cc-135">conditions</span><span class="sxs-lookup"><span data-stu-id="387cc-135">conditions</span></span> | [<span data-ttu-id="387cc-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="387cc-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="387cc-137">Условия, при соблюдении которых с указанным правилом выполняются соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="387cc-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="387cc-138">displayName</span><span class="sxs-lookup"><span data-stu-id="387cc-138">displayName</span></span> | <span data-ttu-id="387cc-139">String</span><span class="sxs-lookup"><span data-stu-id="387cc-139">String</span></span> | <span data-ttu-id="387cc-140">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="387cc-140">The display name of the rule.</span></span> |
| <span data-ttu-id="387cc-141">exceptions</span><span class="sxs-lookup"><span data-stu-id="387cc-141">exceptions</span></span> | [<span data-ttu-id="387cc-142">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="387cc-142">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="387cc-143">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="387cc-143">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="387cc-144">isEnabled</span><span class="sxs-lookup"><span data-stu-id="387cc-144">isEnabled</span></span> | <span data-ttu-id="387cc-145">Логический</span><span class="sxs-lookup"><span data-stu-id="387cc-145">Boolean</span></span> | <span data-ttu-id="387cc-146">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="387cc-146">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="387cc-147">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="387cc-147">isReadOnly</span></span> | <span data-ttu-id="387cc-148">Логический</span><span class="sxs-lookup"><span data-stu-id="387cc-148">Boolean</span></span> | <span data-ttu-id="387cc-149">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="387cc-149">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="387cc-150">sequence</span><span class="sxs-lookup"><span data-stu-id="387cc-150">sequence</span></span> | <span data-ttu-id="387cc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="387cc-151">Int32</span></span> | <span data-ttu-id="387cc-152">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="387cc-152">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="387cc-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="387cc-153">Response</span></span>
<span data-ttu-id="387cc-154">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="387cc-154">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="387cc-155">Пример</span><span class="sxs-lookup"><span data-stu-id="387cc-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="387cc-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="387cc-156">Request</span></span>
<span data-ttu-id="387cc-157">В приведенном ниже примере меняется имя правила, а также действия, выполняемые с этим правилом в [примере](messagerule-get.md#example) [получения правила](messagerule-get.md), — вместо пересылки на указанный адрес устанавливается высокая важность.</span><span class="sxs-lookup"><span data-stu-id="387cc-157">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 
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
##### <a name="response"></a><span data-ttu-id="387cc-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="387cc-158">Response</span></span>
<span data-ttu-id="387cc-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="387cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->