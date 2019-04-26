---
title: Тип ресурса контракта
description: Представляет существующую связь, с которой клиент-партнер имеет клиент.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0d8da7c20705796cdb612ad1a24c4d03ce160447
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341214"
---
# <a name="contract-resource-type"></a><span data-ttu-id="88ad5-103">Тип ресурса контракта</span><span class="sxs-lookup"><span data-stu-id="88ad5-103">Contract resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88ad5-104">Представляет существующую связь, с которой клиент-партнер имеет клиент.</span><span class="sxs-lookup"><span data-stu-id="88ad5-104">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="88ad5-105">**Важно!** Существует только в партнерских клиентах.</span><span class="sxs-lookup"><span data-stu-id="88ad5-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="88ad5-106">Партнерские клиенты — это клиенты Azure AD, которые принадлежат партнерам Майкрософт, которые входят в состав [поставщика облачНых решений корпорации Майкрософт](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 для синдикации или партнерских программ Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="88ad5-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="88ad5-107">Методы</span><span class="sxs-lookup"><span data-stu-id="88ad5-107">Methods</span></span>

| <span data-ttu-id="88ad5-108">Метод</span><span class="sxs-lookup"><span data-stu-id="88ad5-108">Method</span></span>   | <span data-ttu-id="88ad5-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="88ad5-109">Return Type</span></span> | <span data-ttu-id="88ad5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="88ad5-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="88ad5-111">Получение контрактов</span><span class="sxs-lookup"><span data-stu-id="88ad5-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="88ad5-112">Суммы</span><span class="sxs-lookup"><span data-stu-id="88ad5-112">Contract</span></span> |<span data-ttu-id="88ad5-113">Считывание свойств определенного объекта Contract.</span><span class="sxs-lookup"><span data-stu-id="88ad5-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="88ad5-114">Список контрактов</span><span class="sxs-lookup"><span data-stu-id="88ad5-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="88ad5-115">Коллекция контрактов</span><span class="sxs-lookup"><span data-stu-id="88ad5-115">Contract collection</span></span> | <span data-ttu-id="88ad5-116">Список контрактов в клиенте партнера.</span><span class="sxs-lookup"><span data-stu-id="88ad5-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="88ad5-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="88ad5-117">Properties</span></span>
| <span data-ttu-id="88ad5-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="88ad5-118">Property</span></span>   | <span data-ttu-id="88ad5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="88ad5-119">Type</span></span> | <span data-ttu-id="88ad5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="88ad5-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="88ad5-121">Контракттипе</span><span class="sxs-lookup"><span data-stu-id="88ad5-121">contractType</span></span>|<span data-ttu-id="88ad5-122">String</span><span class="sxs-lookup"><span data-stu-id="88ad5-122">String</span></span>|<span data-ttu-id="88ad5-123">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="88ad5-123">Type of contract.</span></span><br><br><span data-ttu-id="88ad5-124">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="88ad5-124">Possible values are:</span></span><br> <span data-ttu-id="88ad5-125">*Синдикатионпартнер* -партнер, который исключительно перепродает и управляет O365 и Intune для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="88ad5-125">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="88ad5-126">Они перепродают и поддерживают своих клиентов.</span><span class="sxs-lookup"><span data-stu-id="88ad5-126">They resell and support their customers.</span></span><br> <span data-ttu-id="88ad5-127">*Бреадспартнер* -Partner предоставляет возможность администрирования для этого клиента.</span><span class="sxs-lookup"><span data-stu-id="88ad5-127">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="88ad5-128">Тем не менее, партнеру не разрешено перепродавать клиенту.</span><span class="sxs-lookup"><span data-stu-id="88ad5-128">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="88ad5-129">*Реселлерпартнер* -партнер, аналогичный партнеру синдикации, за исключением того, что партнер не имеет монопольного доступа к клиенту.</span><span class="sxs-lookup"><span data-stu-id="88ad5-129">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="88ad5-130">В случае синдикации клиент не может покупать дополнительные подписки от Майкрософт или других партнеров.</span><span class="sxs-lookup"><span data-stu-id="88ad5-130">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="88ad5-131">customerId</span><span class="sxs-lookup"><span data-stu-id="88ad5-131">customerId</span></span>|<span data-ttu-id="88ad5-132">GUID</span><span class="sxs-lookup"><span data-stu-id="88ad5-132">Guid</span></span>|<span data-ttu-id="88ad5-133">Уникальный идентификатор клиента клиента, на который ссылается это партнерство.</span><span class="sxs-lookup"><span data-stu-id="88ad5-133">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="88ad5-134">Соответствует свойству ID ресурса организации клиента клиента.</span><span class="sxs-lookup"><span data-stu-id="88ad5-134">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="88ad5-135">Дефаултдомаиннаме</span><span class="sxs-lookup"><span data-stu-id="88ad5-135">defaultDomainName</span></span>|<span data-ttu-id="88ad5-136">String</span><span class="sxs-lookup"><span data-stu-id="88ad5-136">String</span></span>|<span data-ttu-id="88ad5-137">Копия доменного имени клиента, используемого по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="88ad5-137">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="88ad5-138">Копия создается при установке связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="88ad5-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="88ad5-139">Он не обновляется автоматически, если изменяется доменное имя клиента по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="88ad5-139">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="88ad5-140">displayName</span><span class="sxs-lookup"><span data-stu-id="88ad5-140">displayName</span></span>|<span data-ttu-id="88ad5-141">String</span><span class="sxs-lookup"><span data-stu-id="88ad5-141">String</span></span>|<span data-ttu-id="88ad5-142">Копия отображаемого имени клиента.</span><span class="sxs-lookup"><span data-stu-id="88ad5-142">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="88ad5-143">Копия создается при установке связи с клиентом.</span><span class="sxs-lookup"><span data-stu-id="88ad5-143">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="88ad5-144">Он не обновляется автоматически при изменении отображаемого имени клиента клиента.</span><span class="sxs-lookup"><span data-stu-id="88ad5-144">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="88ad5-145">id</span><span class="sxs-lookup"><span data-stu-id="88ad5-145">id</span></span>|<span data-ttu-id="88ad5-146">String</span><span class="sxs-lookup"><span data-stu-id="88ad5-146">String</span></span>| <span data-ttu-id="88ad5-147">Уникальный идентификатор партнерства.</span><span class="sxs-lookup"><span data-stu-id="88ad5-147">The unique identifier for the partnership.</span></span> <span data-ttu-id="88ad5-148">Ключ, только для чтения</span><span class="sxs-lookup"><span data-stu-id="88ad5-148">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="88ad5-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="88ad5-149">Relationships</span></span>
<span data-ttu-id="88ad5-150">Нет</span><span class="sxs-lookup"><span data-stu-id="88ad5-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="88ad5-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88ad5-151">JSON representation</span></span>
<span data-ttu-id="88ad5-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88ad5-152">Here is a JSON representation of the resource.</span></span>

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
