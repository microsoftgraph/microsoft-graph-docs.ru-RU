---
title: Тип ресурса контракта
description: Представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: b09d773a740a82b8424a7699f959ddb38d78e1cf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444263"
---
# <a name="contract-resource-type"></a><span data-ttu-id="a20f4-103">Тип ресурса контракта</span><span class="sxs-lookup"><span data-stu-id="a20f4-103">Contract resource type</span></span>

<span data-ttu-id="a20f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a20f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a20f4-105">Представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.</span><span class="sxs-lookup"><span data-stu-id="a20f4-105">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="a20f4-106">**Важно:** Существует только в клиентах-партнерах.</span><span class="sxs-lookup"><span data-stu-id="a20f4-106">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="a20f4-107">Клиенты-партнеры — это клиенты Azure AD, которые принадлежат партнерам Майкрософт, которые являются либо частью поставщика облачных решений [Microsoft,](https://partnercenter.microsoft.com/en-us/partner/programs)Office 365 Syndication, либо партнерской программы Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="a20f4-107">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="a20f4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a20f4-108">Methods</span></span>

| <span data-ttu-id="a20f4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a20f4-109">Method</span></span>   | <span data-ttu-id="a20f4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a20f4-110">Return Type</span></span> | <span data-ttu-id="a20f4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a20f4-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a20f4-112">Получение контрактов</span><span class="sxs-lookup"><span data-stu-id="a20f4-112">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="a20f4-113">Контракт</span><span class="sxs-lookup"><span data-stu-id="a20f4-113">Contract</span></span> |<span data-ttu-id="a20f4-114">Чтение свойств определенного объекта контракта.</span><span class="sxs-lookup"><span data-stu-id="a20f4-114">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="a20f4-115">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="a20f4-115">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="a20f4-116">Коллекция контрактов</span><span class="sxs-lookup"><span data-stu-id="a20f4-116">Contract collection</span></span> | <span data-ttu-id="a20f4-117">Список контрактов в клиенте-партнере.</span><span class="sxs-lookup"><span data-stu-id="a20f4-117">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="a20f4-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a20f4-118">Properties</span></span>
| <span data-ttu-id="a20f4-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a20f4-119">Property</span></span>   | <span data-ttu-id="a20f4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a20f4-120">Type</span></span> | <span data-ttu-id="a20f4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a20f4-121">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a20f4-122">contractType</span><span class="sxs-lookup"><span data-stu-id="a20f4-122">contractType</span></span>|<span data-ttu-id="a20f4-123">String</span><span class="sxs-lookup"><span data-stu-id="a20f4-123">String</span></span>|<span data-ttu-id="a20f4-124">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="a20f4-124">Type of contract.</span></span><br><br><span data-ttu-id="a20f4-125">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="a20f4-125">Possible values are:</span></span><br> <span data-ttu-id="a20f4-126">*SyndicationPartner* — партнер, который исключительно перепродает и управляет O365 и Intune для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="a20f4-126">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="a20f4-127">Они перепродают и поддерживают своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="a20f4-127">They resell and support their customers.</span></span><br> <span data-ttu-id="a20f4-128">*BreadthPartner* — партнер может оказывать административную поддержку этому клиенту.</span><span class="sxs-lookup"><span data-stu-id="a20f4-128">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="a20f4-129">Однако партнер не имеет права перепродавать клиенту.</span><span class="sxs-lookup"><span data-stu-id="a20f4-129">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="a20f4-130">*ResellerPartner* — партнер, похожий на партнера по синдикации, за исключением того, что у партнера нет эксклюзивного доступа к клиенту.</span><span class="sxs-lookup"><span data-stu-id="a20f4-130">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="a20f4-131">В случае синдикации клиент не может покупать дополнительные прямые подписки у Microsoft или у других партнеров.</span><span class="sxs-lookup"><span data-stu-id="a20f4-131">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="a20f4-132">customerId</span><span class="sxs-lookup"><span data-stu-id="a20f4-132">customerId</span></span>|<span data-ttu-id="a20f4-133">Guid</span><span class="sxs-lookup"><span data-stu-id="a20f4-133">Guid</span></span>|<span data-ttu-id="a20f4-134">Уникальный идентификатор клиента клиента, на который ссылается это партнерство.</span><span class="sxs-lookup"><span data-stu-id="a20f4-134">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="a20f4-135">Соответствует свойству id ресурса организации клиента клиента.</span><span class="sxs-lookup"><span data-stu-id="a20f4-135">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="a20f4-136">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="a20f4-136">defaultDomainName</span></span>|<span data-ttu-id="a20f4-137">String</span><span class="sxs-lookup"><span data-stu-id="a20f4-137">String</span></span>|<span data-ttu-id="a20f4-138">Копия доменного имени клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a20f4-138">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="a20f4-139">Копия будет выполнена после того, как будет установлено партнерство с клиентом.</span><span class="sxs-lookup"><span data-stu-id="a20f4-139">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="a20f4-140">Он не обновляется автоматически, если меняется имя домена клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a20f4-140">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="a20f4-141">displayName</span><span class="sxs-lookup"><span data-stu-id="a20f4-141">displayName</span></span>|<span data-ttu-id="a20f4-142">String</span><span class="sxs-lookup"><span data-stu-id="a20f4-142">String</span></span>|<span data-ttu-id="a20f4-143">Копия отображаемого имени клиента.</span><span class="sxs-lookup"><span data-stu-id="a20f4-143">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="a20f4-144">Копия будет выполнена после того, как будет установлено партнерство с клиентом.</span><span class="sxs-lookup"><span data-stu-id="a20f4-144">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="a20f4-145">Оно не обновляется автоматически, если меняется имя отображения клиента.</span><span class="sxs-lookup"><span data-stu-id="a20f4-145">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="a20f4-146">id</span><span class="sxs-lookup"><span data-stu-id="a20f4-146">id</span></span>|<span data-ttu-id="a20f4-147">String</span><span class="sxs-lookup"><span data-stu-id="a20f4-147">String</span></span>| <span data-ttu-id="a20f4-148">Уникальный идентификатор для партнерства.</span><span class="sxs-lookup"><span data-stu-id="a20f4-148">The unique identifier for the partnership.</span></span> <span data-ttu-id="a20f4-149">Клавиша, только для чтения</span><span class="sxs-lookup"><span data-stu-id="a20f4-149">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="a20f4-150">Связи</span><span class="sxs-lookup"><span data-stu-id="a20f4-150">Relationships</span></span>
<span data-ttu-id="a20f4-151">Нет</span><span class="sxs-lookup"><span data-stu-id="a20f4-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a20f4-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a20f4-152">JSON representation</span></span>
<span data-ttu-id="a20f4-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a20f4-153">Here is a JSON representation of the resource.</span></span>

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


