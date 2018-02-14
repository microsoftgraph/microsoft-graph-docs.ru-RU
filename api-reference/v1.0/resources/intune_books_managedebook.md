# <a name="managedebook-resource-type"></a><span data-ttu-id="92c2d-101">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="92c2d-101">managedEBook resource type</span></span>

> <span data-ttu-id="92c2d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="92c2d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92c2d-103">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-103">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="92c2d-104">Методы</span><span class="sxs-lookup"><span data-stu-id="92c2d-104">Methods</span></span>
|<span data-ttu-id="92c2d-105">Метод</span><span class="sxs-lookup"><span data-stu-id="92c2d-105">Method</span></span>|<span data-ttu-id="92c2d-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="92c2d-106">Return Type</span></span>|<span data-ttu-id="92c2d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="92c2d-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="92c2d-108">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="92c2d-108">List managedEBooks</span></span>](../api/intune_books_managedebook_list.md)|<span data-ttu-id="92c2d-109">Коллекция [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="92c2d-109">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="92c2d-110">Список свойств и связей объектов [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="92c2d-110">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>|
|[<span data-ttu-id="92c2d-111">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="92c2d-111">Get managedEBook</span></span>](../api/intune_books_managedebook_get.md)|[<span data-ttu-id="92c2d-112">managedEBook</span><span class="sxs-lookup"><span data-stu-id="92c2d-112">managedEBook</span></span>](../resources/intune_books_managedebook.md)|<span data-ttu-id="92c2d-113">Чтение свойств и связей объекта [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="92c2d-113">Read properties and relationships of [plannerPlanDetails](../resources/intune_books_managedebook.md) object.</span></span>|
|[<span data-ttu-id="92c2d-114">действие назначения</span><span class="sxs-lookup"><span data-stu-id="92c2d-114">assign action</span></span>](../api/intune_books_managedebook_assign.md)|<span data-ttu-id="92c2d-115">Нет</span><span class="sxs-lookup"><span data-stu-id="92c2d-115">None</span></span>|<span data-ttu-id="92c2d-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="92c2d-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="92c2d-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="92c2d-117">Properties</span></span>
|<span data-ttu-id="92c2d-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="92c2d-118">Property</span></span>|<span data-ttu-id="92c2d-119">Тип</span><span class="sxs-lookup"><span data-stu-id="92c2d-119">Type</span></span>|<span data-ttu-id="92c2d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="92c2d-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92c2d-121">id</span><span class="sxs-lookup"><span data-stu-id="92c2d-121">id</span></span>|<span data-ttu-id="92c2d-122">String</span><span class="sxs-lookup"><span data-stu-id="92c2d-122">String</span></span>|<span data-ttu-id="92c2d-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="92c2d-123">Key of the setting.</span></span>|
|<span data-ttu-id="92c2d-124">displayName</span><span class="sxs-lookup"><span data-stu-id="92c2d-124">displayName</span></span>|<span data-ttu-id="92c2d-125">String</span><span class="sxs-lookup"><span data-stu-id="92c2d-125">String</span></span>|<span data-ttu-id="92c2d-126">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-126">Name of the folder.</span></span>|
|<span data-ttu-id="92c2d-127">description</span><span class="sxs-lookup"><span data-stu-id="92c2d-127">description</span></span>|<span data-ttu-id="92c2d-128">String</span><span class="sxs-lookup"><span data-stu-id="92c2d-128">String</span></span>|<span data-ttu-id="92c2d-129">Описание.</span><span class="sxs-lookup"><span data-stu-id="92c2d-129">Description</span></span>|
|<span data-ttu-id="92c2d-130">publisher</span><span class="sxs-lookup"><span data-stu-id="92c2d-130">Publisher</span></span>|<span data-ttu-id="92c2d-131">String</span><span class="sxs-lookup"><span data-stu-id="92c2d-131">String</span></span>|<span data-ttu-id="92c2d-132">Издатель.</span><span class="sxs-lookup"><span data-stu-id="92c2d-132">Publisher</span></span>|
|<span data-ttu-id="92c2d-133">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="92c2d-133">publishedDateTime</span></span>|<span data-ttu-id="92c2d-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92c2d-134">DateTimeOffset</span></span>|<span data-ttu-id="92c2d-135">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-135">The date and time when the page was created.</span></span>|
|<span data-ttu-id="92c2d-136">largeCover</span><span class="sxs-lookup"><span data-stu-id="92c2d-136">largeCover</span></span>|[<span data-ttu-id="92c2d-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="92c2d-137">mimeContent</span></span>](../resources/intune_books_mimecontent.md)|<span data-ttu-id="92c2d-138">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-138">Book cover</span></span>|
|<span data-ttu-id="92c2d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="92c2d-139">createdDateTime</span></span>|<span data-ttu-id="92c2d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92c2d-140">DateTimeOffset</span></span>|<span data-ttu-id="92c2d-141">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-141">The date and time when the page was created.</span></span>|
|<span data-ttu-id="92c2d-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="92c2d-142">lastModifiedDateTime</span></span>|<span data-ttu-id="92c2d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92c2d-143">DateTimeOffset</span></span>|<span data-ttu-id="92c2d-144">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-144">The date and time when the attachment was last modified.</span></span>|
|<span data-ttu-id="92c2d-145">informationUrl</span><span class="sxs-lookup"><span data-stu-id="92c2d-145">informationUrl</span></span>|<span data-ttu-id="92c2d-146">String</span><span class="sxs-lookup"><span data-stu-id="92c2d-146">String</span></span>|<span data-ttu-id="92c2d-147">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="92c2d-147">The more information Url.</span></span>|
|<span data-ttu-id="92c2d-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="92c2d-148">privacyInformationUrl</span></span>|<span data-ttu-id="92c2d-149">String</span><span class="sxs-lookup"><span data-stu-id="92c2d-149">String</span></span>|<span data-ttu-id="92c2d-150">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="92c2d-150">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92c2d-151">Связи</span><span class="sxs-lookup"><span data-stu-id="92c2d-151">Relationships</span></span>
|<span data-ttu-id="92c2d-152">Связь</span><span class="sxs-lookup"><span data-stu-id="92c2d-152">Relationship</span></span>|<span data-ttu-id="92c2d-153">Тип</span><span class="sxs-lookup"><span data-stu-id="92c2d-153">Type</span></span>|<span data-ttu-id="92c2d-154">Описание</span><span class="sxs-lookup"><span data-stu-id="92c2d-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92c2d-155">assignments</span><span class="sxs-lookup"><span data-stu-id="92c2d-155">assignments</span></span>|<span data-ttu-id="92c2d-156">Коллекция [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="92c2d-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="92c2d-157">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-157">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="92c2d-158">installSummary</span><span class="sxs-lookup"><span data-stu-id="92c2d-158">installSummary</span></span>|[<span data-ttu-id="92c2d-159">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="92c2d-159">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="92c2d-160">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="92c2d-160">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="92c2d-161">deviceStates</span><span class="sxs-lookup"><span data-stu-id="92c2d-161">deviceStates</span></span>|<span data-ttu-id="92c2d-162">Коллекция [deviceInstallState](../resources/intune_books_deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="92c2d-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="92c2d-163">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-163">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="92c2d-164">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="92c2d-164">userStateSummary</span></span>|<span data-ttu-id="92c2d-165">Коллекция [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="92c2d-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="92c2d-166">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="92c2d-166">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92c2d-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92c2d-167">JSON Representation</span></span>
<span data-ttu-id="92c2d-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92c2d-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```



