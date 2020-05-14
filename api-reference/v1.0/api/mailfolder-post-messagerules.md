---
title: Создание правила
description: 'Создает объект messageRule, определяя набор условий и действий. '
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9525480d123aa2689ed2ae05b3766d35aa4aec53
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43361972"
---
# <a name="create-rule"></a><span data-ttu-id="b410b-103">Создание правила</span><span class="sxs-lookup"><span data-stu-id="b410b-103">Create rule</span></span>

<span data-ttu-id="b410b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b410b-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="b410b-105">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="b410b-105">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="b410b-106">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="b410b-106">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="b410b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b410b-107">Permissions</span></span>
<span data-ttu-id="b410b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b410b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b410b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b410b-110">Permission type</span></span>      | <span data-ttu-id="b410b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b410b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b410b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b410b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b410b-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b410b-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b410b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b410b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b410b-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b410b-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b410b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b410b-116">Application</span></span> | <span data-ttu-id="b410b-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b410b-117">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="b410b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b410b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="b410b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b410b-119">Request headers</span></span>
| <span data-ttu-id="b410b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="b410b-120">Name</span></span>       | <span data-ttu-id="b410b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="b410b-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b410b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b410b-122">Authorization</span></span>  | <span data-ttu-id="b410b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b410b-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b410b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b410b-125">Request body</span></span>
<span data-ttu-id="b410b-126">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="b410b-126">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="b410b-127">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="b410b-127">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="b410b-128">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="b410b-128">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="b410b-129">Имя</span><span class="sxs-lookup"><span data-stu-id="b410b-129">Name</span></span>       | <span data-ttu-id="b410b-130">Тип</span><span class="sxs-lookup"><span data-stu-id="b410b-130">Type</span></span>|<span data-ttu-id="b410b-131">Описание</span><span class="sxs-lookup"><span data-stu-id="b410b-131">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="b410b-132">actions</span><span class="sxs-lookup"><span data-stu-id="b410b-132">actions</span></span>|[<span data-ttu-id="b410b-133">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="b410b-133">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="b410b-134">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="b410b-134">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="b410b-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b410b-135">Required.</span></span>|
|<span data-ttu-id="b410b-136">conditions</span><span class="sxs-lookup"><span data-stu-id="b410b-136">conditions</span></span>|[<span data-ttu-id="b410b-137">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="b410b-137">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="b410b-138">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="b410b-138">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="b410b-139">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b410b-139">Optional.</span></span>|
|<span data-ttu-id="b410b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="b410b-140">displayName</span></span>| <span data-ttu-id="b410b-141">String</span><span class="sxs-lookup"><span data-stu-id="b410b-141">String</span></span>  | <span data-ttu-id="b410b-142">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="b410b-142">The display name of the rule.</span></span> <span data-ttu-id="b410b-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b410b-143">Required.</span></span>|
|<span data-ttu-id="b410b-144">exceptions</span><span class="sxs-lookup"><span data-stu-id="b410b-144">exceptions</span></span>| [<span data-ttu-id="b410b-145">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="b410b-145">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="b410b-146">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="b410b-146">Represents exception conditions for the rule.</span></span> <span data-ttu-id="b410b-147">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b410b-147">Optional.</span></span> |
|<span data-ttu-id="b410b-148">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b410b-148">isEnabled</span></span> | <span data-ttu-id="b410b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b410b-149">Boolean</span></span> | <span data-ttu-id="b410b-150">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="b410b-150">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="b410b-151">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b410b-151">Optional.</span></span> |
|<span data-ttu-id="b410b-152">sequence</span><span class="sxs-lookup"><span data-stu-id="b410b-152">sequence</span></span>| <span data-ttu-id="b410b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b410b-153">Int32</span></span> | <span data-ttu-id="b410b-154">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="b410b-154">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="b410b-155">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b410b-155">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="b410b-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="b410b-156">Response</span></span>
<span data-ttu-id="b410b-157">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b410b-157">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b410b-158">Пример</span><span class="sxs-lookup"><span data-stu-id="b410b-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b410b-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="b410b-159">Request</span></span>
<span data-ttu-id="b410b-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b410b-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b410b-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="b410b-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="b410b-162">C#</span><span class="sxs-lookup"><span data-stu-id="b410b-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-messagerule-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b410b-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b410b-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-messagerule-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b410b-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b410b-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-messagerule-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b410b-165">Java</span><span class="sxs-lookup"><span data-stu-id="b410b-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-messagerule-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b410b-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="b410b-166">Response</span></span>
<span data-ttu-id="b410b-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b410b-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
