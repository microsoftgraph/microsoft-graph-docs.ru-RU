---
title: Обновление правила
description: Изменение записываемых свойств объекта messageRule и сохранение изменений.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: db0bd06dfe4ae65e977f5489939178a8eda664f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914544"
---
# <a name="update-rule"></a><span data-ttu-id="f7894-103">Обновление правила</span><span class="sxs-lookup"><span data-stu-id="f7894-103">Update rule</span></span>


<span data-ttu-id="f7894-104">Изменение записываемых свойств объекта [messageRule](../resources/messagerule.md) и сохранение изменений.</span><span class="sxs-lookup"><span data-stu-id="f7894-104">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7894-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f7894-105">Permissions</span></span>
<span data-ttu-id="f7894-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7894-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7894-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7894-108">Permission type</span></span>      | <span data-ttu-id="f7894-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7894-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7894-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7894-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7894-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7894-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f7894-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7894-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7894-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7894-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="f7894-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7894-114">Application</span></span> | <span data-ttu-id="f7894-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f7894-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7894-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7894-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messageRules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="f7894-117">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f7894-117">Optional request headers</span></span>
| <span data-ttu-id="f7894-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f7894-118">Name</span></span>       | <span data-ttu-id="f7894-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f7894-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f7894-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f7894-120">Authorization</span></span>  | <span data-ttu-id="f7894-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7894-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f7894-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7894-123">Request body</span></span>
<span data-ttu-id="f7894-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="f7894-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f7894-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7894-127">Property</span></span>     | <span data-ttu-id="f7894-128">Тип</span><span class="sxs-lookup"><span data-stu-id="f7894-128">Type</span></span>   |<span data-ttu-id="f7894-129">Описание</span><span class="sxs-lookup"><span data-stu-id="f7894-129">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f7894-130">actions</span><span class="sxs-lookup"><span data-stu-id="f7894-130">actions</span></span> | [<span data-ttu-id="f7894-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="f7894-131">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="f7894-132">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="f7894-132">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="f7894-133">conditions</span><span class="sxs-lookup"><span data-stu-id="f7894-133">conditions</span></span> | [<span data-ttu-id="f7894-134">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="f7894-134">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="f7894-135">Условия, при соблюдении которых с указанным правилом выполняются соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="f7894-135">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="f7894-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f7894-136">displayName</span></span> | <span data-ttu-id="f7894-137">Строка</span><span class="sxs-lookup"><span data-stu-id="f7894-137">String</span></span> | <span data-ttu-id="f7894-138">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="f7894-138">The display name of the rule.</span></span> |
| <span data-ttu-id="f7894-139">exceptions</span><span class="sxs-lookup"><span data-stu-id="f7894-139">exceptions</span></span> | [<span data-ttu-id="f7894-140">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="f7894-140">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="f7894-141">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="f7894-141">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="f7894-142">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f7894-142">isEnabled</span></span> | <span data-ttu-id="f7894-143">Логический</span><span class="sxs-lookup"><span data-stu-id="f7894-143">Boolean</span></span> | <span data-ttu-id="f7894-144">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="f7894-144">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="f7894-145">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="f7894-145">isReadOnly</span></span> | <span data-ttu-id="f7894-146">Логический</span><span class="sxs-lookup"><span data-stu-id="f7894-146">Boolean</span></span> | <span data-ttu-id="f7894-147">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="f7894-147">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="f7894-148">sequence</span><span class="sxs-lookup"><span data-stu-id="f7894-148">sequence</span></span> | <span data-ttu-id="f7894-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f7894-149">Int32</span></span> | <span data-ttu-id="f7894-150">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="f7894-150">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="f7894-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7894-151">Response</span></span>
<span data-ttu-id="f7894-152">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="f7894-152">If successful, this method returns a `200 OK` response code and updated [messageRule](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7894-153">Пример</span><span class="sxs-lookup"><span data-stu-id="f7894-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7894-154">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7894-154">Request</span></span>
<span data-ttu-id="f7894-155">В приведенном ниже примере меняется имя правила, а также действия, выполняемые с этим правилом в [примере](messagerule-get.md#example) [получения правила](messagerule-get.md), — вместо пересылки на указанный адрес устанавливается высокая важность.</span><span class="sxs-lookup"><span data-stu-id="f7894-155">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule-get.md#example) in [Get rule](messagerule-get.md), from forwarding to an address to marking its importance as high.</span></span> 
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
##### <a name="response"></a><span data-ttu-id="f7894-156">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7894-156">Response</span></span>
<span data-ttu-id="f7894-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7894-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
