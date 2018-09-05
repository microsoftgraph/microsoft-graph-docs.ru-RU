# <a name="onpremisesextensionattributes-resource-type"></a><span data-ttu-id="e3d75-101">Тип ресурса onPremisesExtensionAttributes</span><span class="sxs-lookup"><span data-stu-id="e3d75-101">onPremisesExtensionAttributes resource type</span></span>

<span data-ttu-id="e3d75-102">Свойство **onPremisesExtensionAttributes** сущности[пользователя](user.md) содержит пятнадцать настраиваемых свойств атрибута расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-102">The **onPremisesExtensionAttributes** property of the [user](user.md) entity contains fifteen custom extension attribute properties.</span></span> <span data-ttu-id="e3d75-103">Для пользователя с **onPremisesSyncEnabled** этот набор свойств создается в локальной службе Active Directory, синхронизируется с Azure AD и доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-103">For an **onPremisesSyncEnabled** user, this set of properties is mastered in on-premises Active Directory and synchronized to Azure AD, and is read-only.</span></span> <span data-ttu-id="e3d75-104">Для пользователей только в облаке (где **onPremisesSyncEnabled** имеет значение false) эти свойства могут быть установлены во время создания или обновления.</span><span class="sxs-lookup"><span data-stu-id="e3d75-104">For a cloud-only user (where **onPremisesSyncEnabled** is false), these properties may be set during creation or update.</span></span>


## <a name="properties"></a><span data-ttu-id="e3d75-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="e3d75-105">Properties</span></span>
| <span data-ttu-id="e3d75-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="e3d75-106">Property</span></span>     | <span data-ttu-id="e3d75-107">Тип</span><span class="sxs-lookup"><span data-stu-id="e3d75-107">Type</span></span>   |<span data-ttu-id="e3d75-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e3d75-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3d75-109">extensionAttribute1</span><span class="sxs-lookup"><span data-stu-id="e3d75-109">extensionAttribute1</span></span>|<span data-ttu-id="e3d75-110">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-110">String</span></span>| <span data-ttu-id="e3d75-111">Первый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-111">First customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-112">extensionAttribute2</span><span class="sxs-lookup"><span data-stu-id="e3d75-112">extensionAttribute2</span></span>|<span data-ttu-id="e3d75-113">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-113">String</span></span>| <span data-ttu-id="e3d75-114">Второй настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-114">Second customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-115">extensionAttribute3</span><span class="sxs-lookup"><span data-stu-id="e3d75-115">extensionAttribute3</span></span>|<span data-ttu-id="e3d75-116">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-116">String</span></span>| <span data-ttu-id="e3d75-117">Третий настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-117">Third customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-118">extensionAttribute4</span><span class="sxs-lookup"><span data-stu-id="e3d75-118">extensionAttribute4</span></span>|<span data-ttu-id="e3d75-119">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-119">String</span></span>| <span data-ttu-id="e3d75-120">Четвертый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-120">Fourth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-121">extensionAttribute5</span><span class="sxs-lookup"><span data-stu-id="e3d75-121">extensionAttribute5</span></span>|<span data-ttu-id="e3d75-122">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-122">String</span></span>| <span data-ttu-id="e3d75-123">Пятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-123">Fifth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-124">extensionAttribute6</span><span class="sxs-lookup"><span data-stu-id="e3d75-124">extensionAttribute6</span></span>|<span data-ttu-id="e3d75-125">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-125">String</span></span>| <span data-ttu-id="e3d75-126">Шестой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-126">Sixth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-127">extensionAttribute7</span><span class="sxs-lookup"><span data-stu-id="e3d75-127">extensionAttribute7</span></span>|<span data-ttu-id="e3d75-128">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-128">String</span></span>| <span data-ttu-id="e3d75-129">Седьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-129">Seventh customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-130">extensionAttribute8</span><span class="sxs-lookup"><span data-stu-id="e3d75-130">extensionAttribute8</span></span>|<span data-ttu-id="e3d75-131">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-131">String</span></span>| <span data-ttu-id="e3d75-132">Восьмой настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-132">Eighth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-133">extensionAttribute9</span><span class="sxs-lookup"><span data-stu-id="e3d75-133">extensionAttribute9</span></span>|<span data-ttu-id="e3d75-134">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-134">String</span></span>| <span data-ttu-id="e3d75-135">Девятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-135">Ninth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-136">extensionAttribute10</span><span class="sxs-lookup"><span data-stu-id="e3d75-136">extensionAttribute10</span></span>|<span data-ttu-id="e3d75-137">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-137">String</span></span>| <span data-ttu-id="e3d75-138">Десятый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-138">Tenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-139">extensionAttribute11</span><span class="sxs-lookup"><span data-stu-id="e3d75-139">extensionAttribute11</span></span>|<span data-ttu-id="e3d75-140">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-140">String</span></span>| <span data-ttu-id="e3d75-141">Одиннадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-141">Eleventh customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-142">extensionAttribute12</span><span class="sxs-lookup"><span data-stu-id="e3d75-142">extensionAttribute12</span></span>|<span data-ttu-id="e3d75-143">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-143">String</span></span>| <span data-ttu-id="e3d75-144">Двенадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-144">Twelfth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-145">extensionAttribute13</span><span class="sxs-lookup"><span data-stu-id="e3d75-145">extensionAttribute13</span></span>|<span data-ttu-id="e3d75-146">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-146">String</span></span>| <span data-ttu-id="e3d75-147">Тринадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-147">Thirteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-148">extensionAttribute14</span><span class="sxs-lookup"><span data-stu-id="e3d75-148">extensionAttribute14</span></span>|<span data-ttu-id="e3d75-149">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-149">String</span></span>| <span data-ttu-id="e3d75-150">Четырнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-150">Fourteenth customizable extension attribute.</span></span> |
|<span data-ttu-id="e3d75-151">extensionAttribute15</span><span class="sxs-lookup"><span data-stu-id="e3d75-151">extensionAttribute15</span></span>|<span data-ttu-id="e3d75-152">String</span><span class="sxs-lookup"><span data-stu-id="e3d75-152">String</span></span>| <span data-ttu-id="e3d75-153">Пятнадцатый настраиваемый атрибут расширения.</span><span class="sxs-lookup"><span data-stu-id="e3d75-153">Fifteenth customizable extension attribute.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e3d75-154">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e3d75-154">JSON representation</span></span>

<span data-ttu-id="e3d75-155">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e3d75-155">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
}-->


```json
{
      "extensionAttribute1": "string",
      "extensionAttribute2": "string",
      "extensionAttribute3": "string",
      "extensionAttribute4": "string",
      "extensionAttribute5": "string",
      "extensionAttribute6": "string",
      "extensionAttribute7": "string",
      "extensionAttribute8": "string",
      "extensionAttribute9": "string",
      "extensionAttribute10": "string",
      "extensionAttribute11": "string",
      "extensionAttribute12": "string",
      "extensionAttribute13": "string",
      "extensionAttribute14": "string",
      "extensionAttribute15": "string"
  }

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesExtensionAttributes resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->