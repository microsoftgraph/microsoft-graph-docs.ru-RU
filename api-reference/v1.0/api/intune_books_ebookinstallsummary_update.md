# <a name="update-ebookinstallsummary"></a><span data-ttu-id="530c9-101">Обновление eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="530c9-101">Update eBookInstallSummary</span></span>

> <span data-ttu-id="530c9-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="530c9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="530c9-103">Обновление свойств объекта [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="530c9-103">Update the properties of a [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="530c9-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="530c9-104">Prerequisites</span></span>
<span data-ttu-id="530c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="530c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="530c9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="530c9-107">Permission type</span></span>|<span data-ttu-id="530c9-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="530c9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="530c9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="530c9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="530c9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="530c9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="530c9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="530c9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="530c9-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="530c9-112">Not supported.</span></span>|
|<span data-ttu-id="530c9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="530c9-113">Application</span></span>|<span data-ttu-id="530c9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="530c9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="530c9-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="530c9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="530c9-116">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="530c9-116">Request headers</span></span>
|<span data-ttu-id="530c9-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="530c9-117">Header</span></span>|<span data-ttu-id="530c9-118">Значение</span><span class="sxs-lookup"><span data-stu-id="530c9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="530c9-119">Авторизация</span><span class="sxs-lookup"><span data-stu-id="530c9-119">Authorization</span></span>|<span data-ttu-id="530c9-120">Требуется Bearer &lt;маркер&gt;</span><span class="sxs-lookup"><span data-stu-id="530c9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="530c9-121">Принять</span><span class="sxs-lookup"><span data-stu-id="530c9-121">Accept</span></span>|<span data-ttu-id="530c9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="530c9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="530c9-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="530c9-123">Request body</span></span>
<span data-ttu-id="530c9-124">В теле запроса добавьте представление объекта [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="530c9-124">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="530c9-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="530c9-125">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span></span>

|<span data-ttu-id="530c9-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="530c9-126">Property</span></span>|<span data-ttu-id="530c9-127">Тип</span><span class="sxs-lookup"><span data-stu-id="530c9-127">Type</span></span>|<span data-ttu-id="530c9-128">Описание</span><span class="sxs-lookup"><span data-stu-id="530c9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="530c9-129">ид</span><span class="sxs-lookup"><span data-stu-id="530c9-129">id</span></span>|<span data-ttu-id="530c9-130">Строка</span><span class="sxs-lookup"><span data-stu-id="530c9-130">String</span></span>|<span data-ttu-id="530c9-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="530c9-131">Key of the entity.</span></span>|
|<span data-ttu-id="530c9-132">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="530c9-132">installedDeviceCount</span></span>|<span data-ttu-id="530c9-133">Int32</span><span class="sxs-lookup"><span data-stu-id="530c9-133">Int32</span></span>|<span data-ttu-id="530c9-134">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="530c9-134">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="530c9-135">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="530c9-135">failedDeviceCount</span></span>|<span data-ttu-id="530c9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="530c9-136">Int32</span></span>|<span data-ttu-id="530c9-137">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="530c9-137">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="530c9-138">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="530c9-138">notInstalledDeviceCount</span></span>|<span data-ttu-id="530c9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="530c9-139">Int32</span></span>|<span data-ttu-id="530c9-140">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="530c9-140">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="530c9-141">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="530c9-141">installedUserCount</span></span>|<span data-ttu-id="530c9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="530c9-142">Int32</span></span>|<span data-ttu-id="530c9-143">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="530c9-143">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="530c9-144">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="530c9-144">failedUserCount</span></span>|<span data-ttu-id="530c9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="530c9-145">Int32</span></span>|<span data-ttu-id="530c9-146">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="530c9-146">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="530c9-147">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="530c9-147">notInstalledUserCount</span></span>|<span data-ttu-id="530c9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="530c9-148">Int32</span></span>|<span data-ttu-id="530c9-149">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="530c9-149">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="530c9-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="530c9-150">Response</span></span>
<span data-ttu-id="530c9-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="530c9-151">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="530c9-152">Пример</span><span class="sxs-lookup"><span data-stu-id="530c9-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="530c9-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="530c9-153">Request</span></span>
<span data-ttu-id="530c9-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="530c9-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="530c9-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="530c9-155">Response</span></span>
<span data-ttu-id="530c9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="530c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```








