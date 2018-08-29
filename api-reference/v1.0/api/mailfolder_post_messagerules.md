# <a name="create-rule"></a><span data-ttu-id="0ac9f-101">Создание правила</span><span class="sxs-lookup"><span data-stu-id="0ac9f-101">Create rule</span></span>


<span data-ttu-id="0ac9f-102">Создает объект [messageRule](../resources/messagerule.md), определяя набор условий и действий.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-102">Create a [messageRule](../resources/messagerule.md) object by specifying a set of conditions and actions.</span></span> 

<span data-ttu-id="0ac9f-103">Outlook выполняет эти действия, если входящее сообщение в папке "Входящие" пользователя соответствует указанным условиям.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-103">Outlook carries out those actions if an incoming message in the user's Inbox meets the specified conditions.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ac9f-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ac9f-104">Permissions</span></span>
<span data-ttu-id="0ac9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0ac9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0ac9f-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ac9f-107">Permission type</span></span>      | <span data-ttu-id="0ac9f-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ac9f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ac9f-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ac9f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="0ac9f-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ac9f-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0ac9f-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ac9f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ac9f-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ac9f-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0ac9f-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ac9f-113">Application</span></span> | <span data-ttu-id="0ac9f-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ac9f-114">MailboxSettings.ReadWrite</span></span> |


## <a name="http-request"></a><span data-ttu-id="0ac9f-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ac9f-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/mailFolders/inbox/messageRules
POST /users/{id | userPrincipalName}/mailFolders/inbox/messageRules
```
## <a name="request-headers"></a><span data-ttu-id="0ac9f-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ac9f-116">Request headers</span></span>
| <span data-ttu-id="0ac9f-117">Имя</span><span class="sxs-lookup"><span data-stu-id="0ac9f-117">Name</span></span>       | <span data-ttu-id="0ac9f-118">Описание</span><span class="sxs-lookup"><span data-stu-id="0ac9f-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ac9f-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ac9f-119">Authorization</span></span>  | <span data-ttu-id="0ac9f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="0ac9f-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ac9f-122">Request body</span></span>
<span data-ttu-id="0ac9f-123">В тексте запроса укажите параметры, применимые к вашему правилу.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-123">In the request body, supply the parameters that are applicable to your rule.</span></span> <span data-ttu-id="0ac9f-124">Ниже представлены параметры текста, которые обычно используются при создании правил.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-124">The following are body parameters that are typically used when creating rules.</span></span> <span data-ttu-id="0ac9f-125">Можно соответствующим образом указать любые другие записываемые свойства **messageRule** в тексте запроса.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-125">You can specify any other writable **messageRule** properties as appropriate in the request body.</span></span>

### <a name="request-parameters"></a><span data-ttu-id="0ac9f-126">Параметры запроса</span><span class="sxs-lookup"><span data-stu-id="0ac9f-126">Request parameters</span></span>
| <span data-ttu-id="0ac9f-127">Имя</span><span class="sxs-lookup"><span data-stu-id="0ac9f-127">Name</span></span>       | <span data-ttu-id="0ac9f-128">Тип</span><span class="sxs-lookup"><span data-stu-id="0ac9f-128">Type</span></span>|<span data-ttu-id="0ac9f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0ac9f-129">Description</span></span>|
|:--------|:-------|:----------|
|<span data-ttu-id="0ac9f-130">actions</span><span class="sxs-lookup"><span data-stu-id="0ac9f-130">actions</span></span>|[<span data-ttu-id="0ac9f-131">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="0ac9f-131">messageRuleActions</span></span>](../resources/messageruleactions.md)|<span data-ttu-id="0ac9f-132">Действия, применимые к сообщению при выполнении соответствующих условий (если таковые имеются).</span><span class="sxs-lookup"><span data-stu-id="0ac9f-132">Actions to be taken on a message when the corresponding conditions, if any, are fulfilled.</span></span> <span data-ttu-id="0ac9f-133">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-133">Required.</span></span>|
|<span data-ttu-id="0ac9f-134">conditions</span><span class="sxs-lookup"><span data-stu-id="0ac9f-134">conditions</span></span>|[<span data-ttu-id="0ac9f-135">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0ac9f-135">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)|<span data-ttu-id="0ac9f-136">Условия, выполнение которых активирует соответствующие действия для указанного правила.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-136">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> <span data-ttu-id="0ac9f-137">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-137">Optional.</span></span>|
|<span data-ttu-id="0ac9f-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac9f-138">displayName</span></span>| <span data-ttu-id="0ac9f-139">String</span><span class="sxs-lookup"><span data-stu-id="0ac9f-139">String</span></span>  | <span data-ttu-id="0ac9f-140">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-140">The display name of the rule.</span></span> <span data-ttu-id="0ac9f-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-141">Required.</span></span>|
|<span data-ttu-id="0ac9f-142">exceptions</span><span class="sxs-lookup"><span data-stu-id="0ac9f-142">exceptions</span></span>| [<span data-ttu-id="0ac9f-143">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="0ac9f-143">messageRulePredicates</span></span>](../resources/messagerulepredicates.md)| <span data-ttu-id="0ac9f-144">Представляет условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-144">Represents exception conditions for the rule.</span></span> <span data-ttu-id="0ac9f-145">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-145">Optional.</span></span> |
|<span data-ttu-id="0ac9f-146">isEnabled</span><span class="sxs-lookup"><span data-stu-id="0ac9f-146">isEnabled</span></span> | <span data-ttu-id="0ac9f-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac9f-147">Boolean</span></span> | <span data-ttu-id="0ac9f-148">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-148">Indicates whether the rule is enabled to be applied to messages.</span></span> <span data-ttu-id="0ac9f-149">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-149">Optional.</span></span> |
|<span data-ttu-id="0ac9f-150">sequence</span><span class="sxs-lookup"><span data-stu-id="0ac9f-150">sequence</span></span>| <span data-ttu-id="0ac9f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac9f-151">Int32</span></span> | <span data-ttu-id="0ac9f-152">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-152">Indicates the order in which the rule is executed, among other rules.</span></span> <span data-ttu-id="0ac9f-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-153">Required.</span></span>|

## <a name="response"></a><span data-ttu-id="0ac9f-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ac9f-154">Response</span></span>
<span data-ttu-id="0ac9f-155">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект **messageRule** в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-155">If successful, this method returns `201 Created` response code and a **messageRule** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac9f-156">Пример</span><span class="sxs-lookup"><span data-stu-id="0ac9f-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ac9f-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ac9f-157">Request</span></span>
<span data-ttu-id="0ac9f-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-158">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0ac9f-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="0ac9f-159">Response</span></span>
<span data-ttu-id="0ac9f-p110">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ac9f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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