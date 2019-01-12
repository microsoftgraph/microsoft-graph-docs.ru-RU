---
title: Тип ресурса person
description: Объединенные данные о сотруднике из всех почты, контакты и социальными сетями. Пользователи могут быть локального контактов, контакты из социальных сетей, вашей организации каталогов и людей из последних коммуникаций (например, электронной почты и Скайп).
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 7f0f3c71769d2ad8927f634b065253cf118316b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929384"
---
# <a name="person-resource-type"></a><span data-ttu-id="3639e-104">Тип ресурса person</span><span class="sxs-lookup"><span data-stu-id="3639e-104">person resource type</span></span>

> <span data-ttu-id="3639e-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3639e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3639e-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3639e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3639e-107">Объединенные данные о сотруднике из всех почты, контакты и социальными сетями.</span><span class="sxs-lookup"><span data-stu-id="3639e-107">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="3639e-108">Пользователи могут быть локального контактов, контакты из социальных сетей, вашей организации каталогов и людей из последних коммуникаций (например, электронной почты и Скайп).</span><span class="sxs-lookup"><span data-stu-id="3639e-108">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="3639e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3639e-109">Methods</span></span>

| <span data-ttu-id="3639e-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3639e-110">Method</span></span> | <span data-ttu-id="3639e-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3639e-111">Return Type</span></span> | <span data-ttu-id="3639e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3639e-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="3639e-113">List people</span><span class="sxs-lookup"><span data-stu-id="3639e-113">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="3639e-114">**person**</span><span class="sxs-lookup"><span data-stu-id="3639e-114">**person**</span></span> |<span data-ttu-id="3639e-115">Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="3639e-115">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="3639e-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="3639e-116">Properties</span></span>

| <span data-ttu-id="3639e-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="3639e-117">Property</span></span> | <span data-ttu-id="3639e-118">Тип</span><span class="sxs-lookup"><span data-stu-id="3639e-118">Type</span></span> | <span data-ttu-id="3639e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="3639e-119">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3639e-120">birthday</span><span class="sxs-lookup"><span data-stu-id="3639e-120">birthday</span></span>|<span data-ttu-id="3639e-121">string</span><span class="sxs-lookup"><span data-stu-id="3639e-121">string</span></span>|<span data-ttu-id="3639e-122">День рождения человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-122">The person's birthday.</span></span>|
|<span data-ttu-id="3639e-123">companyName</span><span class="sxs-lookup"><span data-stu-id="3639e-123">companyName</span></span>|<span data-ttu-id="3639e-124">string</span><span class="sxs-lookup"><span data-stu-id="3639e-124">string</span></span>|<span data-ttu-id="3639e-125">Название компании человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-125">The name of the person's company.</span></span>|
|<span data-ttu-id="3639e-126">department</span><span class="sxs-lookup"><span data-stu-id="3639e-126">department</span></span>|<span data-ttu-id="3639e-127">string</span><span class="sxs-lookup"><span data-stu-id="3639e-127">string</span></span>|<span data-ttu-id="3639e-128">Отдел, в котором работает человек.</span><span class="sxs-lookup"><span data-stu-id="3639e-128">The person's department.</span></span>|
|<span data-ttu-id="3639e-129">displayName</span><span class="sxs-lookup"><span data-stu-id="3639e-129">displayName</span></span>|<span data-ttu-id="3639e-130">строка</span><span class="sxs-lookup"><span data-stu-id="3639e-130">string</span></span>|<span data-ttu-id="3639e-131">Отображаемое имя человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-131">The person's display name.</span></span>|
|<span data-ttu-id="3639e-132">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="3639e-132">emailAddresses</span></span>|<span data-ttu-id="3639e-133">[rankedEmailAddress](rankedemailaddress.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3639e-133">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="3639e-134">Электронные адреса человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-134">The person's email addresses.</span></span>|
|<span data-ttu-id="3639e-135">givenName</span><span class="sxs-lookup"><span data-stu-id="3639e-135">givenName</span></span>|<span data-ttu-id="3639e-136">string</span><span class="sxs-lookup"><span data-stu-id="3639e-136">string</span></span>|<span data-ttu-id="3639e-137">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-137">The person's given name.</span></span>|
|<span data-ttu-id="3639e-138">id</span><span class="sxs-lookup"><span data-stu-id="3639e-138">id</span></span>|<span data-ttu-id="3639e-139">строка</span><span class="sxs-lookup"><span data-stu-id="3639e-139">string</span></span>|<span data-ttu-id="3639e-p104">Уникальный идентификатор человека. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3639e-p104">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="3639e-142">isFavorite</span><span class="sxs-lookup"><span data-stu-id="3639e-142">isFavorite</span></span>|<span data-ttu-id="3639e-143">boolean</span><span class="sxs-lookup"><span data-stu-id="3639e-143">boolean</span></span>|<span data-ttu-id="3639e-144">Имеет значение `true`, если пользователь добавил этого человека в список избранных.</span><span class="sxs-lookup"><span data-stu-id="3639e-144">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="3639e-145">mailboxType</span><span class="sxs-lookup"><span data-stu-id="3639e-145">mailboxType</span></span>|<span data-ttu-id="3639e-146">string</span><span class="sxs-lookup"><span data-stu-id="3639e-146">string</span></span>|<span data-ttu-id="3639e-147">Тип почтового ящика, представленного адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="3639e-147">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="3639e-148">officeLocation;</span><span class="sxs-lookup"><span data-stu-id="3639e-148">officeLocation</span></span>|<span data-ttu-id="3639e-149">string</span><span class="sxs-lookup"><span data-stu-id="3639e-149">string</span></span>|<span data-ttu-id="3639e-150">Расположение офиса человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-150">The location of the person's office.</span></span>|
|<span data-ttu-id="3639e-151">personNotes</span><span class="sxs-lookup"><span data-stu-id="3639e-151">personNotes</span></span>|<span data-ttu-id="3639e-152">string</span><span class="sxs-lookup"><span data-stu-id="3639e-152">string</span></span>|<span data-ttu-id="3639e-153">Заметки в произвольной форме о человеке, созданные пользователем.</span><span class="sxs-lookup"><span data-stu-id="3639e-153">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="3639e-154">personType</span><span class="sxs-lookup"><span data-stu-id="3639e-154">personType</span></span>|<span data-ttu-id="3639e-155">string</span><span class="sxs-lookup"><span data-stu-id="3639e-155">string</span></span>|<span data-ttu-id="3639e-156">Тип лица, например списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="3639e-156">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="3639e-157">phones</span><span class="sxs-lookup"><span data-stu-id="3639e-157">phones</span></span>|<span data-ttu-id="3639e-158">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="3639e-158">[phone](phone.md) collection</span></span>|<span data-ttu-id="3639e-159">Номера телефонов человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-159">The person's phone numbers.</span></span>|
|<span data-ttu-id="3639e-160">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="3639e-160">postalAddresses</span></span>|<span data-ttu-id="3639e-161">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="3639e-161">[location](location.md) collection</span></span>|<span data-ttu-id="3639e-162">Адреса человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-162">The person's addresses.</span></span>|
|<span data-ttu-id="3639e-163">profession</span><span class="sxs-lookup"><span data-stu-id="3639e-163">profession</span></span>|<span data-ttu-id="3639e-164">string</span><span class="sxs-lookup"><span data-stu-id="3639e-164">string</span></span>|<span data-ttu-id="3639e-165">Профессия человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-165">The person's profession.</span></span>|
|<span data-ttu-id="3639e-166">sources</span><span class="sxs-lookup"><span data-stu-id="3639e-166">sources</span></span>|<span data-ttu-id="3639e-167">[personDataSource](persondatasource.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="3639e-167">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="3639e-168">Источники пользователя данные, поступающие из, например, каталога или контактов Outlook.</span><span class="sxs-lookup"><span data-stu-id="3639e-168">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="3639e-169">surname</span><span class="sxs-lookup"><span data-stu-id="3639e-169">surname</span></span>|<span data-ttu-id="3639e-170">string</span><span class="sxs-lookup"><span data-stu-id="3639e-170">string</span></span>|<span data-ttu-id="3639e-171">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-171">The person's surname.</span></span>|
|<span data-ttu-id="3639e-172">должности.</span><span class="sxs-lookup"><span data-stu-id="3639e-172">title</span></span>|<span data-ttu-id="3639e-173">строка</span><span class="sxs-lookup"><span data-stu-id="3639e-173">string</span></span>|<span data-ttu-id="3639e-174">Должность пользователя.</span><span class="sxs-lookup"><span data-stu-id="3639e-174">The person's title.</span></span>|
|<span data-ttu-id="3639e-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3639e-175">userPrincipalName</span></span>|<span data-ttu-id="3639e-176">string</span><span class="sxs-lookup"><span data-stu-id="3639e-176">string</span></span>|<span data-ttu-id="3639e-p105">Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.</span><span class="sxs-lookup"><span data-stu-id="3639e-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="3639e-181">websites</span><span class="sxs-lookup"><span data-stu-id="3639e-181">websites</span></span>|<span data-ttu-id="3639e-182">Коллекция [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="3639e-182">[website](website.md) collection</span></span>|<span data-ttu-id="3639e-183">Веб-сайты человека.</span><span class="sxs-lookup"><span data-stu-id="3639e-183">The person's websites.</span></span>|
|<span data-ttu-id="3639e-184">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="3639e-184">yomiCompany</span></span>|<span data-ttu-id="3639e-185">string</span><span class="sxs-lookup"><span data-stu-id="3639e-185">string</span></span>|<span data-ttu-id="3639e-186">Название компании человека, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="3639e-186">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3639e-187">Связи</span><span class="sxs-lookup"><span data-stu-id="3639e-187">Relationships</span></span>

<span data-ttu-id="3639e-188">Нет</span><span class="sxs-lookup"><span data-stu-id="3639e-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3639e-189">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3639e-189">JSON representation</span></span>

<span data-ttu-id="3639e-190">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3639e-190">Here is a JSON representation of the resource.</span></span>

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
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
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
