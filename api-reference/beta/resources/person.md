---
title: Тип ресурса person
description: Объединение сведений о человеке через почту, контакты и социальные сети. Пользователи могут быть локальными контактами, контактами из социальных сетей, каталогом вашей организации и людьми из недавних коммуникаций (таких как электронная почта и Skype).
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 32a2c9905ab52e9b229bb8673fb4a84d90a706ac
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561476"
---
# <a name="person-resource-type"></a><span data-ttu-id="2a6f8-104">Тип ресурса person</span><span class="sxs-lookup"><span data-stu-id="2a6f8-104">person resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a6f8-105">Объединение сведений о человеке через почту, контакты и социальные сети.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-105">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="2a6f8-106">Пользователи могут быть локальными контактами, контактами из социальных сетей, каталогом вашей организации и людьми из недавних коммуникаций (таких как электронная почта и Skype).</span><span class="sxs-lookup"><span data-stu-id="2a6f8-106">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="2a6f8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2a6f8-107">Methods</span></span>

| <span data-ttu-id="2a6f8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2a6f8-108">Method</span></span> | <span data-ttu-id="2a6f8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="2a6f8-109">Return Type</span></span> | <span data-ttu-id="2a6f8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2a6f8-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a6f8-111">List people</span><span class="sxs-lookup"><span data-stu-id="2a6f8-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="2a6f8-112">**person**</span><span class="sxs-lookup"><span data-stu-id="2a6f8-112">**person**</span></span> |<span data-ttu-id="2a6f8-113">Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="2a6f8-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="2a6f8-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a6f8-114">Properties</span></span>

| <span data-ttu-id="2a6f8-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a6f8-115">Property</span></span> | <span data-ttu-id="2a6f8-116">Тип</span><span class="sxs-lookup"><span data-stu-id="2a6f8-116">Type</span></span> | <span data-ttu-id="2a6f8-117">Описание</span><span class="sxs-lookup"><span data-stu-id="2a6f8-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2a6f8-118">birthday</span><span class="sxs-lookup"><span data-stu-id="2a6f8-118">birthday</span></span>|<span data-ttu-id="2a6f8-119">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-119">string</span></span>|<span data-ttu-id="2a6f8-120">День рождения человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-120">The person's birthday.</span></span>|
|<span data-ttu-id="2a6f8-121">companyName</span><span class="sxs-lookup"><span data-stu-id="2a6f8-121">companyName</span></span>|<span data-ttu-id="2a6f8-122">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-122">string</span></span>|<span data-ttu-id="2a6f8-123">Название компании человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-123">The name of the person's company.</span></span>|
|<span data-ttu-id="2a6f8-124">department</span><span class="sxs-lookup"><span data-stu-id="2a6f8-124">department</span></span>|<span data-ttu-id="2a6f8-125">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-125">string</span></span>|<span data-ttu-id="2a6f8-126">Отдел, в котором работает человек.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-126">The person's department.</span></span>|
|<span data-ttu-id="2a6f8-127">displayName</span><span class="sxs-lookup"><span data-stu-id="2a6f8-127">displayName</span></span>|<span data-ttu-id="2a6f8-128">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-128">string</span></span>|<span data-ttu-id="2a6f8-129">Отображаемое имя человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-129">The person's display name.</span></span>|
|<span data-ttu-id="2a6f8-130">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="2a6f8-130">emailAddresses</span></span>|<span data-ttu-id="2a6f8-131">Коллекция [ранкедемаиладдресс](rankedemailaddress.md)</span><span class="sxs-lookup"><span data-stu-id="2a6f8-131">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="2a6f8-132">Электронные адреса человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-132">The person's email addresses.</span></span>|
|<span data-ttu-id="2a6f8-133">givenName</span><span class="sxs-lookup"><span data-stu-id="2a6f8-133">givenName</span></span>|<span data-ttu-id="2a6f8-134">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-134">string</span></span>|<span data-ttu-id="2a6f8-135">Имя человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-135">The person's given name.</span></span>|
|<span data-ttu-id="2a6f8-136">id</span><span class="sxs-lookup"><span data-stu-id="2a6f8-136">id</span></span>|<span data-ttu-id="2a6f8-137">строка</span><span class="sxs-lookup"><span data-stu-id="2a6f8-137">string</span></span>|<span data-ttu-id="2a6f8-138">Уникальный идентификатор человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-138">The person's unique identifier.</span></span> <span data-ttu-id="2a6f8-139">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-139">Read-only.</span></span>|
|<span data-ttu-id="2a6f8-140">isFavorite</span><span class="sxs-lookup"><span data-stu-id="2a6f8-140">isFavorite</span></span>|<span data-ttu-id="2a6f8-141">boolean</span><span class="sxs-lookup"><span data-stu-id="2a6f8-141">boolean</span></span>|<span data-ttu-id="2a6f8-142">Имеет значение `true`, если пользователь добавил этого человека в список избранных.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-142">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="2a6f8-143">mailboxType</span><span class="sxs-lookup"><span data-stu-id="2a6f8-143">mailboxType</span></span>|<span data-ttu-id="2a6f8-144">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-144">string</span></span>|<span data-ttu-id="2a6f8-145">Тип почтового ящика, представленного адресом электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-145">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="2a6f8-146">officeLocation</span><span class="sxs-lookup"><span data-stu-id="2a6f8-146">officeLocation</span></span>|<span data-ttu-id="2a6f8-147">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-147">string</span></span>|<span data-ttu-id="2a6f8-148">Расположение офиса человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-148">The location of the person's office.</span></span>|
|<span data-ttu-id="2a6f8-149">personNotes</span><span class="sxs-lookup"><span data-stu-id="2a6f8-149">personNotes</span></span>|<span data-ttu-id="2a6f8-150">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-150">string</span></span>|<span data-ttu-id="2a6f8-151">Заметки в произвольной форме о человеке, созданные пользователем.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-151">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="2a6f8-152">personType</span><span class="sxs-lookup"><span data-stu-id="2a6f8-152">personType</span></span>|<span data-ttu-id="2a6f8-153">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-153">string</span></span>|<span data-ttu-id="2a6f8-154">Тип лица, например список рассылки.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-154">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="2a6f8-155">phones</span><span class="sxs-lookup"><span data-stu-id="2a6f8-155">phones</span></span>|<span data-ttu-id="2a6f8-156">Коллекция [phone](phone.md)</span><span class="sxs-lookup"><span data-stu-id="2a6f8-156">[phone](phone.md) collection</span></span>|<span data-ttu-id="2a6f8-157">Номера телефонов человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-157">The person's phone numbers.</span></span>|
|<span data-ttu-id="2a6f8-158">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="2a6f8-158">postalAddresses</span></span>|<span data-ttu-id="2a6f8-159">Коллекция [location](location.md)</span><span class="sxs-lookup"><span data-stu-id="2a6f8-159">[location](location.md) collection</span></span>|<span data-ttu-id="2a6f8-160">Адреса человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-160">The person's addresses.</span></span>|
|<span data-ttu-id="2a6f8-161">profession</span><span class="sxs-lookup"><span data-stu-id="2a6f8-161">profession</span></span>|<span data-ttu-id="2a6f8-162">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-162">string</span></span>|<span data-ttu-id="2a6f8-163">Профессия человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-163">The person's profession.</span></span>|
|<span data-ttu-id="2a6f8-164">sources</span><span class="sxs-lookup"><span data-stu-id="2a6f8-164">sources</span></span>|<span data-ttu-id="2a6f8-165">Коллекция [персондатасаурце](persondatasource.md)</span><span class="sxs-lookup"><span data-stu-id="2a6f8-165">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="2a6f8-166">Источники, из которых берутся данные пользователя, например, "каталог" или "Контакты Outlook".</span><span class="sxs-lookup"><span data-stu-id="2a6f8-166">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="2a6f8-167">surname</span><span class="sxs-lookup"><span data-stu-id="2a6f8-167">surname</span></span>|<span data-ttu-id="2a6f8-168">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-168">string</span></span>|<span data-ttu-id="2a6f8-169">Фамилия человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-169">The person's surname.</span></span>|
|<span data-ttu-id="2a6f8-170">title</span><span class="sxs-lookup"><span data-stu-id="2a6f8-170">title</span></span>|<span data-ttu-id="2a6f8-171">строка</span><span class="sxs-lookup"><span data-stu-id="2a6f8-171">string</span></span>|<span data-ttu-id="2a6f8-172">Должность человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-172">The person's title.</span></span>|
|<span data-ttu-id="2a6f8-173">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2a6f8-173">userPrincipalName</span></span>|<span data-ttu-id="2a6f8-174">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-174">string</span></span>|<span data-ttu-id="2a6f8-p104">Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="2a6f8-179">websites</span><span class="sxs-lookup"><span data-stu-id="2a6f8-179">websites</span></span>|<span data-ttu-id="2a6f8-180">Коллекция [website](website.md)</span><span class="sxs-lookup"><span data-stu-id="2a6f8-180">[website](website.md) collection</span></span>|<span data-ttu-id="2a6f8-181">Веб-сайты человека.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-181">The person's websites.</span></span>|
|<span data-ttu-id="2a6f8-182">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="2a6f8-182">yomiCompany</span></span>|<span data-ttu-id="2a6f8-183">string</span><span class="sxs-lookup"><span data-stu-id="2a6f8-183">string</span></span>|<span data-ttu-id="2a6f8-184">Название компании человека, записанное так, как оно звучит по-японски.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-184">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a6f8-185">Отношения</span><span class="sxs-lookup"><span data-stu-id="2a6f8-185">Relationships</span></span>

<span data-ttu-id="2a6f8-186">Нет</span><span class="sxs-lookup"><span data-stu-id="2a6f8-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a6f8-187">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a6f8-187">JSON representation</span></span>

<span data-ttu-id="2a6f8-188">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a6f8-188">Here is a JSON representation of the resource.</span></span>

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
