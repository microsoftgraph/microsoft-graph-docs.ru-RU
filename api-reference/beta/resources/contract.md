---
title: Тип ресурса contract
description: Представляет существующее партнерство между клиентом партнера и клиентом пользователя.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6309dfc370d414ccb66065fe4048d7cece51f018
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509702"
---
# <a name="contract-resource-type"></a><span data-ttu-id="7ad10-103">Тип ресурса contract</span><span class="sxs-lookup"><span data-stu-id="7ad10-103">Contract resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ad10-104">Представляет существующее партнерство между клиентом партнера и клиентом пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ad10-104">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="7ad10-p101">**Важно!** Существует только в клиентах партнеров. Клиенты партнеров — это клиенты Azure AD, которые принадлежат партнерам корпорации Майкрософт, являющимся [поставщиками облачных решений (Майкрософт)](https://partnercenter.microsoft.com/en-us/partner/programs), участниками программы синдикации Office 365 или участниками партнерской программы Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="7ad10-p101">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="7ad10-107">Методы</span><span class="sxs-lookup"><span data-stu-id="7ad10-107">Methods</span></span>

| <span data-ttu-id="7ad10-108">Метод</span><span class="sxs-lookup"><span data-stu-id="7ad10-108">Method</span></span>   | <span data-ttu-id="7ad10-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ad10-109">Return Type</span></span> | <span data-ttu-id="7ad10-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ad10-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="7ad10-111">Получение contract</span><span class="sxs-lookup"><span data-stu-id="7ad10-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="7ad10-112">contract</span><span class="sxs-lookup"><span data-stu-id="7ad10-112">Contract</span></span> |<span data-ttu-id="7ad10-113">Чтение свойств определенных объектов contract.</span><span class="sxs-lookup"><span data-stu-id="7ad10-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="7ad10-114">Перечисление объектов contract</span><span class="sxs-lookup"><span data-stu-id="7ad10-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="7ad10-115">Коллекция contract</span><span class="sxs-lookup"><span data-stu-id="7ad10-115">Contract collection</span></span> | <span data-ttu-id="7ad10-116">Перечисление объектов contract в клиенте партнера.</span><span class="sxs-lookup"><span data-stu-id="7ad10-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ad10-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ad10-117">Properties</span></span>
| <span data-ttu-id="7ad10-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ad10-118">Property</span></span>   | <span data-ttu-id="7ad10-119">Тип</span><span class="sxs-lookup"><span data-stu-id="7ad10-119">Type</span></span> | <span data-ttu-id="7ad10-120">Описание</span><span class="sxs-lookup"><span data-stu-id="7ad10-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7ad10-121">contractType</span><span class="sxs-lookup"><span data-stu-id="7ad10-121">contractType</span></span>|<span data-ttu-id="7ad10-122">String</span><span class="sxs-lookup"><span data-stu-id="7ad10-122">String</span></span>|<span data-ttu-id="7ad10-123">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="7ad10-123">Type of contract.</span></span><br><br><span data-ttu-id="7ad10-124">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="7ad10-124">Possible values are:</span></span><br> <span data-ttu-id="7ad10-p102">*SyndicationPartner*. Партнер, имеющий исключительные права на перепродажу Office 365 и Intune для этого пользователя, а также управление ими. Такие партнеры выполняют перепродажу и предоставляют пользователям поддержку.</span><span class="sxs-lookup"><span data-stu-id="7ad10-p102">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="7ad10-p103">*BreadthPartner*. Партнер может предоставлять пользователю административную поддержку. Прав на перепродажу этот партнер не имеет.</span><span class="sxs-lookup"><span data-stu-id="7ad10-p103">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="7ad10-p104">*ResellerPartner*. Этот тип партнеров аналогичен SyndicationPartner, но не предусматривает эксклюзивного доступа к клиенту. В случае SyndicationPartner пользователь не может приобретать дополнительные подписки непосредственно у корпорации Майкрософт или у других партнеров.</span><span class="sxs-lookup"><span data-stu-id="7ad10-p104">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="7ad10-131">customerId</span><span class="sxs-lookup"><span data-stu-id="7ad10-131">customerId</span></span>|<span data-ttu-id="7ad10-132">Guid</span><span class="sxs-lookup"><span data-stu-id="7ad10-132">Guid</span></span>|<span data-ttu-id="7ad10-p105">Уникальный идентификатор для клиента пользователя, указываемый в случае партнерства. Соответствует свойству id для ресурса организации клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ad10-p105">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="7ad10-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="7ad10-135">defaultDomainName</span></span>|<span data-ttu-id="7ad10-136">String</span><span class="sxs-lookup"><span data-stu-id="7ad10-136">String</span></span>|<span data-ttu-id="7ad10-p106">Копия стандартного доменного имени для клиента пользователя. Копия создается при установлении партнерства с пользователем. Она не обновляется автоматически, если изменяется стандартное доменное имя для клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ad10-p106">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="7ad10-140">displayName</span><span class="sxs-lookup"><span data-stu-id="7ad10-140">displayName</span></span>|<span data-ttu-id="7ad10-141">String</span><span class="sxs-lookup"><span data-stu-id="7ad10-141">String</span></span>|<span data-ttu-id="7ad10-p107">Копия отображаемого имени клиента пользователя. Копия создается при установлении партнерства с пользователем. Она не обновляется автоматически, если изменяется отображаемое имя клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ad10-p107">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="7ad10-145">id</span><span class="sxs-lookup"><span data-stu-id="7ad10-145">id</span></span>|<span data-ttu-id="7ad10-146">String</span><span class="sxs-lookup"><span data-stu-id="7ad10-146">String</span></span>| <span data-ttu-id="7ad10-p108">Уникальный идентификатор, заданный для партнерства. Ключ, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ad10-p108">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="7ad10-149">Связи</span><span class="sxs-lookup"><span data-stu-id="7ad10-149">Relationships</span></span>
<span data-ttu-id="7ad10-150">Нет</span><span class="sxs-lookup"><span data-stu-id="7ad10-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7ad10-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ad10-151">JSON representation</span></span>
<span data-ttu-id="7ad10-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ad10-152">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/contract.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
