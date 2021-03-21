---
title: Тип ресурса контракта
description: Представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2ec65433edf3a6d0ec5973c0a3bc8cf46cef00d0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962471"
---
# <a name="contract-resource-type"></a><span data-ttu-id="4ce5c-103">Тип ресурса контракта</span><span class="sxs-lookup"><span data-stu-id="4ce5c-103">Contract resource type</span></span>

<span data-ttu-id="4ce5c-104">Пространство имен: microsoft.graph представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-104">Namespace: microsoft.graph Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="4ce5c-105">**Важно:** Существует только в клиентах-партнерах.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="4ce5c-106">Клиенты-партнеры — это клиенты Azure AD, которые принадлежат партнерам Майкрософт, которые являются либо частью поставщика облачных решений [Microsoft,](https://partnercenter.microsoft.com/en-us/partner/programs)Office 365 Syndication, либо партнерской программы Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="4ce5c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="4ce5c-107">Methods</span></span>

| <span data-ttu-id="4ce5c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="4ce5c-108">Method</span></span>   | <span data-ttu-id="4ce5c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4ce5c-109">Return Type</span></span> | <span data-ttu-id="4ce5c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4ce5c-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="4ce5c-111">Получение контрактов</span><span class="sxs-lookup"><span data-stu-id="4ce5c-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="4ce5c-112">Контракт</span><span class="sxs-lookup"><span data-stu-id="4ce5c-112">Contract</span></span> |<span data-ttu-id="4ce5c-113">Чтение свойств определенного объекта контракта.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="4ce5c-114">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="4ce5c-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="4ce5c-115">Коллекция контрактов</span><span class="sxs-lookup"><span data-stu-id="4ce5c-115">Contract collection</span></span> | <span data-ttu-id="4ce5c-116">Список контрактов в клиенте-партнере.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="4ce5c-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="4ce5c-117">Properties</span></span>
| <span data-ttu-id="4ce5c-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="4ce5c-118">Property</span></span>   | <span data-ttu-id="4ce5c-119">Тип</span><span class="sxs-lookup"><span data-stu-id="4ce5c-119">Type</span></span> | <span data-ttu-id="4ce5c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4ce5c-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4ce5c-121">contractType</span><span class="sxs-lookup"><span data-stu-id="4ce5c-121">contractType</span></span>|<span data-ttu-id="4ce5c-122">String</span><span class="sxs-lookup"><span data-stu-id="4ce5c-122">String</span></span>|<span data-ttu-id="4ce5c-123">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-123">Type of contract.</span></span> <span data-ttu-id="4ce5c-124">Возможные значения:  `SyndicationPartner` , `BreadthPartner` , `ResellerPartner` .</span><span class="sxs-lookup"><span data-stu-id="4ce5c-124">Possible values are:  `SyndicationPartner`, `BreadthPartner`, `ResellerPartner`.</span></span> <span data-ttu-id="4ce5c-125">Подробнее в таблице [ниже](#contracttype-values).</span><span class="sxs-lookup"><span data-stu-id="4ce5c-125">See more in the [table below](#contracttype-values).</span></span>|
|<span data-ttu-id="4ce5c-126">customerId</span><span class="sxs-lookup"><span data-stu-id="4ce5c-126">customerId</span></span>|<span data-ttu-id="4ce5c-127">Guid</span><span class="sxs-lookup"><span data-stu-id="4ce5c-127">Guid</span></span>|<span data-ttu-id="4ce5c-128">Уникальный идентификатор клиента клиента, на который ссылается это партнерство.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-128">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="4ce5c-129">Соответствует свойству id ресурса организации клиента клиента.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-129">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="4ce5c-130">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="4ce5c-130">defaultDomainName</span></span>|<span data-ttu-id="4ce5c-131">String</span><span class="sxs-lookup"><span data-stu-id="4ce5c-131">String</span></span>|<span data-ttu-id="4ce5c-132">Копия доменного имени клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-132">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="4ce5c-133">Копия будет выполнена после того, как будет установлено партнерство с клиентом.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-133">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="4ce5c-134">Он не обновляется автоматически, если меняется имя домена клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-134">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="4ce5c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4ce5c-135">displayName</span></span>|<span data-ttu-id="4ce5c-136">String</span><span class="sxs-lookup"><span data-stu-id="4ce5c-136">String</span></span>|<span data-ttu-id="4ce5c-137">Копия отображаемого имени клиента.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-137">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="4ce5c-138">Копия будет выполнена после того, как будет установлено партнерство с клиентом.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="4ce5c-139">Оно не обновляется автоматически, если меняется имя отображения клиента.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-139">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="4ce5c-140">id</span><span class="sxs-lookup"><span data-stu-id="4ce5c-140">id</span></span>|<span data-ttu-id="4ce5c-141">String</span><span class="sxs-lookup"><span data-stu-id="4ce5c-141">String</span></span>| <span data-ttu-id="4ce5c-142">Уникальный идентификатор для партнерства.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-142">The unique identifier for the partnership.</span></span> <span data-ttu-id="4ce5c-143">Клавиша, только для чтения</span><span class="sxs-lookup"><span data-stu-id="4ce5c-143">Key, read-only</span></span> |

### <a name="contracttype-values"></a><span data-ttu-id="4ce5c-144">значения contractType</span><span class="sxs-lookup"><span data-stu-id="4ce5c-144">contractType values</span></span>

|<span data-ttu-id="4ce5c-145">Member</span><span class="sxs-lookup"><span data-stu-id="4ce5c-145">Member</span></span>|<span data-ttu-id="4ce5c-146">Описание</span><span class="sxs-lookup"><span data-stu-id="4ce5c-146">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4ce5c-147">SyndicationPartner</span><span class="sxs-lookup"><span data-stu-id="4ce5c-147">SyndicationPartner</span></span>|<span data-ttu-id="4ce5c-148">Партнер, *который исключительно перепродает* и управляет O365 и Intune для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-148">Partner that *exclusively* resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="4ce5c-149">Они перепродают и поддерживают своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-149">They resell and support their customers.</span></span>|
|<span data-ttu-id="4ce5c-150">BreadthPartner</span><span class="sxs-lookup"><span data-stu-id="4ce5c-150">BreadthPartner</span></span>|<span data-ttu-id="4ce5c-151">Партнер может оказывать административную поддержку этому клиенту.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-151">Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="4ce5c-152">Однако партнер не имеет права перепродавать клиенту.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-152">However, the partner is not allowed to resell to the customer.</span></span>|
|<span data-ttu-id="4ce5c-153">ResellerPartner</span><span class="sxs-lookup"><span data-stu-id="4ce5c-153">ResellerPartner</span></span>|<span data-ttu-id="4ce5c-154">Партнер, аналогичный партнеру синдикации, за исключением того, что у партнера нет эксклюзивного доступа к клиенту.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-154">Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="4ce5c-155">В случае синдикации клиент не может покупать дополнительные прямые подписки у Microsoft или у других партнеров.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-155">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ce5c-156">Связи</span><span class="sxs-lookup"><span data-stu-id="4ce5c-156">Relationships</span></span>
<span data-ttu-id="4ce5c-157">Нет</span><span class="sxs-lookup"><span data-stu-id="4ce5c-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4ce5c-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4ce5c-158">JSON representation</span></span>
<span data-ttu-id="4ce5c-159">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4ce5c-159">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

