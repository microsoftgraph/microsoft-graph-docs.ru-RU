---
title: Тип ресурса person
description: Агрегирование сведений о человеке из почты, контактов и социальных сетей. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога вашей организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype).
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 8a1139388f5fcb17ea43cecf1cf321f490fe87c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022892"
---
# <a name="person-resource-type"></a><span data-ttu-id="e5821-104">Тип ресурса person</span><span class="sxs-lookup"><span data-stu-id="e5821-104">person resource type</span></span>

<span data-ttu-id="e5821-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5821-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5821-p102">Агрегирование сведений о человеке из почты, контактов и социальных сетей. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога вашей организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype).</span><span class="sxs-lookup"><span data-stu-id="e5821-p102">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="e5821-108">Методы</span><span class="sxs-lookup"><span data-stu-id="e5821-108">Methods</span></span>

| <span data-ttu-id="e5821-109">Метод</span><span class="sxs-lookup"><span data-stu-id="e5821-109">Method</span></span> | <span data-ttu-id="e5821-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e5821-110">Return Type</span></span> | <span data-ttu-id="e5821-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e5821-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="e5821-112">List people</span><span class="sxs-lookup"><span data-stu-id="e5821-112">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="e5821-113">**person**</span><span class="sxs-lookup"><span data-stu-id="e5821-113">**person**</span></span> |<span data-ttu-id="e5821-114">Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="e5821-114">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="e5821-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="e5821-115">Properties</span></span>

| <span data-ttu-id="e5821-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="e5821-116">Property</span></span> | <span data-ttu-id="e5821-117">Тип</span><span class="sxs-lookup"><span data-stu-id="e5821-117">Type</span></span> | <span data-ttu-id="e5821-118">Описание</span><span class="sxs-lookup"><span data-stu-id="e5821-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e5821-119">birthday</span><span class="sxs-lookup"><span data-stu-id="e5821-119">birthday</span></span>|<span data-ttu-id="e5821-120">String</span><span class="sxs-lookup"><span data-stu-id="e5821-120">String</span></span>|<span data-ttu-id="e5821-121">День рождения человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-121">The person's birthday.</span></span>|
|<span data-ttu-id="e5821-122">companyName</span><span class="sxs-lookup"><span data-stu-id="e5821-122">companyName</span></span>|<span data-ttu-id="e5821-123">String</span><span class="sxs-lookup"><span data-stu-id="e5821-123">String</span></span>|<span data-ttu-id="e5821-124">Название компании человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-124">The name of the person's company.</span></span>|
|<span data-ttu-id="e5821-125">department</span><span class="sxs-lookup"><span data-stu-id="e5821-125">department</span></span>|<span data-ttu-id="e5821-126">String</span><span class="sxs-lookup"><span data-stu-id="e5821-126">String</span></span>|<span data-ttu-id="e5821-127">Отдел, в котором работает человек.</span><span class="sxs-lookup"><span data-stu-id="e5821-127">The person's department.</span></span>|
|<span data-ttu-id="e5821-128">displayName</span><span class="sxs-lookup"><span data-stu-id="e5821-128">displayName</span></span>|<span data-ttu-id="e5821-129">String</span><span class="sxs-lookup"><span data-stu-id="e5821-129">String</span></span>|<span data-ttu-id="e5821-130">Отображаемое имя человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-130">The person's display name.</span></span>|
|<span data-ttu-id="e5821-131">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="e5821-131">scoredEmailAddresses</span></span>|<span data-ttu-id="e5821-132">Коллекция [scoredEmailAddress](scoredemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="e5821-132">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="e5821-133">Электронные адреса человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-133">The person's email addresses.</span></span>|
|<span data-ttu-id="e5821-134">givenName</span><span class="sxs-lookup"><span data-stu-id="e5821-134">givenName</span></span>|<span data-ttu-id="e5821-135">String</span><span class="sxs-lookup"><span data-stu-id="e5821-135">String</span></span>|<span data-ttu-id="e5821-136">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-136">The person's given name.</span></span>|
|<span data-ttu-id="e5821-137">id</span><span class="sxs-lookup"><span data-stu-id="e5821-137">id</span></span>|<span data-ttu-id="e5821-138">String</span><span class="sxs-lookup"><span data-stu-id="e5821-138">String</span></span>|<span data-ttu-id="e5821-p103">Уникальный идентификатор человека. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5821-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="e5821-141">imAddress</span><span class="sxs-lookup"><span data-stu-id="e5821-141">imAddress</span></span>|<span data-ttu-id="e5821-142">String</span><span class="sxs-lookup"><span data-stu-id="e5821-142">String</span></span>|<span data-ttu-id="e5821-p104">Адрес SIP VOIP для обмена мгновенными сообщениями для пользователя. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e5821-p104">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="e5821-145">isFavorite</span><span class="sxs-lookup"><span data-stu-id="e5821-145">isFavorite</span></span>|<span data-ttu-id="e5821-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5821-146">Boolean</span></span>|<span data-ttu-id="e5821-147">Имеет значение `true`, если пользователь добавил этого человека в список избранных.</span><span class="sxs-lookup"><span data-stu-id="e5821-147">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="e5821-148">jobTitle</span><span class="sxs-lookup"><span data-stu-id="e5821-148">jobTitle</span></span>|<span data-ttu-id="e5821-149">String</span><span class="sxs-lookup"><span data-stu-id="e5821-149">String</span></span>|<span data-ttu-id="e5821-150">Должность человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-150">The person's job title.</span></span>|
|<span data-ttu-id="e5821-151">officeLocation</span><span class="sxs-lookup"><span data-stu-id="e5821-151">officeLocation</span></span>|<span data-ttu-id="e5821-152">String</span><span class="sxs-lookup"><span data-stu-id="e5821-152">String</span></span>|<span data-ttu-id="e5821-153">Расположение офиса человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-153">The location of the person's office.</span></span>|
|<span data-ttu-id="e5821-154">personNotes</span><span class="sxs-lookup"><span data-stu-id="e5821-154">personNotes</span></span>|<span data-ttu-id="e5821-155">String</span><span class="sxs-lookup"><span data-stu-id="e5821-155">String</span></span>|<span data-ttu-id="e5821-156">Заметки в произвольной форме о человеке, созданные пользователем.</span><span class="sxs-lookup"><span data-stu-id="e5821-156">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="e5821-157">personType</span><span class="sxs-lookup"><span data-stu-id="e5821-157">personType</span></span>|[<span data-ttu-id="e5821-158">personType</span><span class="sxs-lookup"><span data-stu-id="e5821-158">personType</span></span>](persontype.md) |<span data-ttu-id="e5821-159">Тип человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-159">The type of person.</span></span>|
|<span data-ttu-id="e5821-160">phones</span><span class="sxs-lookup"><span data-stu-id="e5821-160">phones</span></span>|<span data-ttu-id="e5821-161">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="e5821-161">[phone](phone.md) collection</span></span>|<span data-ttu-id="e5821-162">Номера телефонов человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-162">The person's phone numbers.</span></span>|
|<span data-ttu-id="e5821-163">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="e5821-163">postalAddresses</span></span>|<span data-ttu-id="e5821-164">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="e5821-164">[location](location.md) collection</span></span>|<span data-ttu-id="e5821-165">Адреса человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-165">The person's addresses.</span></span>|
|<span data-ttu-id="e5821-166">profession</span><span class="sxs-lookup"><span data-stu-id="e5821-166">profession</span></span>|<span data-ttu-id="e5821-167">String</span><span class="sxs-lookup"><span data-stu-id="e5821-167">String</span></span>|<span data-ttu-id="e5821-168">Профессия человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-168">The person's profession.</span></span>|
|<span data-ttu-id="e5821-169">surname</span><span class="sxs-lookup"><span data-stu-id="e5821-169">surname</span></span>|<span data-ttu-id="e5821-170">String</span><span class="sxs-lookup"><span data-stu-id="e5821-170">String</span></span>|<span data-ttu-id="e5821-171">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-171">The person's surname.</span></span>|
|<span data-ttu-id="e5821-172">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e5821-172">userPrincipalName</span></span>|<span data-ttu-id="e5821-173">String</span><span class="sxs-lookup"><span data-stu-id="e5821-173">String</span></span>|<span data-ttu-id="e5821-p105">Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.</span><span class="sxs-lookup"><span data-stu-id="e5821-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="e5821-178">websites</span><span class="sxs-lookup"><span data-stu-id="e5821-178">websites</span></span>|<span data-ttu-id="e5821-179">Коллекция [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="e5821-179">[website](website.md) collection</span></span>|<span data-ttu-id="e5821-180">Веб-сайты человека.</span><span class="sxs-lookup"><span data-stu-id="e5821-180">The person's websites.</span></span>|
|<span data-ttu-id="e5821-181">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="e5821-181">yomiCompany</span></span>|<span data-ttu-id="e5821-182">String</span><span class="sxs-lookup"><span data-stu-id="e5821-182">String</span></span>|<span data-ttu-id="e5821-183">Название компании человека, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="e5821-183">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5821-184">Связи</span><span class="sxs-lookup"><span data-stu-id="e5821-184">Relationships</span></span>

<span data-ttu-id="e5821-185">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5821-185">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5821-186">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e5821-186">JSON representation</span></span>

<span data-ttu-id="e5821-187">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e5821-187">The following is a JSON representation of the resource.</span></span>

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

