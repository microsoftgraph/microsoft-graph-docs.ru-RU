# <a name="update-rule"></a><span data-ttu-id="1296c-101">Обновление правила</span><span class="sxs-lookup"><span data-stu-id="1296c-101">Update rule</span></span>


<span data-ttu-id="1296c-102">Изменение записываемых свойств объекта [messageRule](../resources/messagerule.md) и сохранение изменений.</span><span class="sxs-lookup"><span data-stu-id="1296c-102">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="1296c-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1296c-103">Permissions</span></span>
<span data-ttu-id="1296c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1296c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1296c-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1296c-106">Permission type</span></span>      | <span data-ttu-id="1296c-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1296c-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1296c-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1296c-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1296c-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1296c-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1296c-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1296c-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1296c-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1296c-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="1296c-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1296c-112">Application</span></span> | <span data-ttu-id="1296c-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1296c-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1296c-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1296c-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="1296c-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1296c-115">Optional request headers</span></span>
| <span data-ttu-id="1296c-116">Имя</span><span class="sxs-lookup"><span data-stu-id="1296c-116">Name</span></span>       | <span data-ttu-id="1296c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="1296c-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="1296c-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1296c-118">Authorization</span></span>  | <span data-ttu-id="1296c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1296c-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="1296c-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1296c-121">Request body</span></span>
<span data-ttu-id="1296c-p103">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="1296c-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1296c-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="1296c-125">Property</span></span>     | <span data-ttu-id="1296c-126">Тип</span><span class="sxs-lookup"><span data-stu-id="1296c-126">Type</span></span>   |<span data-ttu-id="1296c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="1296c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1296c-128">actions</span><span class="sxs-lookup"><span data-stu-id="1296c-128">actions</span></span> | [<span data-ttu-id="1296c-129">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="1296c-129">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="1296c-130">Действия, которые нужно применить к сообщению при выполнении определенных условий.</span><span class="sxs-lookup"><span data-stu-id="1296c-130">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="1296c-131">conditions</span><span class="sxs-lookup"><span data-stu-id="1296c-131">Conditions:</span></span> | [<span data-ttu-id="1296c-132">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="1296c-132">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="1296c-133">Условия, при соблюдении которых с указанным правилом выполняются соответствующие действия.</span><span class="sxs-lookup"><span data-stu-id="1296c-133">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="1296c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1296c-134">displayName</span></span> | <span data-ttu-id="1296c-135">Строка</span><span class="sxs-lookup"><span data-stu-id="1296c-135">String</span></span> | <span data-ttu-id="1296c-136">Отображаемое имя правила.</span><span class="sxs-lookup"><span data-stu-id="1296c-136">The display name of the rule.</span></span> |
| <span data-ttu-id="1296c-137">exceptions</span><span class="sxs-lookup"><span data-stu-id="1296c-137">exceptions</span></span> | [<span data-ttu-id="1296c-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="1296c-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="1296c-139">Условия исключения для правила.</span><span class="sxs-lookup"><span data-stu-id="1296c-139">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="1296c-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1296c-140">isEnabled</span></span> | <span data-ttu-id="1296c-141">Логический</span><span class="sxs-lookup"><span data-stu-id="1296c-141">Boolean</span></span> | <span data-ttu-id="1296c-142">Указывает, включено ли применение правила к сообщениям.</span><span class="sxs-lookup"><span data-stu-id="1296c-142">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="1296c-143">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="1296c-143">isReadOnly</span></span> | <span data-ttu-id="1296c-144">Логический</span><span class="sxs-lookup"><span data-stu-id="1296c-144">Boolean</span></span> | <span data-ttu-id="1296c-145">Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил.</span><span class="sxs-lookup"><span data-stu-id="1296c-145">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="1296c-146">sequence</span><span class="sxs-lookup"><span data-stu-id="1296c-146">Sequence</span></span> | <span data-ttu-id="1296c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="1296c-147">Int32</span></span> | <span data-ttu-id="1296c-148">Определяет последовательность выполнения правила среди прочих правил.</span><span class="sxs-lookup"><span data-stu-id="1296c-148">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="1296c-149">Ответ</span><span class="sxs-lookup"><span data-stu-id="1296c-149">Response</span></span>
<span data-ttu-id="1296c-150">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [messageRule](../resources/messagerule.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="1296c-150">If successful, this method returns a `200 OK` response code and updated [ChartSeries](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1296c-151">Пример</span><span class="sxs-lookup"><span data-stu-id="1296c-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1296c-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="1296c-152">Request</span></span>
<span data-ttu-id="1296c-153">В приведенном ниже примере меняется имя правила, а также действия, выполняемые с этим правилом в [примере](messagerule_get.md#example) [получения правила](messagerule_get.md), — вместо пересылки на указанный адрес устанавливается высокая важность.</span><span class="sxs-lookup"><span data-stu-id="1296c-153">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule_get.md#example) in [Get rule](messagerule_get.md), from forwarding to an address to marking its importance as high.</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')

Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
##### <a name="response"></a><span data-ttu-id="1296c-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="1296c-154">Response</span></span>
<span data-ttu-id="1296c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1296c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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