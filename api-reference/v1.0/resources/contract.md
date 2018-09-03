# <a name="contract-resource-type"></a><span data-ttu-id="35529-101">Тип ресурса contract</span><span class="sxs-lookup"><span data-stu-id="35529-101">Contract resource type</span></span>
<span data-ttu-id="35529-102">Представляет существующее партнерство между клиентом партнера и клиентом пользователя.</span><span class="sxs-lookup"><span data-stu-id="35529-102">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="35529-p101">**Важно!** Существует только в клиентах партнеров. Клиенты партнеров — это клиенты Azure AD, которые принадлежат партнерам корпорации Майкрософт, являющимся [поставщиками облачных решений (Майкрософт)](https://partnercenter.microsoft.com/en-us/partner/programs), участниками программы синдикации Office 365 или участниками партнерской программы Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="35529-p101">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="35529-105">Методы</span><span class="sxs-lookup"><span data-stu-id="35529-105">Methods</span></span>

| <span data-ttu-id="35529-106">Метод</span><span class="sxs-lookup"><span data-stu-id="35529-106">Method</span></span>   | <span data-ttu-id="35529-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="35529-107">Return Type</span></span> | <span data-ttu-id="35529-108">Описание</span><span class="sxs-lookup"><span data-stu-id="35529-108">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="35529-109">Получение contract</span><span class="sxs-lookup"><span data-stu-id="35529-109">Get contract</span></span>](../api/contract_get.md) | <span data-ttu-id="35529-110">contract</span><span class="sxs-lookup"><span data-stu-id="35529-110">Contract</span></span> |<span data-ttu-id="35529-111">Чтение свойств определенных объектов contract.</span><span class="sxs-lookup"><span data-stu-id="35529-111">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="35529-112">Перечисление объектов contract</span><span class="sxs-lookup"><span data-stu-id="35529-112">List contracts</span></span>](../api/contract_list.md) | <span data-ttu-id="35529-113">Коллекция contract</span><span class="sxs-lookup"><span data-stu-id="35529-113">Contract collection</span></span> | <span data-ttu-id="35529-114">Перечисление объектов contract в клиенте партнера.</span><span class="sxs-lookup"><span data-stu-id="35529-114">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="35529-115">Свойства</span><span class="sxs-lookup"><span data-stu-id="35529-115">Properties</span></span>
| <span data-ttu-id="35529-116">Свойство</span><span class="sxs-lookup"><span data-stu-id="35529-116">Property</span></span>   | <span data-ttu-id="35529-117">Тип</span><span class="sxs-lookup"><span data-stu-id="35529-117">Type</span></span> | <span data-ttu-id="35529-118">Описание</span><span class="sxs-lookup"><span data-stu-id="35529-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="35529-119">contractType</span><span class="sxs-lookup"><span data-stu-id="35529-119">contractType</span></span>|<span data-ttu-id="35529-120">Строка​</span><span class="sxs-lookup"><span data-stu-id="35529-120">String</span></span>|<span data-ttu-id="35529-121">Тип контракта.</span><span class="sxs-lookup"><span data-stu-id="35529-121">Type of contract.</span></span><br><br><span data-ttu-id="35529-122">Возможные значения:</span><span class="sxs-lookup"><span data-stu-id="35529-122">Possible values are:</span></span><br> <span data-ttu-id="35529-p102">*SyndicationPartner*. Партнер, имеющий исключительные права на перепродажу Office 365 и Intune для этого пользователя, а также управление ими. Такие партнеры выполняют перепродажу и предоставляют пользователям поддержку.</span><span class="sxs-lookup"><span data-stu-id="35529-p102">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="35529-p103">*BreadthPartner*. Партнер может предоставлять пользователю административную поддержку. Прав на перепродажу этот партнер не имеет.</span><span class="sxs-lookup"><span data-stu-id="35529-p103">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="35529-p104">*ResellerPartner*. Этот тип партнеров аналогичен SyndicationPartner, но не предусматривает эксклюзивного доступа к клиенту. В случае SyndicationPartner пользователь не может приобретать дополнительные подписки непосредственно у корпорации Майкрософт или у других партнеров.</span><span class="sxs-lookup"><span data-stu-id="35529-p104">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="35529-129">customerId</span><span class="sxs-lookup"><span data-stu-id="35529-129">customerId</span></span>|<span data-ttu-id="35529-130">Guid</span><span class="sxs-lookup"><span data-stu-id="35529-130">Guid</span></span>|<span data-ttu-id="35529-p105">Уникальный идентификатор для клиента пользователя, указываемый в случае партнерства. Соответствует свойству id для ресурса организации клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="35529-p105">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="35529-133">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="35529-133">defaultDomainName</span></span>|<span data-ttu-id="35529-134">Строка​</span><span class="sxs-lookup"><span data-stu-id="35529-134">String</span></span>|<span data-ttu-id="35529-p106">Копия стандартного доменного имени для клиента пользователя. Копия создается при установлении партнерства с пользователем. Она не обновляется автоматически, если изменяется стандартное доменное имя для клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="35529-p106">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="35529-138">displayName</span><span class="sxs-lookup"><span data-stu-id="35529-138">displayName</span></span>|<span data-ttu-id="35529-139">Строка​</span><span class="sxs-lookup"><span data-stu-id="35529-139">String</span></span>|<span data-ttu-id="35529-p107">Копия отображаемого имени клиента пользователя. Копия создается при установлении партнерства с пользователем. Она не обновляется автоматически, если изменяется отображаемое имя клиента пользователя.</span><span class="sxs-lookup"><span data-stu-id="35529-p107">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="35529-143">id</span><span class="sxs-lookup"><span data-stu-id="35529-143">id</span></span>|<span data-ttu-id="35529-144">Строка​</span><span class="sxs-lookup"><span data-stu-id="35529-144">String</span></span>| <span data-ttu-id="35529-p108">Уникальный идентификатор, заданный для партнерства. Ключ, только для чтения.</span><span class="sxs-lookup"><span data-stu-id="35529-p108">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="35529-147">Связи</span><span class="sxs-lookup"><span data-stu-id="35529-147">Relationships</span></span>
<span data-ttu-id="35529-148">Нет</span><span class="sxs-lookup"><span data-stu-id="35529-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="35529-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35529-149">JSON representation</span></span>
<span data-ttu-id="35529-150">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35529-150">Here is a JSON representation of the resource.</span></span>

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