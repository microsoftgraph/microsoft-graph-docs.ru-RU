---
title: Создание правила
description: 'Создает объект messageRule, определяя набор условий и действий. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 2d42db335a8e08e813081b51c9ffdd055cb8860a
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266656"
---
# <a name="create-rule"></a><span data-ttu-id="6f23e-103">Создание правила</span><span class="sxs-lookup"><span data-stu-id="6f23e-103">Create rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f23e-104">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="6f23e-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="6f23e-105">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="6f23e-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="6f23e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6f23e-106">Permissions</span></span>
<span data-ttu-id="6f23e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f23e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f23e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f23e-109">Permission type</span></span>      | <span data-ttu-id="6f23e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f23e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f23e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f23e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6f23e-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f23e-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6f23e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f23e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f23e-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f23e-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="6f23e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f23e-115">Application</span></span> | <span data-ttu-id="6f23e-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6f23e-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="6f23e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f23e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="6f23e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f23e-118">Request headers</span></span>
| <span data-ttu-id="6f23e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6f23e-119">Name</span></span>       | <span data-ttu-id="6f23e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6f23e-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6f23e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f23e-121">Authorization</span></span>  | <span data-ttu-id="6f23e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f23e-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="6f23e-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6f23e-124">Request body</span></span>
<span data-ttu-id="6f23e-125">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="6f23e-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="6f23e-126">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="6f23e-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="6f23e-127">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="6f23e-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="6f23e-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="6f23e-128">Parameter</span></span>       | <span data-ttu-id="6f23e-129">Тип</span><span class="sxs-lookup"><span data-stu-id="6f23e-129">Type</span></span>|<span data-ttu-id="6f23e-130">Описание</span><span class="sxs-lookup"><span data-stu-id="6f23e-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="6f23e-131">actions</span><span class="sxs-lookup"><span data-stu-id="6f23e-131">actions</span></span>|[<span data-ttu-id="6f23e-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="6f23e-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="6f23e-133">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="6f23e-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="6f23e-134">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6f23e-134">Required.</span></span>|
|<span data-ttu-id="6f23e-135">conditions</span><span class="sxs-lookup"><span data-stu-id="6f23e-135">conditions</span></span>|[<span data-ttu-id="6f23e-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="6f23e-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="6f23e-137">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="6f23e-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="6f23e-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="6f23e-138">Optional.</span></span>|
|<span data-ttu-id="6f23e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="6f23e-139">displayName</span></span>| <span data-ttu-id="6f23e-140">String</span><span class="sxs-lookup"><span data-stu-id="6f23e-140">String</span></span>  | <span data-ttu-id="6f23e-141">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="6f23e-141">The display name of the rule.</span></span> <span data-ttu-id="6f23e-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="6f23e-142">Required.</span></span>|
|<span data-ttu-id="6f23e-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="6f23e-143">exceptions</span></span>| [<span data-ttu-id="6f23e-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="6f23e-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="6f23e-145">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="6f23e-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="6f23e-146">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="6f23e-146">Optional.</span></span> |
|<span data-ttu-id="6f23e-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="6f23e-147">isEnabled</span></span> | <span data-ttu-id="6f23e-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="6f23e-148">Boolean</span></span> | <span data-ttu-id="6f23e-149">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="6f23e-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="6f23e-150">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="6f23e-150">Optional.</span></span> |
|<span data-ttu-id="6f23e-151">sequence</span><span class="sxs-lookup"><span data-stu-id="6f23e-151">sequence</span></span>| <span data-ttu-id="6f23e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6f23e-152">Int32</span></span> | <span data-ttu-id="6f23e-153">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="6f23e-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="6f23e-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6f23e-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="6f23e-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f23e-155">Response</span></span>
<span data-ttu-id="6f23e-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6f23e-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f23e-157">Пример</span><span class="sxs-lookup"><span data-stu-id="6f23e-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6f23e-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f23e-158">Request</span></span>
<span data-ttu-id="6f23e-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f23e-159">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_mailfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/mailFolders/inbox/messagerules
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
##### <a name="response"></a><span data-ttu-id="6f23e-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="6f23e-160">Response</span></span>
<span data-ttu-id="6f23e-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6f23e-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="6f23e-164">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="6f23e-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="6f23e-165">C#</span><span class="sxs-lookup"><span data-stu-id="6f23e-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6f23e-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="6f23e-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6f23e-167">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6f23e-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
