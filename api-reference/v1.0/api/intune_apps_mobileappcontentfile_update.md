# <a name="update-mobileappcontentfile"></a><span data-ttu-id="f7855-101">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="f7855-101">Update mobileAppContentFile</span></span>

> <span data-ttu-id="f7855-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f7855-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7855-103">Обновление свойств объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="f7855-103">Update the properties of a [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7855-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f7855-104">Prerequisites</span></span>
<span data-ttu-id="f7855-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f7855-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7855-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f7855-107">Permission type</span></span>|<span data-ttu-id="f7855-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f7855-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7855-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f7855-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f7855-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7855-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f7855-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f7855-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7855-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7855-112">Not supported.</span></span>|
|<span data-ttu-id="f7855-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f7855-113">Application</span></span>|<span data-ttu-id="f7855-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f7855-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7855-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f7855-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="f7855-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f7855-116">Request headers</span></span>
|<span data-ttu-id="f7855-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f7855-117">Header</span></span>|<span data-ttu-id="f7855-118">Значение</span><span class="sxs-lookup"><span data-stu-id="f7855-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7855-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7855-119">Authorization</span></span>|<span data-ttu-id="f7855-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f7855-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7855-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f7855-121">Accept</span></span>|<span data-ttu-id="f7855-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f7855-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7855-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f7855-123">Request body</span></span>
<span data-ttu-id="f7855-124">В теле запроса добавьте представление объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7855-124">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="f7855-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="f7855-125">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span></span>

|<span data-ttu-id="f7855-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7855-126">Property</span></span>|<span data-ttu-id="f7855-127">Тип</span><span class="sxs-lookup"><span data-stu-id="f7855-127">Type</span></span>|<span data-ttu-id="f7855-128">Описание</span><span class="sxs-lookup"><span data-stu-id="f7855-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7855-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="f7855-129">azureStorageUri</span></span>|<span data-ttu-id="f7855-130">String</span><span class="sxs-lookup"><span data-stu-id="f7855-130">String</span></span>|<span data-ttu-id="f7855-131">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="f7855-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="f7855-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="f7855-132">isCommitted</span></span>|<span data-ttu-id="f7855-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7855-133">Boolean</span></span>|<span data-ttu-id="f7855-134">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="f7855-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="f7855-135">id</span><span class="sxs-lookup"><span data-stu-id="f7855-135">id</span></span>|<span data-ttu-id="f7855-136">String</span><span class="sxs-lookup"><span data-stu-id="f7855-136">String</span></span>|<span data-ttu-id="f7855-137">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="f7855-137">The File Id.</span></span>|
|<span data-ttu-id="f7855-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7855-138">createdDateTime</span></span>|<span data-ttu-id="f7855-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7855-139">DateTimeOffset</span></span>|<span data-ttu-id="f7855-140">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="f7855-140">The time the file was created.</span></span>|
|<span data-ttu-id="f7855-141">name</span><span class="sxs-lookup"><span data-stu-id="f7855-141">name</span></span>|<span data-ttu-id="f7855-142">String</span><span class="sxs-lookup"><span data-stu-id="f7855-142">String</span></span>|<span data-ttu-id="f7855-143">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="f7855-143">the file name.</span></span>|
|<span data-ttu-id="f7855-144">size</span><span class="sxs-lookup"><span data-stu-id="f7855-144">size</span></span>|<span data-ttu-id="f7855-145">Int64</span><span class="sxs-lookup"><span data-stu-id="f7855-145">Int64</span></span>|<span data-ttu-id="f7855-146">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="f7855-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="f7855-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="f7855-147">sizeEncrypted</span></span>|<span data-ttu-id="f7855-148">Int64</span><span class="sxs-lookup"><span data-stu-id="f7855-148">Int64</span></span>|<span data-ttu-id="f7855-149">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="f7855-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="f7855-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f7855-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="f7855-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7855-151">DateTimeOffset</span></span>|<span data-ttu-id="f7855-152">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="f7855-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="f7855-153">manifest</span><span class="sxs-lookup"><span data-stu-id="f7855-153">manifest</span></span>|<span data-ttu-id="f7855-154">Binary</span><span class="sxs-lookup"><span data-stu-id="f7855-154">Binary</span></span>|<span data-ttu-id="f7855-155">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="f7855-155">The manifest information.</span></span>|
|<span data-ttu-id="f7855-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="f7855-156">uploadState</span></span>|[<span data-ttu-id="f7855-157">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="f7855-157">mobileAppContentFileUploadState</span></span>](../resources/intune_apps_mobileappcontentfileuploadstate.md)|<span data-ttu-id="f7855-158">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="f7855-158">The state of the current upload request.</span></span> <span data-ttu-id="f7855-159">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="f7855-159">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="f7855-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7855-160">Response</span></span>
<span data-ttu-id="f7855-161">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f7855-161">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7855-162">Пример</span><span class="sxs-lookup"><span data-stu-id="f7855-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7855-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="f7855-163">Request</span></span>
<span data-ttu-id="f7855-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f7855-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="f7855-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="f7855-165">Response</span></span>
<span data-ttu-id="f7855-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f7855-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```



