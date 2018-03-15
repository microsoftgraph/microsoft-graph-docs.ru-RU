# <a name="update-grouplifecyclepolicy"></a><span data-ttu-id="766f5-101">Update groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="766f5-101">Update groupLifecyclePolicy</span></span>

<span data-ttu-id="766f5-102">Обновляет свойства объекта groupLifecyclePolicy[тип ресурса groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="766f5-102">Update the properties of a groupLifecyclePolicy[groupLifecyclePolicy resource type](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="766f5-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="766f5-103">Permissions</span></span>

<span data-ttu-id="766f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="766f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 
|<span data-ttu-id="766f5-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="766f5-106">Permission type</span></span>      | <span data-ttu-id="766f5-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="766f5-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="766f5-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="766f5-108">Delegated (work or school account)</span></span> | <span data-ttu-id="766f5-109">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="766f5-109">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="766f5-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="766f5-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="766f5-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="766f5-111">Not supported.</span></span>    |
|<span data-ttu-id="766f5-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="766f5-112">Application</span></span> | <span data-ttu-id="766f5-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="766f5-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="766f5-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="766f5-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groupLifecyclePolicies/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="766f5-115">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="766f5-115">Optional request headers</span></span>
| <span data-ttu-id="766f5-116">Имя</span><span class="sxs-lookup"><span data-stu-id="766f5-116">Name</span></span> | <span data-ttu-id="766f5-117">Описание</span><span class="sxs-lookup"><span data-stu-id="766f5-117">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="766f5-118">Авторизация</span><span class="sxs-lookup"><span data-stu-id="766f5-118">Authorization</span></span> | <span data-ttu-id="766f5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="766f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="766f5-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="766f5-121">Content-Type</span></span>  | <span data-ttu-id="766f5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="766f5-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="766f5-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="766f5-123">Request body</span></span>

<span data-ttu-id="766f5-124">В теле запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="766f5-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="766f5-125">Предыдущие значения существующих свойств, не включенных в тело запроса, остаются прежними или повторно вычисляются с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="766f5-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="766f5-126">Для наилучших результатов не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="766f5-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="766f5-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="766f5-127">Property</span></span> | <span data-ttu-id="766f5-128">Тип</span><span class="sxs-lookup"><span data-stu-id="766f5-128">Type</span></span> | <span data-ttu-id="766f5-129">Описание</span><span class="sxs-lookup"><span data-stu-id="766f5-129">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="766f5-130">alternateNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="766f5-130">alternateNotificationEmails</span></span>|<span data-ttu-id="766f5-131">String</span><span class="sxs-lookup"><span data-stu-id="766f5-131">String</span></span>| <span data-ttu-id="766f5-132">Список адресов электронной почты для отправки уведомлений о группах без владельцев.</span><span class="sxs-lookup"><span data-stu-id="766f5-132">List of email address to send notifications for groups without owners.</span></span> <span data-ttu-id="766f5-133">Можно указать несколько адресов электронной почты, разделив их точкой с запятой.</span><span class="sxs-lookup"><span data-stu-id="766f5-133">Multiple email address can be defined by separating email address with a semicolon.</span></span> |
|<span data-ttu-id="766f5-134">groupLifetimeInDays</span><span class="sxs-lookup"><span data-stu-id="766f5-134">groupLifetimeInDays</span></span>|<span data-ttu-id="766f5-135">Int32</span><span class="sxs-lookup"><span data-stu-id="766f5-135">Int32</span></span>| <span data-ttu-id="766f5-136">Количество дней до истечения срока действия группы.</span><span class="sxs-lookup"><span data-stu-id="766f5-136">Number of days before a group expires and needs to be renewed.</span></span> <span data-ttu-id="766f5-137">После продления группа будет оставаться активной в течение указанного количества дней.</span><span class="sxs-lookup"><span data-stu-id="766f5-137">Once renewed, the group expiration is extended by the number of days defined.</span></span> |
|<span data-ttu-id="766f5-138">managedGroupTypes</span><span class="sxs-lookup"><span data-stu-id="766f5-138">managedGroupTypes</span></span>|<span data-ttu-id="766f5-139">String</span><span class="sxs-lookup"><span data-stu-id="766f5-139">String</span></span>| <span data-ttu-id="766f5-140">Тип группы, к которому применяется политика истечения срока действия.</span><span class="sxs-lookup"><span data-stu-id="766f5-140">The group type for which the expiration policy applies.</span></span> <span data-ttu-id="766f5-141">Возможные значения — **All**, **Selected** и **None**.</span><span class="sxs-lookup"><span data-stu-id="766f5-141">Possible values are **All**, **Selected** or **None**.</span></span> |

## <a name="response"></a><span data-ttu-id="766f5-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="766f5-142">Response</span></span>

<span data-ttu-id="766f5-143">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="766f5-143">If successful, this method returns a `200 OK` response code and updated [Chart](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="766f5-144">Пример</span><span class="sxs-lookup"><span data-stu-id="766f5-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="766f5-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="766f5-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_grouplifecyclepolicy"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
##### <a name="response"></a><span data-ttu-id="766f5-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="766f5-146">Response</span></span>
<span data-ttu-id="766f5-147">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="766f5-147">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "id": "id-value",
  "groupLifetimeInDays": 180,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->