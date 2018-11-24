# <a name="ebookinstallsummary-resource-type"></a><span data-ttu-id="19d38-101">Тип ресурса eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="19d38-101">eBookInstallSummary resource type</span></span>

> <span data-ttu-id="19d38-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19d38-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19d38-103">Содержит свойства сводки по установке книги для устройства.</span><span class="sxs-lookup"><span data-stu-id="19d38-103">Contains properties for the installation summary of a book for a device.</span></span>
## <a name="methods"></a><span data-ttu-id="19d38-104">Методы</span><span class="sxs-lookup"><span data-stu-id="19d38-104">Methods</span></span>
|<span data-ttu-id="19d38-105">Метод</span><span class="sxs-lookup"><span data-stu-id="19d38-105">Method</span></span>|<span data-ttu-id="19d38-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="19d38-106">Return Type</span></span>|<span data-ttu-id="19d38-107">Описание</span><span class="sxs-lookup"><span data-stu-id="19d38-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="19d38-108">Получение объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="19d38-108">Get eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_get.md)|[<span data-ttu-id="19d38-109">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="19d38-109">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="19d38-110">Чтение свойств и связей объекта [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="19d38-110">Read properties and relationships of the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|
|[<span data-ttu-id="19d38-111">Обновление объекта eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="19d38-111">Update eBookInstallSummary</span></span>](../api/intune_books_ebookinstallsummary_update.md)|[<span data-ttu-id="19d38-112">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="19d38-112">eBookInstallSummary</span></span>](../resources/intune_books_ebookinstallsummary.md)|<span data-ttu-id="19d38-113">Обновление свойств объекта [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="19d38-113">Update the properties of a [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="19d38-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="19d38-114">Properties</span></span>
|<span data-ttu-id="19d38-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="19d38-115">Property</span></span>|<span data-ttu-id="19d38-116">Тип</span><span class="sxs-lookup"><span data-stu-id="19d38-116">Type</span></span>|<span data-ttu-id="19d38-117">Описание</span><span class="sxs-lookup"><span data-stu-id="19d38-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19d38-118">id</span><span class="sxs-lookup"><span data-stu-id="19d38-118">id</span></span>|<span data-ttu-id="19d38-119">String</span><span class="sxs-lookup"><span data-stu-id="19d38-119">String</span></span>|<span data-ttu-id="19d38-120">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="19d38-120">Key of the entity.</span></span>|
|<span data-ttu-id="19d38-121">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19d38-121">installedDeviceCount</span></span>|<span data-ttu-id="19d38-122">Int32</span><span class="sxs-lookup"><span data-stu-id="19d38-122">Int32</span></span>|<span data-ttu-id="19d38-123">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="19d38-123">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="19d38-124">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19d38-124">failedDeviceCount</span></span>|<span data-ttu-id="19d38-125">Int32</span><span class="sxs-lookup"><span data-stu-id="19d38-125">Int32</span></span>|<span data-ttu-id="19d38-126">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="19d38-126">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="19d38-127">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="19d38-127">notInstalledDeviceCount</span></span>|<span data-ttu-id="19d38-128">Int32</span><span class="sxs-lookup"><span data-stu-id="19d38-128">Int32</span></span>|<span data-ttu-id="19d38-129">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="19d38-129">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="19d38-130">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="19d38-130">installedUserCount</span></span>|<span data-ttu-id="19d38-131">Int32</span><span class="sxs-lookup"><span data-stu-id="19d38-131">Int32</span></span>|<span data-ttu-id="19d38-132">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="19d38-132">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="19d38-133">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="19d38-133">failedUserCount</span></span>|<span data-ttu-id="19d38-134">Int32</span><span class="sxs-lookup"><span data-stu-id="19d38-134">Int32</span></span>|<span data-ttu-id="19d38-135">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="19d38-135">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="19d38-136">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="19d38-136">notInstalledUserCount</span></span>|<span data-ttu-id="19d38-137">Int32</span><span class="sxs-lookup"><span data-stu-id="19d38-137">Int32</span></span>|<span data-ttu-id="19d38-138">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="19d38-138">Number of Users that did not install this book.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19d38-139">Связи</span><span class="sxs-lookup"><span data-stu-id="19d38-139">Relationships</span></span>
<span data-ttu-id="19d38-140">Нет</span><span class="sxs-lookup"><span data-stu-id="19d38-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19d38-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19d38-141">JSON Representation</span></span>
<span data-ttu-id="19d38-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19d38-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eBookInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notInstalledUserCount": 1024
}
```



