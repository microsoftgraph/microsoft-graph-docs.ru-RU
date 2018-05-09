# <a name="update-organization"></a><span data-ttu-id="94445-101">Обновление организации</span><span class="sxs-lookup"><span data-stu-id="94445-101">Update organization</span></span>

<span data-ttu-id="94445-102">Обновление свойств объекта organization, для которого выполнена проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="94445-102">Update the properties of the currently authenticated organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="94445-103">Разрешения</span><span class="sxs-lookup"><span data-stu-id="94445-103">Permissions</span></span>

<span data-ttu-id="94445-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="94445-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="94445-106">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="94445-106">Permission type</span></span> | <span data-ttu-id="94445-107">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="94445-107">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94445-108">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="94445-108">Delegated (work or school account)</span></span> | <span data-ttu-id="94445-109">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94445-109">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94445-110">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="94445-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94445-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94445-111">Not supported.</span></span>    |
|<span data-ttu-id="94445-112">Для приложений</span><span class="sxs-lookup"><span data-stu-id="94445-112">Application</span></span> | <span data-ttu-id="94445-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="94445-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="94445-114">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="94445-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization

```

## <a name="request-headers"></a><span data-ttu-id="94445-115">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="94445-115">Request headers</span></span>

| <span data-ttu-id="94445-116">Имя</span><span class="sxs-lookup"><span data-stu-id="94445-116">Name</span></span>       | <span data-ttu-id="94445-117">Тип</span><span class="sxs-lookup"><span data-stu-id="94445-117">Type</span></span> | <span data-ttu-id="94445-118">Описание</span><span class="sxs-lookup"><span data-stu-id="94445-118">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="94445-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="94445-119">Authorization</span></span>  | <span data-ttu-id="94445-120">string</span><span class="sxs-lookup"><span data-stu-id="94445-120">string</span></span>  | <span data-ttu-id="94445-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="94445-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="94445-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="94445-123">Request body</span></span>
<span data-ttu-id="94445-124">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="94445-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="94445-125">Предыдущие значения существующих свойств, не включенных в тело запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="94445-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="94445-126">Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="94445-126">For best performance, you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="94445-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="94445-127">Property</span></span>     | <span data-ttu-id="94445-128">Тип</span><span class="sxs-lookup"><span data-stu-id="94445-128">Type</span></span>   |<span data-ttu-id="94445-129">Описание</span><span class="sxs-lookup"><span data-stu-id="94445-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94445-130">marketingNotificationEmails</span><span class="sxs-lookup"><span data-stu-id="94445-130">marketingNotificationEmails</span></span>|<span data-ttu-id="94445-131">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="94445-131">String collection</span></span>|                                        <span data-ttu-id="94445-132">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="94445-132">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="94445-133">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="94445-133">privacyProfile</span></span>|[<span data-ttu-id="94445-134">privacyProfile</span><span class="sxs-lookup"><span data-stu-id="94445-134">privacyProfile</span></span>](../resources/privacyprofile.md)|<span data-ttu-id="94445-135">Профиль конфиденциальности организации (заданные свойства statementUrl и contactEmail).</span><span class="sxs-lookup"><span data-stu-id="94445-135">The privacy profile of an organization (set statementUrl and contactEmail).</span></span>            |
|<span data-ttu-id="94445-136">securityComplianceNotificationMails</span><span class="sxs-lookup"><span data-stu-id="94445-136">securityComplianceNotificationMails</span></span>|<span data-ttu-id="94445-137">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="94445-137">String collection</span></span>||
|<span data-ttu-id="94445-138">securityComplianceNotificationPhones</span><span class="sxs-lookup"><span data-stu-id="94445-138">securityComplianceNotificationPhones</span></span>|<span data-ttu-id="94445-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="94445-139">String collection</span></span>||
|<span data-ttu-id="94445-140">technicalNotificationMails</span><span class="sxs-lookup"><span data-stu-id="94445-140">technicalNotificationMails</span></span>|<span data-ttu-id="94445-141">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="94445-141">String collection</span></span>|                                        <span data-ttu-id="94445-142">**Примечание.** Значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="94445-142">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="94445-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="94445-143">Response</span></span>

<span data-ttu-id="94445-144">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="94445-144">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="94445-145">Пример</span><span class="sxs-lookup"><span data-stu-id="94445-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="94445-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="94445-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_organization"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization
Content-type: application/json
Content-length: 411

{
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      "contactEmail":"alice@contoso.com",
      "statementUrl":"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
}
```

### <a name="response"></a><span data-ttu-id="94445-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="94445-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organization"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organization",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
