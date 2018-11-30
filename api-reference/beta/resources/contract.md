---
title: Тип ресурса contract
description: Представляет существующее партнерство между клиентом партнера и клиентом пользователя.
ms.openlocfilehash: 7465a54c735b7c1e6f9d5ecb8bf79420b8de45c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082008"
---
# <a name="contract-resource-type"></a><span data-ttu-id="5a9a2-103">Тип ресурса contract</span><span class="sxs-lookup"><span data-stu-id="5a9a2-103">Contract resource type</span></span>

> <span data-ttu-id="5a9a2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a9a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a9a2-106">Представляет существующее партнерство между клиентом партнера и клиентом пользователя.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-106">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="5a9a2-p102">**Важно!** Существует только в клиентах партнеров. Клиенты партнеров — это клиенты Azure AD, которые принадлежат партнерам корпорации Майкрософт, являющимся [поставщиками облачных решений (Майкрософт)](https://partnercenter.microsoft.com/en-us/partner/programs), участниками программы синдикации Office 365 или участниками партнерской программы Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-p102">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="5a9a2-109">Методы</span><span class="sxs-lookup"><span data-stu-id="5a9a2-109">Methods</span></span>

| <span data-ttu-id="5a9a2-110">Метод</span><span class="sxs-lookup"><span data-stu-id="5a9a2-110">Method</span></span>   | <span data-ttu-id="5a9a2-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5a9a2-111">Return Type</span></span> | <span data-ttu-id="5a9a2-112">Описание</span><span class="sxs-lookup"><span data-stu-id="5a9a2-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="5a9a2-113">Получение contract</span><span class="sxs-lookup"><span data-stu-id="5a9a2-113">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="5a9a2-114">contract</span><span class="sxs-lookup"><span data-stu-id="5a9a2-114">Contract</span></span> |<span data-ttu-id="5a9a2-115">Чтение свойств определенных объектов contract.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-115">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="5a9a2-116">Перечисление объектов contract</span><span class="sxs-lookup"><span data-stu-id="5a9a2-116">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="5a9a2-117">Коллекция contract</span><span class="sxs-lookup"><span data-stu-id="5a9a2-117">Contract collection</span></span> | <span data-ttu-id="5a9a2-118">Перечисление объектов contract в клиенте партнера.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-118">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="5a9a2-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="5a9a2-119">Properties</span></span>
| <span data-ttu-id="5a9a2-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a9a2-120">Property</span></span>   | <span data-ttu-id="5a9a2-121">Тип</span><span class="sxs-lookup"><span data-stu-id="5a9a2-121">Type</span></span> | <span data-ttu-id="5a9a2-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5a9a2-122">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5a9a2-123">contractType</span><span class="sxs-lookup"><span data-stu-id="5a9a2-123">contractType</span></span>|<span data-ttu-id="5a9a2-124">String</span><span class="sxs-lookup"><span data-stu-id="5a9a2-124">String</span></span>|<span data-ttu-id="5a9a2-125">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-125">Type of contract.</span></span><br><br><span data-ttu-id="5a9a2-126">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="5a9a2-126">Possible values are:</span></span><br> <span data-ttu-id="5a9a2-p103">*SyndicationPartner*. Партнер, имеющий исключительные права на перепродажу Office 365 и Intune для этого пользователя, а также управление ими. Такие партнеры выполняют перепродажу и предоставляют пользователям поддержку.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-p103">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="5a9a2-p104">*BreadthPartner*. Партнер может предоставлять пользователю административную поддержку. Прав на перепродажу этот партнер не имеет.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-p104">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="5a9a2-p105">*ResellerPartner*. Этот тип партнеров аналогичен SyndicationPartner, но не предусматривает эксклюзивного доступа к клиенту. В случае SyndicationPartner пользователь не может приобретать дополнительные подписки непосредственно у корпорации Майкрософт или у других партнеров.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-p105">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="5a9a2-133">customerId</span><span class="sxs-lookup"><span data-stu-id="5a9a2-133">customerId</span></span>|<span data-ttu-id="5a9a2-134">Guid</span><span class="sxs-lookup"><span data-stu-id="5a9a2-134">Guid</span></span>|<span data-ttu-id="5a9a2-p106">Уникальный идентификатор для клиента пользователя, указываемый в случае партнерства. Соответствует свойству id для ресурса организации клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-p106">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="5a9a2-137">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="5a9a2-137">defaultDomainName</span></span>|<span data-ttu-id="5a9a2-138">String</span><span class="sxs-lookup"><span data-stu-id="5a9a2-138">String</span></span>|<span data-ttu-id="5a9a2-p107">Копия стандартного доменного имени для клиента пользователя. Копия создается при установлении партнерства с пользователем. Она не обновляется автоматически, если изменяется стандартное доменное имя для клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-p107">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="5a9a2-142">displayName</span><span class="sxs-lookup"><span data-stu-id="5a9a2-142">displayName</span></span>|<span data-ttu-id="5a9a2-143">String</span><span class="sxs-lookup"><span data-stu-id="5a9a2-143">String</span></span>|<span data-ttu-id="5a9a2-p108">Копия отображаемого имени клиента пользователя. Копия создается при установлении партнерства с пользователем. Она не обновляется автоматически, если изменяется отображаемое имя клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-p108">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="5a9a2-147">id</span><span class="sxs-lookup"><span data-stu-id="5a9a2-147">id</span></span>|<span data-ttu-id="5a9a2-148">String</span><span class="sxs-lookup"><span data-stu-id="5a9a2-148">String</span></span>| <span data-ttu-id="5a9a2-p109">Уникальный идентификатор, заданный для партнерства. Ключ, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-p109">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="5a9a2-151">Связи</span><span class="sxs-lookup"><span data-stu-id="5a9a2-151">Relationships</span></span>
<span data-ttu-id="5a9a2-152">Нет</span><span class="sxs-lookup"><span data-stu-id="5a9a2-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5a9a2-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5a9a2-153">JSON representation</span></span>
<span data-ttu-id="5a9a2-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5a9a2-154">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->