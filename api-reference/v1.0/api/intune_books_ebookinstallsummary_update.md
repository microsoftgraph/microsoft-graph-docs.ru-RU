# <a name="update-ebookinstallsummary"></a><span data-ttu-id="2debf-101">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="2debf-101">Update eBookInstallSummary</span></span>

> <span data-ttu-id="2debf-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2debf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2debf-103">Обновление свойств объекта [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2debf-103">Update the properties of a [calendar](../resources/intune_books_ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2debf-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="2debf-104">Prerequisites</span></span>
<span data-ttu-id="2debf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2debf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2debf-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2debf-107">Permission type</span></span>|<span data-ttu-id="2debf-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="2debf-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2debf-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2debf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2debf-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2debf-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2debf-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2debf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2debf-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2debf-112">Not supported.</span></span>|
|<span data-ttu-id="2debf-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2debf-113">Application</span></span>|<span data-ttu-id="2debf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2debf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2debf-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2debf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="2debf-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="2debf-116">Request headers</span></span>
|<span data-ttu-id="2debf-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2debf-117">Header</span></span>|<span data-ttu-id="2debf-118">Значение</span><span class="sxs-lookup"><span data-stu-id="2debf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2debf-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2debf-119">Authorization</span></span>|<span data-ttu-id="2debf-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2debf-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2debf-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2debf-121">Accept</span></span>|<span data-ttu-id="2debf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2debf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2debf-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2debf-123">Request body</span></span>
<span data-ttu-id="2debf-124">В теле запроса добавьте представление объекта [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2debf-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_books_ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="2debf-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="2debf-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2debf-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="2debf-126">Property</span></span>|<span data-ttu-id="2debf-127">Тип</span><span class="sxs-lookup"><span data-stu-id="2debf-127">Type</span></span>|<span data-ttu-id="2debf-128">Описание</span><span class="sxs-lookup"><span data-stu-id="2debf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2debf-129">id</span><span class="sxs-lookup"><span data-stu-id="2debf-129">id</span></span>|<span data-ttu-id="2debf-130">String</span><span class="sxs-lookup"><span data-stu-id="2debf-130">String</span></span>|<span data-ttu-id="2debf-131">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="2debf-131">Key of the setting.</span></span>|
|<span data-ttu-id="2debf-132">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2debf-132">installedDeviceCount</span></span>|<span data-ttu-id="2debf-133">Int32</span><span class="sxs-lookup"><span data-stu-id="2debf-133">Int32</span></span>|<span data-ttu-id="2debf-134">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="2debf-134">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="2debf-135">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2debf-135">failedDeviceCount</span></span>|<span data-ttu-id="2debf-136">Int32</span><span class="sxs-lookup"><span data-stu-id="2debf-136">Int32</span></span>|<span data-ttu-id="2debf-137">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="2debf-137">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="2debf-138">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="2debf-138">notInstalledDeviceCount</span></span>|<span data-ttu-id="2debf-139">Int32</span><span class="sxs-lookup"><span data-stu-id="2debf-139">Int32</span></span>|<span data-ttu-id="2debf-140">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="2debf-140">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="2debf-141">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="2debf-141">installedUserCount</span></span>|<span data-ttu-id="2debf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2debf-142">Int32</span></span>|<span data-ttu-id="2debf-143">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="2debf-143">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="2debf-144">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="2debf-144">failedUserCount</span></span>|<span data-ttu-id="2debf-145">Int32</span><span class="sxs-lookup"><span data-stu-id="2debf-145">Int32</span></span>|<span data-ttu-id="2debf-146">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="2debf-146">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="2debf-147">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="2debf-147">notInstalledUserCount</span></span>|<span data-ttu-id="2debf-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2debf-148">Int32</span></span>|<span data-ttu-id="2debf-149">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="2debf-149">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="2debf-150">Ответ</span><span class="sxs-lookup"><span data-stu-id="2debf-150">Response</span></span>
<span data-ttu-id="2debf-151">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="2debf-151">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_books_ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2debf-152">Пример</span><span class="sxs-lookup"><span data-stu-id="2debf-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="2debf-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="2debf-153">Request</span></span>
<span data-ttu-id="2debf-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2debf-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2debf-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="2debf-155">Response</span></span>
<span data-ttu-id="2debf-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="2debf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



