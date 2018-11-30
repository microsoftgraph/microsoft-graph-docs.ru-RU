---
title: Создание правила
description: 'Создает объект messageRule, определяя набор условий и действий. '
ms.openlocfilehash: f725aa0a078938cf111782aedf1feb041a5a0e19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082567"
---
# <a name="create-rule"></a><span data-ttu-id="20661-103">Создание правила</span><span class="sxs-lookup"><span data-stu-id="20661-103">Create rule</span></span>

> <span data-ttu-id="20661-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20661-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20661-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20661-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20661-106">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="20661-106">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="20661-107">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="20661-107">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="20661-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="20661-108">Permissions</span></span>
<span data-ttu-id="20661-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20661-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20661-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20661-111">Permission type</span></span>      | <span data-ttu-id="20661-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="20661-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="20661-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20661-113">Delegated (work or school account)</span></span> | <span data-ttu-id="20661-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20661-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="20661-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20661-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20661-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20661-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="20661-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20661-117">Application</span></span> | <span data-ttu-id="20661-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="20661-118">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="20661-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20661-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="20661-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20661-120">Request headers</span></span>
| <span data-ttu-id="20661-121">Имя</span><span class="sxs-lookup"><span data-stu-id="20661-121">Name</span></span>       | <span data-ttu-id="20661-122">Описание</span><span class="sxs-lookup"><span data-stu-id="20661-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20661-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20661-123">Authorization</span></span>  | <span data-ttu-id="20661-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20661-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="20661-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="20661-126">Request body</span></span>
<span data-ttu-id="20661-127">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="20661-127">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="20661-128">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="20661-128">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="20661-129">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="20661-129">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="20661-130">Параметр</span><span class="sxs-lookup"><span data-stu-id="20661-130">Parameter</span></span>       | <span data-ttu-id="20661-131">Тип</span><span class="sxs-lookup"><span data-stu-id="20661-131">Type</span></span>|<span data-ttu-id="20661-132">Описание</span><span class="sxs-lookup"><span data-stu-id="20661-132">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="20661-133">actions</span><span class="sxs-lookup"><span data-stu-id="20661-133">actions</span></span>|[<span data-ttu-id="20661-134">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="20661-134">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="20661-135">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="20661-135">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="20661-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20661-136">Required.</span></span>|
|<span data-ttu-id="20661-137">conditions</span><span class="sxs-lookup"><span data-stu-id="20661-137">conditions</span></span>|[<span data-ttu-id="20661-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="20661-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="20661-139">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="20661-139">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="20661-140">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="20661-140">Optional.</span></span>|
|<span data-ttu-id="20661-141">displayName</span><span class="sxs-lookup"><span data-stu-id="20661-141">displayName</span></span>| <span data-ttu-id="20661-142">String</span><span class="sxs-lookup"><span data-stu-id="20661-142">String</span></span>  | <span data-ttu-id="20661-143">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="20661-143">The display name of the rule.</span></span> <span data-ttu-id="20661-144">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20661-144">Required.</span></span>|
|<span data-ttu-id="20661-145">exceptions</span><span class="sxs-lookup"><span data-stu-id="20661-145">exceptions</span></span>| [<span data-ttu-id="20661-146">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="20661-146">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="20661-147">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="20661-147">Represents exception conditions for the rule.</span></span> <span data-ttu-id="20661-148">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="20661-148">Optional.</span></span> |
|<span data-ttu-id="20661-149">isEnabled</span><span class="sxs-lookup"><span data-stu-id="20661-149">isEnabled</span></span> | <span data-ttu-id="20661-150">Логический</span><span class="sxs-lookup"><span data-stu-id="20661-150">Boolean</span></span> | <span data-ttu-id="20661-151">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="20661-151">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="20661-152">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="20661-152">Optional.</span></span> |
|<span data-ttu-id="20661-153">sequence</span><span class="sxs-lookup"><span data-stu-id="20661-153">sequence</span></span>| <span data-ttu-id="20661-154">Int32</span><span class="sxs-lookup"><span data-stu-id="20661-154">Int32</span></span> | <span data-ttu-id="20661-155">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="20661-155">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="20661-156">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="20661-156">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="20661-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="20661-157">Response</span></span>
<span data-ttu-id="20661-158">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="20661-158">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20661-159">Пример</span><span class="sxs-lookup"><span data-stu-id="20661-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20661-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="20661-160">Request</span></span>
<span data-ttu-id="20661-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20661-161">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="20661-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="20661-162">Response</span></span>
<span data-ttu-id="20661-p111">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="20661-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->