---
title: Создание правила
description: 'Создает объект messageRule, определяя набор условий и действий. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f2c06fce207728af6d89b5284eda2458d9b65438
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540697"
---
# <a name="create-rule"></a><span data-ttu-id="e8644-103">Создание правила</span><span class="sxs-lookup"><span data-stu-id="e8644-103">Create rule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8644-104">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="e8644-104">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="e8644-105">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="e8644-105">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8644-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e8644-106">Permissions</span></span>
<span data-ttu-id="e8644-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8644-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e8644-109">Permission type</span></span>      | <span data-ttu-id="e8644-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e8644-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8644-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e8644-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e8644-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8644-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e8644-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e8644-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8644-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8644-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="e8644-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e8644-115">Application</span></span> | <span data-ttu-id="e8644-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8644-116">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="e8644-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e8644-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messagerules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messagerules
```
## <a name="request-headers"></a><span data-ttu-id="e8644-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e8644-118">Request headers</span></span>
| <span data-ttu-id="e8644-119">Имя</span><span class="sxs-lookup"><span data-stu-id="e8644-119">Name</span></span>       | <span data-ttu-id="e8644-120">Описание</span><span class="sxs-lookup"><span data-stu-id="e8644-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e8644-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e8644-121">Authorization</span></span>  | <span data-ttu-id="e8644-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8644-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="e8644-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e8644-124">Request body</span></span>
<span data-ttu-id="e8644-125">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="e8644-125">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="e8644-126">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="e8644-126">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="e8644-127">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="e8644-127">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

| <span data-ttu-id="e8644-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="e8644-128">Parameter</span></span>       | <span data-ttu-id="e8644-129">Тип</span><span class="sxs-lookup"><span data-stu-id="e8644-129">Type</span></span>|<span data-ttu-id="e8644-130">Описание</span><span class="sxs-lookup"><span data-stu-id="e8644-130">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="e8644-131">actions</span><span class="sxs-lookup"><span data-stu-id="e8644-131">actions</span></span>|[<span data-ttu-id="e8644-132">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="e8644-132">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="e8644-133">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="e8644-133">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="e8644-134">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8644-134">Required.</span></span>|
|<span data-ttu-id="e8644-135">conditions</span><span class="sxs-lookup"><span data-stu-id="e8644-135">conditions</span></span>|[<span data-ttu-id="e8644-136">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e8644-136">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="e8644-137">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="e8644-137">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="e8644-138">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e8644-138">Optional.</span></span>|
|<span data-ttu-id="e8644-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e8644-139">displayName</span></span>| <span data-ttu-id="e8644-140">String</span><span class="sxs-lookup"><span data-stu-id="e8644-140">String</span></span>  | <span data-ttu-id="e8644-141">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="e8644-141">The display name of the rule.</span></span> <span data-ttu-id="e8644-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8644-142">Required.</span></span>|
|<span data-ttu-id="e8644-143">exceptions</span><span class="sxs-lookup"><span data-stu-id="e8644-143">exceptions</span></span>| [<span data-ttu-id="e8644-144">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="e8644-144">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="e8644-145">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="e8644-145">Represents exception conditions for the rule.</span></span> <span data-ttu-id="e8644-146">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="e8644-146">Optional.</span></span> |
|<span data-ttu-id="e8644-147">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e8644-147">isEnabled</span></span> | <span data-ttu-id="e8644-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="e8644-148">Boolean</span></span> | <span data-ttu-id="e8644-149">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="e8644-149">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="e8644-150">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="e8644-150">Optional.</span></span> |
|<span data-ttu-id="e8644-151">sequence</span><span class="sxs-lookup"><span data-stu-id="e8644-151">sequence</span></span>| <span data-ttu-id="e8644-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e8644-152">Int32</span></span> | <span data-ttu-id="e8644-153">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="e8644-153">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="e8644-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e8644-154">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="e8644-155">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8644-155">Response</span></span>
<span data-ttu-id="e8644-156">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e8644-156">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8644-157">Пример</span><span class="sxs-lookup"><span data-stu-id="e8644-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8644-158">Запрос</span><span class="sxs-lookup"><span data-stu-id="e8644-158">Request</span></span>
<span data-ttu-id="e8644-159">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e8644-159">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e8644-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="e8644-160">Response</span></span>
<span data-ttu-id="e8644-p110">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e8644-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/mailfolder-post-messagerules.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
