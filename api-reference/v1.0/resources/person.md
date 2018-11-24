# <a name="person-resource-type"></a><span data-ttu-id="b1222-101">Тип ресурса person</span><span class="sxs-lookup"><span data-stu-id="b1222-101">person resource type</span></span>

<span data-ttu-id="b1222-p101">Агрегирование сведений о человеке из почты, контактов и социальных сетей. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога вашей организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype).</span><span class="sxs-lookup"><span data-stu-id="b1222-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="b1222-104">Методы</span><span class="sxs-lookup"><span data-stu-id="b1222-104">Methods</span></span>

| <span data-ttu-id="b1222-105">Метод</span><span class="sxs-lookup"><span data-stu-id="b1222-105">Method</span></span> | <span data-ttu-id="b1222-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="b1222-106">Return Type</span></span> | <span data-ttu-id="b1222-107">Описание</span><span class="sxs-lookup"><span data-stu-id="b1222-107">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="b1222-108">List people</span><span class="sxs-lookup"><span data-stu-id="b1222-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="b1222-109">**person**</span><span class="sxs-lookup"><span data-stu-id="b1222-109">**person**</span></span> |<span data-ttu-id="b1222-110">Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="b1222-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="b1222-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1222-111">Properties</span></span>

| <span data-ttu-id="b1222-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1222-112">Property</span></span> | <span data-ttu-id="b1222-113">Тип</span><span class="sxs-lookup"><span data-stu-id="b1222-113">Type</span></span> | <span data-ttu-id="b1222-114">Описание</span><span class="sxs-lookup"><span data-stu-id="b1222-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b1222-115">birthday</span><span class="sxs-lookup"><span data-stu-id="b1222-115">birthday</span></span>|<span data-ttu-id="b1222-116">String</span><span class="sxs-lookup"><span data-stu-id="b1222-116">String</span></span>|<span data-ttu-id="b1222-117">День рождения человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-117">The person's birthday.</span></span>|
|<span data-ttu-id="b1222-118">companyName</span><span class="sxs-lookup"><span data-stu-id="b1222-118">companyName</span></span>|<span data-ttu-id="b1222-119">String</span><span class="sxs-lookup"><span data-stu-id="b1222-119">String</span></span>|<span data-ttu-id="b1222-120">Название компании человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-120">The name of the person's company.</span></span>|
|<span data-ttu-id="b1222-121">department</span><span class="sxs-lookup"><span data-stu-id="b1222-121">department</span></span>|<span data-ttu-id="b1222-122">String</span><span class="sxs-lookup"><span data-stu-id="b1222-122">String</span></span>|<span data-ttu-id="b1222-123">Отдел, в котором работает человек.</span><span class="sxs-lookup"><span data-stu-id="b1222-123">The person's department.</span></span>|
|<span data-ttu-id="b1222-124">displayName</span><span class="sxs-lookup"><span data-stu-id="b1222-124">displayName</span></span>|<span data-ttu-id="b1222-125">String</span><span class="sxs-lookup"><span data-stu-id="b1222-125">String</span></span>|<span data-ttu-id="b1222-126">Отображаемое имя человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-126">The person's display name.</span></span>|
|<span data-ttu-id="b1222-127">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="b1222-127">scoredEmailAddresses</span></span>|<span data-ttu-id="b1222-128">Коллекция [scoredEmailAddress](scoredemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="b1222-128">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="b1222-129">Электронные адреса человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-129">The person's email addresses.</span></span>|
|<span data-ttu-id="b1222-130">givenName</span><span class="sxs-lookup"><span data-stu-id="b1222-130">givenName</span></span>|<span data-ttu-id="b1222-131">String</span><span class="sxs-lookup"><span data-stu-id="b1222-131">String</span></span>|<span data-ttu-id="b1222-132">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-132">The person's given name.</span></span>|
|<span data-ttu-id="b1222-133">id</span><span class="sxs-lookup"><span data-stu-id="b1222-133">id</span></span>|<span data-ttu-id="b1222-134">String</span><span class="sxs-lookup"><span data-stu-id="b1222-134">String</span></span>|<span data-ttu-id="b1222-p102">Уникальный идентификатор человека. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1222-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="b1222-137">imAddress</span><span class="sxs-lookup"><span data-stu-id="b1222-137">imAddress</span></span>|<span data-ttu-id="b1222-138">String</span><span class="sxs-lookup"><span data-stu-id="b1222-138">String</span></span>|<span data-ttu-id="b1222-p103">Адрес SIP VOIP для обмена мгновенными сообщениями для пользователя. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="b1222-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="b1222-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="b1222-141">isFavorite</span></span>|<span data-ttu-id="b1222-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1222-142">Boolean</span></span>|<span data-ttu-id="b1222-143">Имеет значение `true`, если пользователь добавил этого человека в список избранных.</span><span class="sxs-lookup"><span data-stu-id="b1222-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="b1222-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="b1222-144">jobTitle</span></span>|<span data-ttu-id="b1222-145">String</span><span class="sxs-lookup"><span data-stu-id="b1222-145">String</span></span>|<span data-ttu-id="b1222-146">Должность человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-146">The person's job title.</span></span>|
|<span data-ttu-id="b1222-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="b1222-147">officeLocation</span></span>|<span data-ttu-id="b1222-148">String</span><span class="sxs-lookup"><span data-stu-id="b1222-148">String</span></span>|<span data-ttu-id="b1222-149">Расположение офиса человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-149">The location of the person's office.</span></span>|
|<span data-ttu-id="b1222-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="b1222-150">personNotes</span></span>|<span data-ttu-id="b1222-151">String</span><span class="sxs-lookup"><span data-stu-id="b1222-151">String</span></span>|<span data-ttu-id="b1222-152">Заметки в произвольной форме о человеке, созданные пользователем.</span><span class="sxs-lookup"><span data-stu-id="b1222-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="b1222-153">personType</span><span class="sxs-lookup"><span data-stu-id="b1222-153">personType</span></span>|[<span data-ttu-id="b1222-154">personType</span><span class="sxs-lookup"><span data-stu-id="b1222-154">personType</span></span>](persontype.md) |<span data-ttu-id="b1222-155">Тип человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-155">The type of person.</span></span>|
|<span data-ttu-id="b1222-156">phones</span><span class="sxs-lookup"><span data-stu-id="b1222-156">phones</span></span>|<span data-ttu-id="b1222-157">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="b1222-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="b1222-158">Номера телефонов человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="b1222-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="b1222-159">postalAddresses</span></span>|<span data-ttu-id="b1222-160">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="b1222-160">[location](location.md) collection</span></span>|<span data-ttu-id="b1222-161">Адреса человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-161">The person's addresses.</span></span>|
|<span data-ttu-id="b1222-162">profession</span><span class="sxs-lookup"><span data-stu-id="b1222-162">profession</span></span>|<span data-ttu-id="b1222-163">String</span><span class="sxs-lookup"><span data-stu-id="b1222-163">String</span></span>|<span data-ttu-id="b1222-164">Профессия человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-164">The person's profession.</span></span>|
|<span data-ttu-id="b1222-165">surname</span><span class="sxs-lookup"><span data-stu-id="b1222-165">surname</span></span>|<span data-ttu-id="b1222-166">String</span><span class="sxs-lookup"><span data-stu-id="b1222-166">String</span></span>|<span data-ttu-id="b1222-167">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-167">The person's surname.</span></span>|
|<span data-ttu-id="b1222-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1222-168">userPrincipalName</span></span>|<span data-ttu-id="b1222-169">String</span><span class="sxs-lookup"><span data-stu-id="b1222-169">String</span></span>|<span data-ttu-id="b1222-p104">Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.</span><span class="sxs-lookup"><span data-stu-id="b1222-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="b1222-174">websites</span><span class="sxs-lookup"><span data-stu-id="b1222-174">websites</span></span>|<span data-ttu-id="b1222-175">Коллекция [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="b1222-175">[website](website.md) collection</span></span>|<span data-ttu-id="b1222-176">Веб-сайты человека.</span><span class="sxs-lookup"><span data-stu-id="b1222-176">The person's websites.</span></span>|
|<span data-ttu-id="b1222-177">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="b1222-177">yomiCompany</span></span>|<span data-ttu-id="b1222-178">String</span><span class="sxs-lookup"><span data-stu-id="b1222-178">String</span></span>|<span data-ttu-id="b1222-179">Название компании человека, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="b1222-179">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1222-180">Связи</span><span class="sxs-lookup"><span data-stu-id="b1222-180">Relationships</span></span>

<span data-ttu-id="b1222-181">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b1222-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1222-182">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b1222-182">JSON representation</span></span>

<span data-ttu-id="b1222-183">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1222-183">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
