---
title: Тип ресурса контракта
description: Представляет существующую связь, с которой клиент-партнер имеет клиент.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7727309f146d434f817d1797a782813f136311c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016816"
---
# <a name="contract-resource-type"></a><span data-ttu-id="77924-103">Тип ресурса контракта</span><span class="sxs-lookup"><span data-stu-id="77924-103">Contract resource type</span></span>

<span data-ttu-id="77924-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77924-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77924-105">Представляет существующую связь, с которой клиент-партнер имеет клиент.</span><span class="sxs-lookup"><span data-stu-id="77924-105">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="77924-106">**Важно!** Существует только в партнерских клиентах.</span><span class="sxs-lookup"><span data-stu-id="77924-106">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="77924-107">Партнерские клиенты — это клиенты Azure AD, которые принадлежат партнерам Майкрософт, которые входят в состав [поставщика облачных решений корпорации Майкрософт](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 для синдикации или партнерских программ Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="77924-107">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="77924-108">Методы</span><span class="sxs-lookup"><span data-stu-id="77924-108">Methods</span></span>

| <span data-ttu-id="77924-109">Метод</span><span class="sxs-lookup"><span data-stu-id="77924-109">Method</span></span>   | <span data-ttu-id="77924-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="77924-110">Return Type</span></span> | <span data-ttu-id="77924-111">Описание</span><span class="sxs-lookup"><span data-stu-id="77924-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="77924-112">Получение контрактов</span><span class="sxs-lookup"><span data-stu-id="77924-112">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="77924-113">Суммы</span><span class="sxs-lookup"><span data-stu-id="77924-113">Contract</span></span> |<span data-ttu-id="77924-114">Считывание свойств определенного объекта Contract.</span><span class="sxs-lookup"><span data-stu-id="77924-114">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="77924-115">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="77924-115">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="77924-116">Коллекция контрактов</span><span class="sxs-lookup"><span data-stu-id="77924-116">Contract collection</span></span> | <span data-ttu-id="77924-117">Список контрактов в клиенте партнера.</span><span class="sxs-lookup"><span data-stu-id="77924-117">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="77924-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="77924-118">Properties</span></span>
| <span data-ttu-id="77924-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="77924-119">Property</span></span>   | <span data-ttu-id="77924-120">Тип</span><span class="sxs-lookup"><span data-stu-id="77924-120">Type</span></span> | <span data-ttu-id="77924-121">Описание</span><span class="sxs-lookup"><span data-stu-id="77924-121">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="77924-122">контракттипе</span><span class="sxs-lookup"><span data-stu-id="77924-122">contractType</span></span>|<span data-ttu-id="77924-123">String</span><span class="sxs-lookup"><span data-stu-id="77924-123">String</span></span>|<span data-ttu-id="77924-124">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="77924-124">Type of contract.</span></span><br><br><span data-ttu-id="77924-125">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="77924-125">Possible values are:</span></span><br> <span data-ttu-id="77924-126">*Синдикатионпартнер* -партнер, который исключительно перепродает и управляет O365 и Intune для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="77924-126">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="77924-127">Они перепродают и поддерживают своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="77924-127">They resell and support their customers.</span></span><br> <span data-ttu-id="77924-128">*Бреадспартнер* -Partner предоставляет возможность администрирования для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="77924-128">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="77924-129">Тем не менее, партнеру не разрешено перепродавать клиенту.</span><span class="sxs-lookup"><span data-stu-id="77924-129">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="77924-130">*Реселлерпартнер* -партнер, аналогичный партнеру синдикации, за исключением того, что партнер не имеет монопольного доступа к клиенту.</span><span class="sxs-lookup"><span data-stu-id="77924-130">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="77924-131">В случае синдикации клиент не может покупать дополнительные подписки от Майкрософт или других партнеров.</span><span class="sxs-lookup"><span data-stu-id="77924-131">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="77924-132">customerId</span><span class="sxs-lookup"><span data-stu-id="77924-132">customerId</span></span>|<span data-ttu-id="77924-133">Guid</span><span class="sxs-lookup"><span data-stu-id="77924-133">Guid</span></span>|<span data-ttu-id="77924-134">Уникальный идентификатор клиента клиента, на который ссылается это партнерство.</span><span class="sxs-lookup"><span data-stu-id="77924-134">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="77924-135">Соответствует свойству ID ресурса организации клиента клиента.</span><span class="sxs-lookup"><span data-stu-id="77924-135">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="77924-136">дефаултдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="77924-136">defaultDomainName</span></span>|<span data-ttu-id="77924-137">String</span><span class="sxs-lookup"><span data-stu-id="77924-137">String</span></span>|<span data-ttu-id="77924-138">Копия доменного имени клиента, используемого по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="77924-138">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="77924-139">Копия создается при установке связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="77924-139">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="77924-140">Он не обновляется автоматически, если изменяется доменное имя клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="77924-140">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="77924-141">displayName</span><span class="sxs-lookup"><span data-stu-id="77924-141">displayName</span></span>|<span data-ttu-id="77924-142">String</span><span class="sxs-lookup"><span data-stu-id="77924-142">String</span></span>|<span data-ttu-id="77924-143">Копия отображаемого имени клиента.</span><span class="sxs-lookup"><span data-stu-id="77924-143">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="77924-144">Копия создается при установке связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="77924-144">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="77924-145">Он не обновляется автоматически при изменении отображаемого имени клиента клиента.</span><span class="sxs-lookup"><span data-stu-id="77924-145">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="77924-146">id</span><span class="sxs-lookup"><span data-stu-id="77924-146">id</span></span>|<span data-ttu-id="77924-147">String</span><span class="sxs-lookup"><span data-stu-id="77924-147">String</span></span>| <span data-ttu-id="77924-148">Уникальный идентификатор партнерства.</span><span class="sxs-lookup"><span data-stu-id="77924-148">The unique identifier for the partnership.</span></span> <span data-ttu-id="77924-149">Ключ, только для чтения</span><span class="sxs-lookup"><span data-stu-id="77924-149">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="77924-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="77924-150">Relationships</span></span>
<span data-ttu-id="77924-151">Нет</span><span class="sxs-lookup"><span data-stu-id="77924-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="77924-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77924-152">JSON representation</span></span>
<span data-ttu-id="77924-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77924-153">Here is a JSON representation of the resource.</span></span>

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


