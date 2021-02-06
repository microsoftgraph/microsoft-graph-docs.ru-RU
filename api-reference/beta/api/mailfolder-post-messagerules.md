---
title: Создание правила
description: 'Создает объект messageRule, определяя набор условий и действий. '
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9fc98fd56e958a558a9f5afc6dec72412e35a6d1
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134738"
---
# <a name="create-rule"></a><span data-ttu-id="45fda-103">Создание правила</span><span class="sxs-lookup"><span data-stu-id="45fda-103">Create rule</span></span>

<span data-ttu-id="45fda-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45fda-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45fda-105">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="45fda-105">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="45fda-106">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="45fda-106">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="45fda-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45fda-107">Permissions</span></span>
<span data-ttu-id="45fda-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45fda-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45fda-110">Permission type</span></span>      | <span data-ttu-id="45fda-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45fda-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45fda-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45fda-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45fda-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45fda-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="45fda-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45fda-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45fda-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45fda-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="45fda-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45fda-116">Application</span></span> | <span data-ttu-id="45fda-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45fda-117">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="45fda-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45fda-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="45fda-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45fda-119">Request headers</span></span>
| <span data-ttu-id="45fda-120">Имя</span><span class="sxs-lookup"><span data-stu-id="45fda-120">Name</span></span>       | <span data-ttu-id="45fda-121">Описание</span><span class="sxs-lookup"><span data-stu-id="45fda-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45fda-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45fda-122">Authorization</span></span>  | <span data-ttu-id="45fda-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45fda-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="45fda-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="45fda-125">Request body</span></span>
<span data-ttu-id="45fda-126">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="45fda-126">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="45fda-127">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="45fda-127">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="45fda-128">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="45fda-128">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="45fda-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="45fda-129">Parameter</span></span>       | <span data-ttu-id="45fda-130">Тип</span><span class="sxs-lookup"><span data-stu-id="45fda-130">Type</span></span>|<span data-ttu-id="45fda-131">Описание</span><span class="sxs-lookup"><span data-stu-id="45fda-131">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="45fda-132">actions</span><span class="sxs-lookup"><span data-stu-id="45fda-132">actions</span></span>|[<span data-ttu-id="45fda-133">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="45fda-133">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="45fda-134">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="45fda-134">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="45fda-135">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45fda-135">Required.</span></span>|
|<span data-ttu-id="45fda-136">conditions</span><span class="sxs-lookup"><span data-stu-id="45fda-136">conditions</span></span>|[<span data-ttu-id="45fda-137">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="45fda-137">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="45fda-138">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="45fda-138">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="45fda-139">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="45fda-139">Optional.</span></span>|
|<span data-ttu-id="45fda-140">displayName</span><span class="sxs-lookup"><span data-stu-id="45fda-140">displayName</span></span>| <span data-ttu-id="45fda-141">Строка</span><span class="sxs-lookup"><span data-stu-id="45fda-141">String</span></span>  | <span data-ttu-id="45fda-142">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="45fda-142">The display name of the rule.</span></span> <span data-ttu-id="45fda-143">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45fda-143">Required.</span></span>|
|<span data-ttu-id="45fda-144">exceptions</span><span class="sxs-lookup"><span data-stu-id="45fda-144">exceptions</span></span>| [<span data-ttu-id="45fda-145">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="45fda-145">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="45fda-146">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="45fda-146">Represents exception conditions for the rule.</span></span> <span data-ttu-id="45fda-147">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="45fda-147">Optional.</span></span> |
|<span data-ttu-id="45fda-148">isEnabled</span><span class="sxs-lookup"><span data-stu-id="45fda-148">isEnabled</span></span> | <span data-ttu-id="45fda-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="45fda-149">Boolean</span></span> | <span data-ttu-id="45fda-150">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="45fda-150">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="45fda-151">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="45fda-151">Optional.</span></span> |
|<span data-ttu-id="45fda-152">sequence</span><span class="sxs-lookup"><span data-stu-id="45fda-152">sequence</span></span>| <span data-ttu-id="45fda-153">Int32</span><span class="sxs-lookup"><span data-stu-id="45fda-153">Int32</span></span> | <span data-ttu-id="45fda-154">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="45fda-154">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="45fda-155">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45fda-155">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="45fda-156">Отклик</span><span class="sxs-lookup"><span data-stu-id="45fda-156">Response</span></span>
<span data-ttu-id="45fda-157">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="45fda-157">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45fda-158">Пример</span><span class="sxs-lookup"><span data-stu-id="45fda-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="45fda-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="45fda-159">Request</span></span>
<span data-ttu-id="45fda-160">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45fda-160">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="45fda-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="45fda-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="45fda-162">C#</span><span class="sxs-lookup"><span data-stu-id="45fda-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-messagerule-from-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45fda-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45fda-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-messagerule-from-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45fda-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45fda-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-messagerule-from-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45fda-165">Java</span><span class="sxs-lookup"><span data-stu-id="45fda-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-messagerule-from-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="45fda-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="45fda-166">Response</span></span>
<span data-ttu-id="45fda-p110">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45fda-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


