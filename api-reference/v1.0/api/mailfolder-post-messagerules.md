---
title: Создание правила
description: 'Создает объект messageRule, определяя набор условий и действий. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 60bef0945544ae4f47ab8fe22e4304d32a6203da
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374927"
---
# <a name="create-rule"></a><span data-ttu-id="d50da-103">Создание правила</span><span class="sxs-lookup"><span data-stu-id="d50da-103">Create rule</span></span>


<span data-ttu-id="d50da-104">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="d50da-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="d50da-105">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="d50da-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="d50da-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d50da-106">Permissions</span></span>
<span data-ttu-id="d50da-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d50da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d50da-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d50da-109">Permission type</span></span>      | <span data-ttu-id="d50da-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d50da-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d50da-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d50da-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d50da-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d50da-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d50da-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d50da-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d50da-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d50da-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d50da-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d50da-115">Application</span></span> | <span data-ttu-id="d50da-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d50da-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="d50da-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d50da-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="d50da-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d50da-118">Request headers</span></span>
| <span data-ttu-id="d50da-119">Имя</span><span class="sxs-lookup"><span data-stu-id="d50da-119">Name</span></span>       | <span data-ttu-id="d50da-120">Описание</span><span class="sxs-lookup"><span data-stu-id="d50da-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d50da-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d50da-121">Authorization</span></span>  | <span data-ttu-id="d50da-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d50da-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d50da-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d50da-124">Request body</span></span>
<span data-ttu-id="d50da-125">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="d50da-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="d50da-126">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="d50da-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="d50da-127">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="d50da-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="d50da-128">Имя</span><span class="sxs-lookup"><span data-stu-id="d50da-128">Name</span></span>       | <span data-ttu-id="d50da-129">Тип</span><span class="sxs-lookup"><span data-stu-id="d50da-129">Type</span></span>|<span data-ttu-id="d50da-130">Описание</span><span class="sxs-lookup"><span data-stu-id="d50da-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="d50da-131">actions</span><span class="sxs-lookup"><span data-stu-id="d50da-131">actions</span></span>|[<span data-ttu-id="d50da-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="d50da-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="d50da-133">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="d50da-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="d50da-134">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d50da-134">Required.</span></span>|
|<span data-ttu-id="d50da-135">conditions</span><span class="sxs-lookup"><span data-stu-id="d50da-135">conditions</span></span>|[<span data-ttu-id="d50da-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="d50da-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="d50da-137">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="d50da-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="d50da-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d50da-138">Optional.</span></span>|
|<span data-ttu-id="d50da-139">displayName</span><span class="sxs-lookup"><span data-stu-id="d50da-139">displayName</span></span>| <span data-ttu-id="d50da-140">String</span><span class="sxs-lookup"><span data-stu-id="d50da-140">String</span></span>  | <span data-ttu-id="d50da-141">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="d50da-141">The display name of the rule.</span></span> <span data-ttu-id="d50da-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="d50da-142">Required.</span></span>|
|<span data-ttu-id="d50da-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="d50da-143">exceptions</span></span>| [<span data-ttu-id="d50da-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="d50da-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="d50da-145">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="d50da-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="d50da-146">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d50da-146">Optional.</span></span> |
|<span data-ttu-id="d50da-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d50da-147">isEnabled</span></span> | <span data-ttu-id="d50da-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d50da-148">Boolean</span></span> | <span data-ttu-id="d50da-149">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="d50da-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="d50da-150">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="d50da-150">Optional.</span></span> |
|<span data-ttu-id="d50da-151">sequence</span><span class="sxs-lookup"><span data-stu-id="d50da-151">sequence</span></span>| <span data-ttu-id="d50da-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d50da-152">Int32</span></span> | <span data-ttu-id="d50da-153">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="d50da-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="d50da-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d50da-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="d50da-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="d50da-155">Response</span></span>
<span data-ttu-id="d50da-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d50da-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d50da-157">Пример</span><span class="sxs-lookup"><span data-stu-id="d50da-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d50da-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="d50da-158">Request</span></span>
<span data-ttu-id="d50da-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d50da-159">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d50da-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="d50da-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox"],
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules
Content-type: application/json

{      
    "displayName": "From partner",      
    "sequence": 2,      
    "isEnabled": true,          
    "conditions": {
        "senderContains": [
          "adele"       
        ]
     },
     "actions": {
        "forwardTo": [
          {
             "emailAddress": {
                "name": "Alex Wilbur",
                "address": "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        "stopProcessingRules": true
     }    
}

```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d50da-161">C#</span><span class="sxs-lookup"><span data-stu-id="d50da-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-messagerule-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d50da-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d50da-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-messagerule-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d50da-163">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d50da-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-messagerule-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d50da-164">Java</span><span class="sxs-lookup"><span data-stu-id="d50da-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-messagerule-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d50da-165">Отклик</span><span class="sxs-lookup"><span data-stu-id="d50da-165">Response</span></span>
<span data-ttu-id="d50da-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d50da-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id":"AQAAAJ5dZqA=",
  "displayName":"From partner",
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
      "stopProcessingRules":true,
      "forwardTo":[
        {
          "emailAddress":{
            "name":"Alex Wilbur",
            "address":"AlexW@contoso.onmicrosoft.com"
          }
        }
      ]
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
