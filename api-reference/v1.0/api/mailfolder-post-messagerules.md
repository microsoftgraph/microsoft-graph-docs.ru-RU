---
title: Создание правила
description: 'Создает объект messageRule, определяя набор условий и действий. '
author: angelgolfer-ms
ms.openlocfilehash: 72c4991e077364514104d5bbc8e24625526bce51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361357"
---
# <a name="create-rule"></a><span data-ttu-id="b4b14-103">Создание правила</span><span class="sxs-lookup"><span data-stu-id="b4b14-103">Create rule</span></span>


<span data-ttu-id="b4b14-104">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="b4b14-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="b4b14-105">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="b4b14-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="b4b14-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4b14-106">Permissions</span></span>
<span data-ttu-id="b4b14-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4b14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4b14-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4b14-109">Permission type</span></span>      | <span data-ttu-id="b4b14-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4b14-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4b14-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4b14-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b4b14-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4b14-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b4b14-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4b14-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4b14-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4b14-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="b4b14-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4b14-115">Application</span></span> | <span data-ttu-id="b4b14-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4b14-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="b4b14-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4b14-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="b4b14-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4b14-118">Request headers</span></span>
| <span data-ttu-id="b4b14-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b4b14-119">Name</span></span>       | <span data-ttu-id="b4b14-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b4b14-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b4b14-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4b14-121">Authorization</span></span>  | <span data-ttu-id="b4b14-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4b14-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="b4b14-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4b14-124">Request body</span></span>
<span data-ttu-id="b4b14-125">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="b4b14-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="b4b14-126">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="b4b14-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="b4b14-127">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="b4b14-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="b4b14-128">Имя</span><span class="sxs-lookup"><span data-stu-id="b4b14-128">Name</span></span>       | <span data-ttu-id="b4b14-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b4b14-129">Type</span></span>|<span data-ttu-id="b4b14-130">Описание</span><span class="sxs-lookup"><span data-stu-id="b4b14-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="b4b14-131">actions</span><span class="sxs-lookup"><span data-stu-id="b4b14-131">actions</span></span>|[<span data-ttu-id="b4b14-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="b4b14-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="b4b14-133">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="b4b14-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="b4b14-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4b14-134">Required.</span></span>|
|<span data-ttu-id="b4b14-135">conditions</span><span class="sxs-lookup"><span data-stu-id="b4b14-135">conditions</span></span>|[<span data-ttu-id="b4b14-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="b4b14-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="b4b14-137">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="b4b14-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="b4b14-138">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b4b14-138">Optional.</span></span>|
|<span data-ttu-id="b4b14-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b4b14-139">displayName</span></span>| <span data-ttu-id="b4b14-140">Строка</span><span class="sxs-lookup"><span data-stu-id="b4b14-140">String</span></span>  | <span data-ttu-id="b4b14-141">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="b4b14-141">The display name of the rule.</span></span> <span data-ttu-id="b4b14-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4b14-142">Required.</span></span>|
|<span data-ttu-id="b4b14-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="b4b14-143">exceptions</span></span>| [<span data-ttu-id="b4b14-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="b4b14-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="b4b14-145">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="b4b14-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="b4b14-146">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b4b14-146">Optional.</span></span> |
|<span data-ttu-id="b4b14-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b4b14-147">isEnabled</span></span> | <span data-ttu-id="b4b14-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4b14-148">Boolean</span></span> | <span data-ttu-id="b4b14-149">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="b4b14-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="b4b14-150">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b4b14-150">Optional.</span></span> |
|<span data-ttu-id="b4b14-151">sequence</span><span class="sxs-lookup"><span data-stu-id="b4b14-151">sequence</span></span>| <span data-ttu-id="b4b14-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b4b14-152">Int32</span></span> | <span data-ttu-id="b4b14-153">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="b4b14-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="b4b14-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4b14-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="b4b14-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4b14-155">Response</span></span>
<span data-ttu-id="b4b14-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b4b14-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4b14-157">Пример</span><span class="sxs-lookup"><span data-stu-id="b4b14-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4b14-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4b14-158">Request</span></span>
<span data-ttu-id="b4b14-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b4b14-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="b4b14-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="b4b14-160">Response</span></span>
<span data-ttu-id="b4b14-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="b4b14-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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