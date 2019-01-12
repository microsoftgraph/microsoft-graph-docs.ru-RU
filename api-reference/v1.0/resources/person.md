---
title: Тип ресурса person
description: Агрегирование сведений о человеке из почты, контактов и социальных сетей. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога вашей организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype).
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: c92709143ee7def0ede98dfdb81a419df43c4493
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940297"
---
# <a name="person-resource-type"></a><span data-ttu-id="fe188-104">Тип ресурса person</span><span class="sxs-lookup"><span data-stu-id="fe188-104">person resource type</span></span>

<span data-ttu-id="fe188-p102">Агрегирование сведений о человеке из почты, контактов и социальных сетей. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога вашей организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype).</span><span class="sxs-lookup"><span data-stu-id="fe188-p102">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="fe188-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fe188-107">Methods</span></span>

| <span data-ttu-id="fe188-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fe188-108">Method</span></span> | <span data-ttu-id="fe188-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe188-109">Return Type</span></span> | <span data-ttu-id="fe188-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe188-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe188-111">List people</span><span class="sxs-lookup"><span data-stu-id="fe188-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="fe188-112">**person**</span><span class="sxs-lookup"><span data-stu-id="fe188-112">**person**</span></span> |<span data-ttu-id="fe188-113">Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="fe188-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="fe188-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe188-114">Properties</span></span>

| <span data-ttu-id="fe188-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe188-115">Property</span></span> | <span data-ttu-id="fe188-116">Тип</span><span class="sxs-lookup"><span data-stu-id="fe188-116">Type</span></span> | <span data-ttu-id="fe188-117">Описание</span><span class="sxs-lookup"><span data-stu-id="fe188-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="fe188-118">birthday</span><span class="sxs-lookup"><span data-stu-id="fe188-118">birthday</span></span>|<span data-ttu-id="fe188-119">String</span><span class="sxs-lookup"><span data-stu-id="fe188-119">String</span></span>|<span data-ttu-id="fe188-120">День рождения человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-120">The person's birthday.</span></span>|
|<span data-ttu-id="fe188-121">companyName</span><span class="sxs-lookup"><span data-stu-id="fe188-121">companyName</span></span>|<span data-ttu-id="fe188-122">String</span><span class="sxs-lookup"><span data-stu-id="fe188-122">String</span></span>|<span data-ttu-id="fe188-123">Название компании человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-123">The name of the person's company.</span></span>|
|<span data-ttu-id="fe188-124">department</span><span class="sxs-lookup"><span data-stu-id="fe188-124">department</span></span>|<span data-ttu-id="fe188-125">String</span><span class="sxs-lookup"><span data-stu-id="fe188-125">String</span></span>|<span data-ttu-id="fe188-126">Отдел, в котором работает человек.</span><span class="sxs-lookup"><span data-stu-id="fe188-126">The person's department.</span></span>|
|<span data-ttu-id="fe188-127">displayName</span><span class="sxs-lookup"><span data-stu-id="fe188-127">displayName</span></span>|<span data-ttu-id="fe188-128">String</span><span class="sxs-lookup"><span data-stu-id="fe188-128">String</span></span>|<span data-ttu-id="fe188-129">Отображаемое имя человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-129">The person's display name.</span></span>|
|<span data-ttu-id="fe188-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="fe188-130">scoredEmailAddresses</span></span>|<span data-ttu-id="fe188-131">Коллекция [scoredEmailAddress](scoredemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="fe188-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="fe188-132">Электронные адреса человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-132">The person's email addresses.</span></span>|
|<span data-ttu-id="fe188-133">givenName</span><span class="sxs-lookup"><span data-stu-id="fe188-133">givenName</span></span>|<span data-ttu-id="fe188-134">String</span><span class="sxs-lookup"><span data-stu-id="fe188-134">String</span></span>|<span data-ttu-id="fe188-135">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-135">The person's given name.</span></span>|
|<span data-ttu-id="fe188-136">id</span><span class="sxs-lookup"><span data-stu-id="fe188-136">id</span></span>|<span data-ttu-id="fe188-137">String</span><span class="sxs-lookup"><span data-stu-id="fe188-137">String</span></span>|<span data-ttu-id="fe188-p103">Уникальный идентификатор человека. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe188-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="fe188-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="fe188-140">imAddress</span></span>|<span data-ttu-id="fe188-141">String</span><span class="sxs-lookup"><span data-stu-id="fe188-141">String</span></span>|<span data-ttu-id="fe188-p104">Адрес SIP VOIP для обмена мгновенными сообщениями для пользователя. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe188-p104">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="fe188-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="fe188-144">isFavorite</span></span>|<span data-ttu-id="fe188-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fe188-145">Boolean</span></span>|<span data-ttu-id="fe188-146">Имеет значение `true`, если пользователь добавил этого человека в список избранных.</span><span class="sxs-lookup"><span data-stu-id="fe188-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="fe188-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="fe188-147">jobTitle</span></span>|<span data-ttu-id="fe188-148">String</span><span class="sxs-lookup"><span data-stu-id="fe188-148">String</span></span>|<span data-ttu-id="fe188-149">Должность человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-149">The person's job title.</span></span>|
|<span data-ttu-id="fe188-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="fe188-150">officeLocation</span></span>|<span data-ttu-id="fe188-151">String</span><span class="sxs-lookup"><span data-stu-id="fe188-151">String</span></span>|<span data-ttu-id="fe188-152">Расположение офиса человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-152">The location of the person's office.</span></span>|
|<span data-ttu-id="fe188-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="fe188-153">personNotes</span></span>|<span data-ttu-id="fe188-154">String</span><span class="sxs-lookup"><span data-stu-id="fe188-154">String</span></span>|<span data-ttu-id="fe188-155">Заметки в произвольной форме о человеке, созданные пользователем.</span><span class="sxs-lookup"><span data-stu-id="fe188-155">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="fe188-156">personType</span><span class="sxs-lookup"><span data-stu-id="fe188-156">personType</span></span>|[<span data-ttu-id="fe188-157">personType</span><span class="sxs-lookup"><span data-stu-id="fe188-157">personType</span></span>](persontype.md) |<span data-ttu-id="fe188-158">Тип человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-158">The type of person.</span></span>|
|<span data-ttu-id="fe188-159">phones</span><span class="sxs-lookup"><span data-stu-id="fe188-159">phones</span></span>|<span data-ttu-id="fe188-160">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="fe188-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="fe188-161">Номера телефонов человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-161">The person's phone numbers.</span></span>|
|<span data-ttu-id="fe188-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="fe188-162">postalAddresses</span></span>|<span data-ttu-id="fe188-163">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="fe188-163">[location](location.md) collection</span></span>|<span data-ttu-id="fe188-164">Адреса человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-164">The person's addresses.</span></span>|
|<span data-ttu-id="fe188-165">profession</span><span class="sxs-lookup"><span data-stu-id="fe188-165">profession</span></span>|<span data-ttu-id="fe188-166">String</span><span class="sxs-lookup"><span data-stu-id="fe188-166">String</span></span>|<span data-ttu-id="fe188-167">Профессия человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-167">The person's profession.</span></span>|
|<span data-ttu-id="fe188-168">surname</span><span class="sxs-lookup"><span data-stu-id="fe188-168">surname</span></span>|<span data-ttu-id="fe188-169">String</span><span class="sxs-lookup"><span data-stu-id="fe188-169">String</span></span>|<span data-ttu-id="fe188-170">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-170">The person's surname.</span></span>|
|<span data-ttu-id="fe188-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe188-171">userPrincipalName</span></span>|<span data-ttu-id="fe188-172">String</span><span class="sxs-lookup"><span data-stu-id="fe188-172">String</span></span>|<span data-ttu-id="fe188-p105">Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.</span><span class="sxs-lookup"><span data-stu-id="fe188-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="fe188-177">websites</span><span class="sxs-lookup"><span data-stu-id="fe188-177">websites</span></span>|<span data-ttu-id="fe188-178">Коллекция [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="fe188-178">[website](website.md) collection</span></span>|<span data-ttu-id="fe188-179">Веб-сайты человека.</span><span class="sxs-lookup"><span data-stu-id="fe188-179">The person's websites.</span></span>|
|<span data-ttu-id="fe188-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="fe188-180">yomiCompany</span></span>|<span data-ttu-id="fe188-181">String</span><span class="sxs-lookup"><span data-stu-id="fe188-181">String</span></span>|<span data-ttu-id="fe188-182">Название компании человека, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="fe188-182">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe188-183">Связи</span><span class="sxs-lookup"><span data-stu-id="fe188-183">Relationships</span></span>

<span data-ttu-id="fe188-184">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fe188-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe188-185">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe188-185">JSON representation</span></span>

<span data-ttu-id="fe188-186">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe188-186">The following is a JSON representation of the resource.</span></span>

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
