---
title: Создание правила
description: 'Создает объект messageRule, определяя набор условий и действий. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c1c8470e7d82f6898fc4895d9ddb27eef254638a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612285"
---
# <a name="create-rule"></a><span data-ttu-id="b55be-103">Создание правила</span><span class="sxs-lookup"><span data-stu-id="b55be-103">Create rule</span></span>


<span data-ttu-id="b55be-104">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="b55be-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="b55be-105">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="b55be-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="b55be-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b55be-106">Permissions</span></span>
<span data-ttu-id="b55be-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b55be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b55be-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b55be-109">Permission type</span></span>      | <span data-ttu-id="b55be-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b55be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b55be-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b55be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b55be-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b55be-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b55be-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b55be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b55be-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b55be-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b55be-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b55be-115">Application</span></span> | <span data-ttu-id="b55be-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b55be-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="b55be-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b55be-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="b55be-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b55be-118">Request headers</span></span>
| <span data-ttu-id="b55be-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b55be-119">Name</span></span>       | <span data-ttu-id="b55be-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b55be-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b55be-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b55be-121">Authorization</span></span>  | <span data-ttu-id="b55be-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b55be-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b55be-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b55be-124">Request body</span></span>
<span data-ttu-id="b55be-125">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="b55be-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="b55be-126">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="b55be-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="b55be-127">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="b55be-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="b55be-128">Имя</span><span class="sxs-lookup"><span data-stu-id="b55be-128">Name</span></span>       | <span data-ttu-id="b55be-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b55be-129">Type</span></span>|<span data-ttu-id="b55be-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b55be-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="b55be-131">actions</span><span class="sxs-lookup"><span data-stu-id="b55be-131">actions</span></span>|[<span data-ttu-id="b55be-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="b55be-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="b55be-133">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="b55be-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="b55be-134">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b55be-134">Required.</span></span>|
|<span data-ttu-id="b55be-135">conditions</span><span class="sxs-lookup"><span data-stu-id="b55be-135">conditions</span></span>|[<span data-ttu-id="b55be-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="b55be-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="b55be-137">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="b55be-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="b55be-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b55be-138">Optional.</span></span>|
|<span data-ttu-id="b55be-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b55be-139">displayName</span></span>| <span data-ttu-id="b55be-140">String</span><span class="sxs-lookup"><span data-stu-id="b55be-140">String</span></span>  | <span data-ttu-id="b55be-141">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="b55be-141">The display name of the rule.</span></span> <span data-ttu-id="b55be-142">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="b55be-142">Required.</span></span>|
|<span data-ttu-id="b55be-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="b55be-143">exceptions</span></span>| [<span data-ttu-id="b55be-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="b55be-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="b55be-145">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="b55be-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="b55be-146">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="b55be-146">Optional.</span></span> |
|<span data-ttu-id="b55be-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b55be-147">isEnabled</span></span> | <span data-ttu-id="b55be-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="b55be-148">Boolean</span></span> | <span data-ttu-id="b55be-149">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="b55be-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="b55be-150">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b55be-150">Optional.</span></span> |
|<span data-ttu-id="b55be-151">sequence</span><span class="sxs-lookup"><span data-stu-id="b55be-151">sequence</span></span>| <span data-ttu-id="b55be-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b55be-152">Int32</span></span> | <span data-ttu-id="b55be-153">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="b55be-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="b55be-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b55be-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="b55be-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b55be-155">Response</span></span>
<span data-ttu-id="b55be-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b55be-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b55be-157">Пример</span><span class="sxs-lookup"><span data-stu-id="b55be-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b55be-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="b55be-158">Request</span></span>
<span data-ttu-id="b55be-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b55be-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b55be-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="b55be-160">Response</span></span>
<span data-ttu-id="b55be-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b55be-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="b55be-164">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="b55be-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="b55be-165">Языках</span><span class="sxs-lookup"><span data-stu-id="b55be-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b55be-166">Язык</span><span class="sxs-lookup"><span data-stu-id="b55be-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_messagerule_from_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-post-messagerules.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
