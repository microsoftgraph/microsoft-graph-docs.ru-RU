---
title: Тип ресурса контракта
description: Представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 35e8cbc38fd183907c09b26c05d5c95cc140a7f5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444429"
---
# <a name="contract-resource-type"></a><span data-ttu-id="93466-103">Тип ресурса контракта</span><span class="sxs-lookup"><span data-stu-id="93466-103">Contract resource type</span></span>

<span data-ttu-id="93466-104">Пространство имен: microsoft.graph представляет существующее партнерство, которое клиент-партнер имеет с клиентом-клиентом.</span><span class="sxs-lookup"><span data-stu-id="93466-104">Namespace: microsoft.graph Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="93466-105">**Важно:** Существует только в клиентах-партнерах.</span><span class="sxs-lookup"><span data-stu-id="93466-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="93466-106">Клиенты-партнеры — это клиенты Azure AD, которые принадлежат партнерам Майкрософт, которые являются либо частью поставщика облачных решений [Microsoft,](https://partnercenter.microsoft.com/en-us/partner/programs)Office 365 Syndication, либо партнерской программы Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="93466-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="93466-107">Методы</span><span class="sxs-lookup"><span data-stu-id="93466-107">Methods</span></span>

| <span data-ttu-id="93466-108">Метод</span><span class="sxs-lookup"><span data-stu-id="93466-108">Method</span></span>   | <span data-ttu-id="93466-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="93466-109">Return Type</span></span> | <span data-ttu-id="93466-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93466-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="93466-111">Получение контрактов</span><span class="sxs-lookup"><span data-stu-id="93466-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="93466-112">Контракт</span><span class="sxs-lookup"><span data-stu-id="93466-112">Contract</span></span> |<span data-ttu-id="93466-113">Чтение свойств определенного объекта контракта.</span><span class="sxs-lookup"><span data-stu-id="93466-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="93466-114">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="93466-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="93466-115">Коллекция контрактов</span><span class="sxs-lookup"><span data-stu-id="93466-115">Contract collection</span></span> | <span data-ttu-id="93466-116">Список контрактов в клиенте-партнере.</span><span class="sxs-lookup"><span data-stu-id="93466-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="93466-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="93466-117">Properties</span></span>
| <span data-ttu-id="93466-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="93466-118">Property</span></span>   | <span data-ttu-id="93466-119">Тип</span><span class="sxs-lookup"><span data-stu-id="93466-119">Type</span></span> | <span data-ttu-id="93466-120">Описание</span><span class="sxs-lookup"><span data-stu-id="93466-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="93466-121">contractType</span><span class="sxs-lookup"><span data-stu-id="93466-121">contractType</span></span>|<span data-ttu-id="93466-122">String</span><span class="sxs-lookup"><span data-stu-id="93466-122">String</span></span>|<span data-ttu-id="93466-123">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="93466-123">Type of contract.</span></span><br><br><span data-ttu-id="93466-124">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="93466-124">Possible values are:</span></span><br> <span data-ttu-id="93466-125">*SyndicationPartner* — партнер, который исключительно перепродает и управляет O365 и Intune для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="93466-125">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="93466-126">Они перепродают и поддерживают своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="93466-126">They resell and support their customers.</span></span><br> <span data-ttu-id="93466-127">*BreadthPartner* — партнер может оказывать административную поддержку этому клиенту.</span><span class="sxs-lookup"><span data-stu-id="93466-127">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="93466-128">Однако партнер не имеет права перепродавать клиенту.</span><span class="sxs-lookup"><span data-stu-id="93466-128">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="93466-129">*ResellerPartner* — партнер, похожий на партнера по синдикации, за исключением того, что у партнера нет эксклюзивного доступа к клиенту.</span><span class="sxs-lookup"><span data-stu-id="93466-129">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="93466-130">В случае синдикации клиент не может покупать дополнительные прямые подписки у Microsoft или у других партнеров.</span><span class="sxs-lookup"><span data-stu-id="93466-130">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="93466-131">customerId</span><span class="sxs-lookup"><span data-stu-id="93466-131">customerId</span></span>|<span data-ttu-id="93466-132">Guid</span><span class="sxs-lookup"><span data-stu-id="93466-132">Guid</span></span>|<span data-ttu-id="93466-133">Уникальный идентификатор клиента клиента, на который ссылается это партнерство.</span><span class="sxs-lookup"><span data-stu-id="93466-133">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="93466-134">Соответствует свойству id ресурса организации клиента клиента.</span><span class="sxs-lookup"><span data-stu-id="93466-134">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="93466-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="93466-135">defaultDomainName</span></span>|<span data-ttu-id="93466-136">String</span><span class="sxs-lookup"><span data-stu-id="93466-136">String</span></span>|<span data-ttu-id="93466-137">Копия доменного имени клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="93466-137">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="93466-138">Копия будет выполнена после того, как будет установлено партнерство с клиентом.</span><span class="sxs-lookup"><span data-stu-id="93466-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="93466-139">Он не обновляется автоматически, если меняется имя домена клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="93466-139">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="93466-140">displayName</span><span class="sxs-lookup"><span data-stu-id="93466-140">displayName</span></span>|<span data-ttu-id="93466-141">String</span><span class="sxs-lookup"><span data-stu-id="93466-141">String</span></span>|<span data-ttu-id="93466-142">Копия отображаемого имени клиента.</span><span class="sxs-lookup"><span data-stu-id="93466-142">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="93466-143">Копия будет выполнена после того, как будет установлено партнерство с клиентом.</span><span class="sxs-lookup"><span data-stu-id="93466-143">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="93466-144">Оно не обновляется автоматически, если меняется имя отображения клиента.</span><span class="sxs-lookup"><span data-stu-id="93466-144">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="93466-145">id</span><span class="sxs-lookup"><span data-stu-id="93466-145">id</span></span>|<span data-ttu-id="93466-146">String</span><span class="sxs-lookup"><span data-stu-id="93466-146">String</span></span>| <span data-ttu-id="93466-147">Уникальный идентификатор для партнерства.</span><span class="sxs-lookup"><span data-stu-id="93466-147">The unique identifier for the partnership.</span></span> <span data-ttu-id="93466-148">Клавиша, только для чтения</span><span class="sxs-lookup"><span data-stu-id="93466-148">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="93466-149">Связи</span><span class="sxs-lookup"><span data-stu-id="93466-149">Relationships</span></span>
<span data-ttu-id="93466-150">Нет</span><span class="sxs-lookup"><span data-stu-id="93466-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="93466-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93466-151">JSON representation</span></span>
<span data-ttu-id="93466-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93466-152">Here is a JSON representation of the resource.</span></span>

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

