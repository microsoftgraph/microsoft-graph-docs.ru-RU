# <a name="managedebook-resource-type"></a><span data-ttu-id="90e4e-101">Тип ресурса managedEBook</span><span class="sxs-lookup"><span data-stu-id="90e4e-101">managedEBook resource type</span></span>

> <span data-ttu-id="90e4e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="90e4e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="90e4e-103">Абстрактный класс, содержащий базовые свойства управляемой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-103">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="90e4e-104">Методы</span><span class="sxs-lookup"><span data-stu-id="90e4e-104">Methods</span></span>
|<span data-ttu-id="90e4e-105">Метод</span><span class="sxs-lookup"><span data-stu-id="90e4e-105">Method</span></span>|<span data-ttu-id="90e4e-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90e4e-106">Return Type</span></span>|<span data-ttu-id="90e4e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="90e4e-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="90e4e-108">Список managedEBooks</span><span class="sxs-lookup"><span data-stu-id="90e4e-108">List managedEBooks</span></span>](../api/intune_books_managedebook_list.md)|<span data-ttu-id="90e4e-109">Коллекция [managedEBook](../resources/intune_books_managedebook.md)</span><span class="sxs-lookup"><span data-stu-id="90e4e-109">[managedEBook](../resources/intune_books_managedebook.md) collection</span></span>|<span data-ttu-id="90e4e-110">Список свойств и связей объектов [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="90e4e-110">List properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) objects.</span></span>|
|[<span data-ttu-id="90e4e-111">Получение объекта managedEBook</span><span class="sxs-lookup"><span data-stu-id="90e4e-111">Get managedEBook</span></span>](../api/intune_books_managedebook_get.md)|[<span data-ttu-id="90e4e-112">managedEBook</span><span class="sxs-lookup"><span data-stu-id="90e4e-112">managedEBook</span></span>](../resources/intune_books_managedebook.md)|<span data-ttu-id="90e4e-113">Чтение свойств и связей объекта [managedEBook](../resources/intune_books_managedebook.md).</span><span class="sxs-lookup"><span data-stu-id="90e4e-113">Read properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) object.</span></span>|
|[<span data-ttu-id="90e4e-114">действие назначения</span><span class="sxs-lookup"><span data-stu-id="90e4e-114">assign action</span></span>](../api/intune_books_managedebook_assign.md)|<span data-ttu-id="90e4e-115">Нет</span><span class="sxs-lookup"><span data-stu-id="90e4e-115">None</span></span>|<span data-ttu-id="90e4e-116">Н/Д</span><span class="sxs-lookup"><span data-stu-id="90e4e-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="90e4e-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="90e4e-117">Properties</span></span>
|<span data-ttu-id="90e4e-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="90e4e-118">Property</span></span>|<span data-ttu-id="90e4e-119">Тип</span><span class="sxs-lookup"><span data-stu-id="90e4e-119">Type</span></span>|<span data-ttu-id="90e4e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="90e4e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90e4e-121">id</span><span class="sxs-lookup"><span data-stu-id="90e4e-121">id</span></span>|<span data-ttu-id="90e4e-122">String</span><span class="sxs-lookup"><span data-stu-id="90e4e-122">String</span></span>|<span data-ttu-id="90e4e-123">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="90e4e-123">Key of the entity.</span></span>|
|<span data-ttu-id="90e4e-124">displayName</span><span class="sxs-lookup"><span data-stu-id="90e4e-124">displayName</span></span>|<span data-ttu-id="90e4e-125">String</span><span class="sxs-lookup"><span data-stu-id="90e4e-125">String</span></span>|<span data-ttu-id="90e4e-126">Имя электронной книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-126">Name of the eBook.</span></span>|
|<span data-ttu-id="90e4e-127">description</span><span class="sxs-lookup"><span data-stu-id="90e4e-127">description</span></span>|<span data-ttu-id="90e4e-128">String</span><span class="sxs-lookup"><span data-stu-id="90e4e-128">String</span></span>|<span data-ttu-id="90e4e-129">Описание.</span><span class="sxs-lookup"><span data-stu-id="90e4e-129">Description.</span></span>|
|<span data-ttu-id="90e4e-130">publisher</span><span class="sxs-lookup"><span data-stu-id="90e4e-130">publisher</span></span>|<span data-ttu-id="90e4e-131">String</span><span class="sxs-lookup"><span data-stu-id="90e4e-131">String</span></span>|<span data-ttu-id="90e4e-132">Издатель.</span><span class="sxs-lookup"><span data-stu-id="90e4e-132">Publisher.</span></span>|
|<span data-ttu-id="90e4e-133">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="90e4e-133">publishedDateTime</span></span>|<span data-ttu-id="90e4e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90e4e-134">DateTimeOffset</span></span>|<span data-ttu-id="90e4e-135">Дата и время публикации электронной книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-135">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="90e4e-136">largeCover</span><span class="sxs-lookup"><span data-stu-id="90e4e-136">largeCover</span></span>|[<span data-ttu-id="90e4e-137">mimeContent</span><span class="sxs-lookup"><span data-stu-id="90e4e-137">mimeContent</span></span>](../resources/intune_shared_mimecontent.md)|<span data-ttu-id="90e4e-138">Обложка книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-138">Book cover.</span></span>|
|<span data-ttu-id="90e4e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="90e4e-139">createdDateTime</span></span>|<span data-ttu-id="90e4e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90e4e-140">DateTimeOffset</span></span>|<span data-ttu-id="90e4e-141">Дата и время создания электронной книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-141">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="90e4e-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="90e4e-142">lastModifiedDateTime</span></span>|<span data-ttu-id="90e4e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90e4e-143">DateTimeOffset</span></span>|<span data-ttu-id="90e4e-144">Дата и время последнего изменения электронной книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-144">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="90e4e-145">informationUrl</span><span class="sxs-lookup"><span data-stu-id="90e4e-145">informationUrl</span></span>|<span data-ttu-id="90e4e-146">String</span><span class="sxs-lookup"><span data-stu-id="90e4e-146">String</span></span>|<span data-ttu-id="90e4e-147">URL-адрес с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="90e4e-147">The more information Url.</span></span>|
|<span data-ttu-id="90e4e-148">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="90e4e-148">privacyInformationUrl</span></span>|<span data-ttu-id="90e4e-149">String</span><span class="sxs-lookup"><span data-stu-id="90e4e-149">String</span></span>|<span data-ttu-id="90e4e-150">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="90e4e-150">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="90e4e-151">Связи</span><span class="sxs-lookup"><span data-stu-id="90e4e-151">Relationships</span></span>
|<span data-ttu-id="90e4e-152">Связь</span><span class="sxs-lookup"><span data-stu-id="90e4e-152">Relationship</span></span>|<span data-ttu-id="90e4e-153">Тип</span><span class="sxs-lookup"><span data-stu-id="90e4e-153">Type</span></span>|<span data-ttu-id="90e4e-154">Описание</span><span class="sxs-lookup"><span data-stu-id="90e4e-154">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90e4e-155">assignments</span><span class="sxs-lookup"><span data-stu-id="90e4e-155">assignments</span></span>|<span data-ttu-id="90e4e-156">Коллекция [managedEBookAssignment](../resources/intune_books_managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="90e4e-156">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="90e4e-157">Список назначений для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-157">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="90e4e-158">installSummary</span><span class="sxs-lookup"><span data-stu-id="90e4e-158">installSummary</span></span>|[<span data-ttu-id="90e4e-159">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="90e4e-159">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="90e4e-160">Общие сведения по установке мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="90e4e-160">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="90e4e-161">deviceStates</span><span class="sxs-lookup"><span data-stu-id="90e4e-161">deviceStates</span></span>|<span data-ttu-id="90e4e-162">Коллекция [deviceInstallState](../resources/intune_books_deviceinstallstate.md)</span><span class="sxs-lookup"><span data-stu-id="90e4e-162">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) collection</span></span>|<span data-ttu-id="90e4e-163">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-163">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="90e4e-164">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="90e4e-164">userStateSummary</span></span>|<span data-ttu-id="90e4e-165">Коллекция [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md)</span><span class="sxs-lookup"><span data-stu-id="90e4e-165">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="90e4e-166">Список состояний установки для этой электронной книги.</span><span class="sxs-lookup"><span data-stu-id="90e4e-166">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90e4e-167">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90e4e-167">JSON Representation</span></span>
<span data-ttu-id="90e4e-168">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90e4e-168">Here is a JSON representation of the resource.</span></span>
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



