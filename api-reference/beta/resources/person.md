---
title: Тип ресурса person
description: Объединение сведений о человеке через почту, контакты и социальные сети. Пользователи могут быть локальными контактами, контактами из социальных сетей, каталогом вашей организации и людьми из недавних коммуникаций (таких как электронная почта и Skype).
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 4df5f82bd14ba56969c26facef82b59f3ac7e3f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521941"
---
# <a name="person-resource-type"></a><span data-ttu-id="749bb-104">Тип ресурса person</span><span class="sxs-lookup"><span data-stu-id="749bb-104">person resource type</span></span>

<span data-ttu-id="749bb-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="749bb-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="749bb-106">Объединение сведений о человеке через почту, контакты и социальные сети.</span><span class="sxs-lookup"><span data-stu-id="749bb-106">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="749bb-107">Пользователи могут быть локальными контактами, контактами из социальных сетей, каталогом вашей организации и людьми из недавних коммуникаций (таких как электронная почта и Skype).</span><span class="sxs-lookup"><span data-stu-id="749bb-107">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="749bb-108">Методы</span><span class="sxs-lookup"><span data-stu-id="749bb-108">Methods</span></span>

| <span data-ttu-id="749bb-109">Метод</span><span class="sxs-lookup"><span data-stu-id="749bb-109">Method</span></span> | <span data-ttu-id="749bb-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="749bb-110">Return Type</span></span> | <span data-ttu-id="749bb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="749bb-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="749bb-112">List people</span><span class="sxs-lookup"><span data-stu-id="749bb-112">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="749bb-113">**person**</span><span class="sxs-lookup"><span data-stu-id="749bb-113">**person**</span></span> |<span data-ttu-id="749bb-114">Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="749bb-114">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="749bb-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="749bb-115">Properties</span></span>

| <span data-ttu-id="749bb-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="749bb-116">Property</span></span> | <span data-ttu-id="749bb-117">Тип</span><span class="sxs-lookup"><span data-stu-id="749bb-117">Type</span></span> | <span data-ttu-id="749bb-118">Описание</span><span class="sxs-lookup"><span data-stu-id="749bb-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="749bb-119">birthday</span><span class="sxs-lookup"><span data-stu-id="749bb-119">birthday</span></span>|<span data-ttu-id="749bb-120">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-120">string</span></span>|<span data-ttu-id="749bb-121">День рождения человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-121">The person's birthday.</span></span>|
|<span data-ttu-id="749bb-122">companyName</span><span class="sxs-lookup"><span data-stu-id="749bb-122">companyName</span></span>|<span data-ttu-id="749bb-123">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-123">string</span></span>|<span data-ttu-id="749bb-124">Название компании человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-124">The name of the person's company.</span></span>|
|<span data-ttu-id="749bb-125">department</span><span class="sxs-lookup"><span data-stu-id="749bb-125">department</span></span>|<span data-ttu-id="749bb-126">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-126">string</span></span>|<span data-ttu-id="749bb-127">Отдел, в котором работает человек.</span><span class="sxs-lookup"><span data-stu-id="749bb-127">The person's department.</span></span>|
|<span data-ttu-id="749bb-128">displayName</span><span class="sxs-lookup"><span data-stu-id="749bb-128">displayName</span></span>|<span data-ttu-id="749bb-129">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-129">string</span></span>|<span data-ttu-id="749bb-130">Отображаемое имя человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-130">The person's display name.</span></span>|
|<span data-ttu-id="749bb-131">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="749bb-131">emailAddresses</span></span>|<span data-ttu-id="749bb-132">Коллекция [ранкедемаиладдресс](rankedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="749bb-132">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="749bb-133">Электронные адреса человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-133">The person's email addresses.</span></span>|
|<span data-ttu-id="749bb-134">givenName</span><span class="sxs-lookup"><span data-stu-id="749bb-134">givenName</span></span>|<span data-ttu-id="749bb-135">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-135">string</span></span>|<span data-ttu-id="749bb-136">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-136">The person's given name.</span></span>|
|<span data-ttu-id="749bb-137">id</span><span class="sxs-lookup"><span data-stu-id="749bb-137">id</span></span>|<span data-ttu-id="749bb-138">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-138">string</span></span>|<span data-ttu-id="749bb-139">Уникальный идентификатор человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-139">The person's unique identifier.</span></span> <span data-ttu-id="749bb-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="749bb-140">Read-only.</span></span>|
|<span data-ttu-id="749bb-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="749bb-141">isFavorite</span></span>|<span data-ttu-id="749bb-142">boolean</span><span class="sxs-lookup"><span data-stu-id="749bb-142">boolean</span></span>|<span data-ttu-id="749bb-143">Имеет значение `true`, если пользователь добавил этого человека в список избранных.</span><span class="sxs-lookup"><span data-stu-id="749bb-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="749bb-144">mailboxType</span><span class="sxs-lookup"><span data-stu-id="749bb-144">mailboxType</span></span>|<span data-ttu-id="749bb-145">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-145">string</span></span>|<span data-ttu-id="749bb-146">Тип почтового ящика, представленного адресом электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="749bb-146">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="749bb-147">officeLocation;</span><span class="sxs-lookup"><span data-stu-id="749bb-147">officeLocation</span></span>|<span data-ttu-id="749bb-148">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-148">string</span></span>|<span data-ttu-id="749bb-149">Расположение офиса человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-149">The location of the person's office.</span></span>|
|<span data-ttu-id="749bb-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="749bb-150">personNotes</span></span>|<span data-ttu-id="749bb-151">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-151">string</span></span>|<span data-ttu-id="749bb-152">Заметки в произвольной форме о человеке, созданные пользователем.</span><span class="sxs-lookup"><span data-stu-id="749bb-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="749bb-153">personType</span><span class="sxs-lookup"><span data-stu-id="749bb-153">personType</span></span>|<span data-ttu-id="749bb-154">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-154">string</span></span>|<span data-ttu-id="749bb-155">Тип лица, например список рассылки.</span><span class="sxs-lookup"><span data-stu-id="749bb-155">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="749bb-156">phones</span><span class="sxs-lookup"><span data-stu-id="749bb-156">phones</span></span>|<span data-ttu-id="749bb-157">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="749bb-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="749bb-158">Номера телефонов человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="749bb-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="749bb-159">postalAddresses</span></span>|<span data-ttu-id="749bb-160">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="749bb-160">[location](location.md) collection</span></span>|<span data-ttu-id="749bb-161">Адреса человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-161">The person's addresses.</span></span>|
|<span data-ttu-id="749bb-162">profession</span><span class="sxs-lookup"><span data-stu-id="749bb-162">profession</span></span>|<span data-ttu-id="749bb-163">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-163">string</span></span>|<span data-ttu-id="749bb-164">Профессия человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-164">The person's profession.</span></span>|
|<span data-ttu-id="749bb-165">sources</span><span class="sxs-lookup"><span data-stu-id="749bb-165">sources</span></span>|<span data-ttu-id="749bb-166">Коллекция [персондатасаурце](persondatasource.md)</span><span class="sxs-lookup"><span data-stu-id="749bb-166">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="749bb-167">Источники, из которых берутся данные пользователя, например, "каталог" или "Контакты Outlook".</span><span class="sxs-lookup"><span data-stu-id="749bb-167">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="749bb-168">surname</span><span class="sxs-lookup"><span data-stu-id="749bb-168">surname</span></span>|<span data-ttu-id="749bb-169">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-169">string</span></span>|<span data-ttu-id="749bb-170">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-170">The person's surname.</span></span>|
|<span data-ttu-id="749bb-171">title</span><span class="sxs-lookup"><span data-stu-id="749bb-171">title</span></span>|<span data-ttu-id="749bb-172">string</span><span class="sxs-lookup"><span data-stu-id="749bb-172">string</span></span>|<span data-ttu-id="749bb-173">Должность человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-173">The person's title.</span></span>|
|<span data-ttu-id="749bb-174">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="749bb-174">userPrincipalName</span></span>|<span data-ttu-id="749bb-175">string</span><span class="sxs-lookup"><span data-stu-id="749bb-175">string</span></span>|<span data-ttu-id="749bb-p104">Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.</span><span class="sxs-lookup"><span data-stu-id="749bb-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="749bb-180">websites</span><span class="sxs-lookup"><span data-stu-id="749bb-180">websites</span></span>|<span data-ttu-id="749bb-181">Коллекция [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="749bb-181">[website](website.md) collection</span></span>|<span data-ttu-id="749bb-182">Веб-сайты человека.</span><span class="sxs-lookup"><span data-stu-id="749bb-182">The person's websites.</span></span>|
|<span data-ttu-id="749bb-183">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="749bb-183">yomiCompany</span></span>|<span data-ttu-id="749bb-184">строка</span><span class="sxs-lookup"><span data-stu-id="749bb-184">string</span></span>|<span data-ttu-id="749bb-185">Название компании человека, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="749bb-185">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="749bb-186">Связи</span><span class="sxs-lookup"><span data-stu-id="749bb-186">Relationships</span></span>

<span data-ttu-id="749bb-187">Нет</span><span class="sxs-lookup"><span data-stu-id="749bb-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="749bb-188">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="749bb-188">JSON representation</span></span>

<span data-ttu-id="749bb-189">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="749bb-189">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
