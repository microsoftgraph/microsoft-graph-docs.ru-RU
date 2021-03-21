---
title: Тип ресурса контракта
description: Представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d1c573b43587ef5213f876b6532358fe5465f84b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962646"
---
# <a name="contract-resource-type"></a><span data-ttu-id="3daf8-103">Тип ресурса контракта</span><span class="sxs-lookup"><span data-stu-id="3daf8-103">Contract resource type</span></span>

<span data-ttu-id="3daf8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3daf8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3daf8-105">Представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.</span><span class="sxs-lookup"><span data-stu-id="3daf8-105">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="3daf8-106">**Важно:** Существует только в клиентах-партнерах.</span><span class="sxs-lookup"><span data-stu-id="3daf8-106">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="3daf8-107">Клиенты-партнеры — это клиенты Azure AD, которые принадлежат партнерам Майкрософт, которые являются либо частью поставщика облачных решений [Microsoft,](https://partnercenter.microsoft.com/en-us/partner/programs)Office 365 Syndication, либо партнерской программы Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="3daf8-107">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="3daf8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="3daf8-108">Methods</span></span>

| <span data-ttu-id="3daf8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="3daf8-109">Method</span></span>   | <span data-ttu-id="3daf8-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3daf8-110">Return Type</span></span> | <span data-ttu-id="3daf8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3daf8-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="3daf8-112">Получение контрактов</span><span class="sxs-lookup"><span data-stu-id="3daf8-112">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="3daf8-113">Контракт</span><span class="sxs-lookup"><span data-stu-id="3daf8-113">Contract</span></span> |<span data-ttu-id="3daf8-114">Чтение свойств определенного объекта контракта.</span><span class="sxs-lookup"><span data-stu-id="3daf8-114">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="3daf8-115">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="3daf8-115">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="3daf8-116">Коллекция контрактов</span><span class="sxs-lookup"><span data-stu-id="3daf8-116">Contract collection</span></span> | <span data-ttu-id="3daf8-117">Список контрактов в клиенте-партнере.</span><span class="sxs-lookup"><span data-stu-id="3daf8-117">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="3daf8-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="3daf8-118">Properties</span></span>
| <span data-ttu-id="3daf8-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="3daf8-119">Property</span></span>   | <span data-ttu-id="3daf8-120">Тип</span><span class="sxs-lookup"><span data-stu-id="3daf8-120">Type</span></span> | <span data-ttu-id="3daf8-121">Описание</span><span class="sxs-lookup"><span data-stu-id="3daf8-121">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="3daf8-122">contractType</span><span class="sxs-lookup"><span data-stu-id="3daf8-122">contractType</span></span>|<span data-ttu-id="3daf8-123">Строка</span><span class="sxs-lookup"><span data-stu-id="3daf8-123">String</span></span>|<span data-ttu-id="3daf8-124">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="3daf8-124">Type of contract.</span></span> <span data-ttu-id="3daf8-125">Возможные значения:  `SyndicationPartner` , `BreadthPartner` , `ResellerPartner` .</span><span class="sxs-lookup"><span data-stu-id="3daf8-125">Possible values are:  `SyndicationPartner`, `BreadthPartner`, `ResellerPartner`.</span></span> <span data-ttu-id="3daf8-126">Подробнее в таблице [ниже](#contracttype-values).</span><span class="sxs-lookup"><span data-stu-id="3daf8-126">See more in the [table below](#contracttype-values).</span></span> |
|<span data-ttu-id="3daf8-127">customerId</span><span class="sxs-lookup"><span data-stu-id="3daf8-127">customerId</span></span>|<span data-ttu-id="3daf8-128">Guid</span><span class="sxs-lookup"><span data-stu-id="3daf8-128">Guid</span></span>|<span data-ttu-id="3daf8-129">Уникальный идентификатор клиента клиента, на который ссылается это партнерство.</span><span class="sxs-lookup"><span data-stu-id="3daf8-129">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="3daf8-130">Соответствует свойству id ресурса организации клиента клиента.</span><span class="sxs-lookup"><span data-stu-id="3daf8-130">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="3daf8-131">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="3daf8-131">defaultDomainName</span></span>|<span data-ttu-id="3daf8-132">Строка</span><span class="sxs-lookup"><span data-stu-id="3daf8-132">String</span></span>|<span data-ttu-id="3daf8-133">Копия доменного имени клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3daf8-133">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="3daf8-134">Копия будет выполнена после того, как будет установлено партнерство с клиентом.</span><span class="sxs-lookup"><span data-stu-id="3daf8-134">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="3daf8-135">Он не обновляется автоматически, если меняется имя домена клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3daf8-135">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="3daf8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3daf8-136">displayName</span></span>|<span data-ttu-id="3daf8-137">Строка</span><span class="sxs-lookup"><span data-stu-id="3daf8-137">String</span></span>|<span data-ttu-id="3daf8-138">Копия отображаемого имени клиента.</span><span class="sxs-lookup"><span data-stu-id="3daf8-138">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="3daf8-139">Копия будет выполнена после того, как будет установлено партнерство с клиентом.</span><span class="sxs-lookup"><span data-stu-id="3daf8-139">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="3daf8-140">Оно не обновляется автоматически, если меняется имя отображения клиента.</span><span class="sxs-lookup"><span data-stu-id="3daf8-140">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="3daf8-141">id</span><span class="sxs-lookup"><span data-stu-id="3daf8-141">id</span></span>|<span data-ttu-id="3daf8-142">Строка</span><span class="sxs-lookup"><span data-stu-id="3daf8-142">String</span></span>| <span data-ttu-id="3daf8-143">Уникальный идентификатор для партнерства.</span><span class="sxs-lookup"><span data-stu-id="3daf8-143">The unique identifier for the partnership.</span></span> <span data-ttu-id="3daf8-144">Клавиша, только для чтения</span><span class="sxs-lookup"><span data-stu-id="3daf8-144">Key, read-only</span></span> |

### <a name="contracttype-values"></a><span data-ttu-id="3daf8-145">значения contractType</span><span class="sxs-lookup"><span data-stu-id="3daf8-145">contractType values</span></span>

|<span data-ttu-id="3daf8-146">Member</span><span class="sxs-lookup"><span data-stu-id="3daf8-146">Member</span></span>|<span data-ttu-id="3daf8-147">Описание</span><span class="sxs-lookup"><span data-stu-id="3daf8-147">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3daf8-148">SyndicationPartner</span><span class="sxs-lookup"><span data-stu-id="3daf8-148">SyndicationPartner</span></span>|<span data-ttu-id="3daf8-149">Партнер, *который исключительно перепродает* и управляет O365 и Intune для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="3daf8-149">Partner that *exclusively* resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="3daf8-150">Они перепродают и поддерживают своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="3daf8-150">They resell and support their customers.</span></span>|
|<span data-ttu-id="3daf8-151">BreadthPartner</span><span class="sxs-lookup"><span data-stu-id="3daf8-151">BreadthPartner</span></span>|<span data-ttu-id="3daf8-152">Партнер может оказывать административную поддержку этому клиенту.</span><span class="sxs-lookup"><span data-stu-id="3daf8-152">Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="3daf8-153">Однако партнер не имеет права перепродавать клиенту.</span><span class="sxs-lookup"><span data-stu-id="3daf8-153">However, the partner is not allowed to resell to the customer.</span></span>|
|<span data-ttu-id="3daf8-154">ResellerPartner</span><span class="sxs-lookup"><span data-stu-id="3daf8-154">ResellerPartner</span></span>|<span data-ttu-id="3daf8-155">Партнер, аналогичный партнеру синдикации, за исключением того, что у партнера нет эксклюзивного доступа к клиенту.</span><span class="sxs-lookup"><span data-stu-id="3daf8-155">Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="3daf8-156">В случае синдикации клиент не может покупать дополнительные прямые подписки у Microsoft или у других партнеров.</span><span class="sxs-lookup"><span data-stu-id="3daf8-156">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3daf8-157">Связи</span><span class="sxs-lookup"><span data-stu-id="3daf8-157">Relationships</span></span>
<span data-ttu-id="3daf8-158">Нет</span><span class="sxs-lookup"><span data-stu-id="3daf8-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3daf8-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3daf8-159">JSON representation</span></span>
<span data-ttu-id="3daf8-160">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3daf8-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
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
<!--
{
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


