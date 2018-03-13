# <a name="person-resource-type"></a><span data-ttu-id="29723-101">Тип ресурса person</span><span class="sxs-lookup"><span data-stu-id="29723-101">person resource type</span></span>

<span data-ttu-id="29723-p101">Агрегирование сведений о человеке из почты, контактов и социальных сетей. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога вашей организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype).</span><span class="sxs-lookup"><span data-stu-id="29723-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="29723-104">Методы</span><span class="sxs-lookup"><span data-stu-id="29723-104">Methods</span></span>

| <span data-ttu-id="29723-105">Метод</span><span class="sxs-lookup"><span data-stu-id="29723-105">Method</span></span>           | <span data-ttu-id="29723-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29723-106">Return Type</span></span>    |<span data-ttu-id="29723-107">Описание</span><span class="sxs-lookup"><span data-stu-id="29723-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29723-108">List people</span><span class="sxs-lookup"><span data-stu-id="29723-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="29723-109">**person**</span><span class="sxs-lookup"><span data-stu-id="29723-109">**person**</span></span> |<span data-ttu-id="29723-110">Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="29723-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|
|[<span data-ttu-id="29723-111">Get person</span><span class="sxs-lookup"><span data-stu-id="29723-111">Get person</span></span>](../api/person_get.md) | <span data-ttu-id="29723-112">**person**</span><span class="sxs-lookup"><span data-stu-id="29723-112">**person**</span></span> |<span data-ttu-id="29723-113">Получение свойств и связей объекта person.</span><span class="sxs-lookup"><span data-stu-id="29723-113">Get properties and relationships of a person object.</span></span>|

## <a name="properties"></a><span data-ttu-id="29723-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="29723-114">Properties</span></span>
| <span data-ttu-id="29723-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="29723-115">Property</span></span>     | <span data-ttu-id="29723-116">Тип</span><span class="sxs-lookup"><span data-stu-id="29723-116">Type</span></span>   |<span data-ttu-id="29723-117">Описание</span><span class="sxs-lookup"><span data-stu-id="29723-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29723-118">birthday</span><span class="sxs-lookup"><span data-stu-id="29723-118">birthday</span></span>|<span data-ttu-id="29723-119">String</span><span class="sxs-lookup"><span data-stu-id="29723-119">String</span></span>|<span data-ttu-id="29723-120">День рождения человека.</span><span class="sxs-lookup"><span data-stu-id="29723-120">The person's birthday.</span></span>|
|<span data-ttu-id="29723-121">companyName</span><span class="sxs-lookup"><span data-stu-id="29723-121">companyName</span></span>|<span data-ttu-id="29723-122">String</span><span class="sxs-lookup"><span data-stu-id="29723-122">String</span></span>|<span data-ttu-id="29723-123">Название компании человека.</span><span class="sxs-lookup"><span data-stu-id="29723-123">The name of the person's company.</span></span>|
|<span data-ttu-id="29723-124">department</span><span class="sxs-lookup"><span data-stu-id="29723-124">department</span></span>|<span data-ttu-id="29723-125">String</span><span class="sxs-lookup"><span data-stu-id="29723-125">String</span></span>|<span data-ttu-id="29723-126">Отдел, в котором работает человек.</span><span class="sxs-lookup"><span data-stu-id="29723-126">The person's department.</span></span>|
|<span data-ttu-id="29723-127">displayName</span><span class="sxs-lookup"><span data-stu-id="29723-127">displayName</span></span>|<span data-ttu-id="29723-128">String</span><span class="sxs-lookup"><span data-stu-id="29723-128">String</span></span>|<span data-ttu-id="29723-129">Отображаемое имя человека.</span><span class="sxs-lookup"><span data-stu-id="29723-129">The person's display name.</span></span>|
|<span data-ttu-id="29723-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="29723-130">scoredEmailAddresses</span></span>|<span data-ttu-id="29723-131">Коллекция [scoredEmailAddress](scoredemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="29723-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="29723-132">Электронные адреса человека.</span><span class="sxs-lookup"><span data-stu-id="29723-132">The person's email addresses.</span></span>|
|<span data-ttu-id="29723-133">givenName</span><span class="sxs-lookup"><span data-stu-id="29723-133">givenName</span></span>|<span data-ttu-id="29723-134">String</span><span class="sxs-lookup"><span data-stu-id="29723-134">String</span></span>|<span data-ttu-id="29723-135">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="29723-135">The person's given name.</span></span>|
|<span data-ttu-id="29723-136">id</span><span class="sxs-lookup"><span data-stu-id="29723-136">id</span></span>|<span data-ttu-id="29723-137">String</span><span class="sxs-lookup"><span data-stu-id="29723-137">String</span></span>|<span data-ttu-id="29723-p102">Уникальный идентификатор человека. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29723-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="29723-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="29723-140">imAddress</span></span>|<span data-ttu-id="29723-141">String</span><span class="sxs-lookup"><span data-stu-id="29723-141">String</span></span>|<span data-ttu-id="29723-p103">Адрес SIP VOIP для обмена мгновенными сообщениями для пользователя. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29723-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="29723-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="29723-144">isFavorite</span></span>|<span data-ttu-id="29723-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="29723-145">Boolean</span></span>|<span data-ttu-id="29723-146">Имеет значение `true`, если пользователь добавил этого человека в список избранных.</span><span class="sxs-lookup"><span data-stu-id="29723-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="29723-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="29723-147">jobTitle</span></span>|<span data-ttu-id="29723-148">String</span><span class="sxs-lookup"><span data-stu-id="29723-148">String</span></span>|<span data-ttu-id="29723-149">Должность человека.</span><span class="sxs-lookup"><span data-stu-id="29723-149">The person's job title.</span></span>|
|<span data-ttu-id="29723-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="29723-150">officeLocation</span></span>|<span data-ttu-id="29723-151">String</span><span class="sxs-lookup"><span data-stu-id="29723-151">String</span></span>|<span data-ttu-id="29723-152">Расположение офиса человека.</span><span class="sxs-lookup"><span data-stu-id="29723-152">The location of the person's office.</span></span>|
|<span data-ttu-id="29723-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="29723-153">personNotes</span></span>|<span data-ttu-id="29723-154">String</span><span class="sxs-lookup"><span data-stu-id="29723-154">String</span></span>|<span data-ttu-id="29723-155">Заметки в произвольной форме о человеке, созданные пользователем.</span><span class="sxs-lookup"><span data-stu-id="29723-155">Free-form notes that the the user has taken about this person.</span></span>|
|<span data-ttu-id="29723-156">personType</span><span class="sxs-lookup"><span data-stu-id="29723-156">personType</span></span>|<span data-ttu-id="29723-157">Коллекция [personType](persontype.md)</span><span class="sxs-lookup"><span data-stu-id="29723-157">[personType](persontype.md) collection</span></span>|<span data-ttu-id="29723-158">Тип человека.</span><span class="sxs-lookup"><span data-stu-id="29723-158">The type of person.</span></span>|
|<span data-ttu-id="29723-159">phones</span><span class="sxs-lookup"><span data-stu-id="29723-159">phones</span></span>|<span data-ttu-id="29723-160">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="29723-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="29723-161">Номера телефонов человека.</span><span class="sxs-lookup"><span data-stu-id="29723-161">The person's phone numbers.</span></span>|
|<span data-ttu-id="29723-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="29723-162">postalAddresses</span></span>|<span data-ttu-id="29723-163">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="29723-163">[location](location.md) collection</span></span>|<span data-ttu-id="29723-164">Адреса человека.</span><span class="sxs-lookup"><span data-stu-id="29723-164">The person's addresses.</span></span>|
|<span data-ttu-id="29723-165">profession</span><span class="sxs-lookup"><span data-stu-id="29723-165">profession</span></span>|<span data-ttu-id="29723-166">String</span><span class="sxs-lookup"><span data-stu-id="29723-166">String</span></span>|<span data-ttu-id="29723-167">Профессия человека.</span><span class="sxs-lookup"><span data-stu-id="29723-167">The person's profession.</span></span>|
|<span data-ttu-id="29723-168">surname</span><span class="sxs-lookup"><span data-stu-id="29723-168">surname</span></span>|<span data-ttu-id="29723-169">String</span><span class="sxs-lookup"><span data-stu-id="29723-169">String</span></span>|<span data-ttu-id="29723-170">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="29723-170">The person's surname.</span></span>|
|<span data-ttu-id="29723-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="29723-171">userPrincipalName</span></span>|<span data-ttu-id="29723-172">String</span><span class="sxs-lookup"><span data-stu-id="29723-172">String</span></span>|<span data-ttu-id="29723-p104">Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.</span><span class="sxs-lookup"><span data-stu-id="29723-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="29723-177">websites</span><span class="sxs-lookup"><span data-stu-id="29723-177">websites</span></span>|<span data-ttu-id="29723-178">Коллекция [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="29723-178">[website](website.md) collection</span></span>|<span data-ttu-id="29723-179">Веб-сайты человека.</span><span class="sxs-lookup"><span data-stu-id="29723-179">The person's websites.</span></span>|
|<span data-ttu-id="29723-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="29723-180">yomiCompany</span></span>|<span data-ttu-id="29723-181">String</span><span class="sxs-lookup"><span data-stu-id="29723-181">String</span></span>|<span data-ttu-id="29723-182">Название компании человека, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="29723-182">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29723-183">Связи</span><span class="sxs-lookup"><span data-stu-id="29723-183">Relationships</span></span>
<span data-ttu-id="29723-184">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="29723-184">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="29723-185">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="29723-185">JSON representation</span></span>

<span data-ttu-id="29723-186">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29723-186">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
