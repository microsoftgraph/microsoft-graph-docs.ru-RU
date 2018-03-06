# <a name="update-mobileappcontentfile"></a><span data-ttu-id="38025-101">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="38025-101">Update mobileAppContentFile</span></span>

> <span data-ttu-id="38025-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="38025-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38025-103">Обновление свойств объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="38025-103">Update the properties of a [calendar](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="38025-104">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="38025-104">Prerequisites</span></span>
<span data-ttu-id="38025-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="38025-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="38025-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="38025-107">Permission type</span></span>|<span data-ttu-id="38025-108">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="38025-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38025-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="38025-109">Delegated (work or school account)</span></span>|<span data-ttu-id="38025-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38025-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38025-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="38025-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38025-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38025-112">Not supported.</span></span>|
|<span data-ttu-id="38025-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="38025-113">Application</span></span>|<span data-ttu-id="38025-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38025-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38025-115">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="38025-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="38025-116">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="38025-116">Request headers</span></span>
|<span data-ttu-id="38025-117">Заголовок</span><span class="sxs-lookup"><span data-stu-id="38025-117">Header</span></span>|<span data-ttu-id="38025-118">Значение</span><span class="sxs-lookup"><span data-stu-id="38025-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38025-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="38025-119">Authorization</span></span>|<span data-ttu-id="38025-120">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="38025-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="38025-121">Accept</span><span class="sxs-lookup"><span data-stu-id="38025-121">Accept</span></span>|<span data-ttu-id="38025-122">application/json</span><span class="sxs-lookup"><span data-stu-id="38025-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38025-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="38025-123">Request body</span></span>
<span data-ttu-id="38025-124">В теле запроса добавьте представление объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38025-124">In the request body, supply a JSON representation of [domain](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="38025-125">Ниже показаны свойства, которые необходимо указывать при создании объекта [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="38025-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="38025-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="38025-126">Property</span></span>|<span data-ttu-id="38025-127">Тип</span><span class="sxs-lookup"><span data-stu-id="38025-127">Type</span></span>|<span data-ttu-id="38025-128">Описание</span><span class="sxs-lookup"><span data-stu-id="38025-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38025-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="38025-129">azureStorageUri</span></span>|<span data-ttu-id="38025-130">String</span><span class="sxs-lookup"><span data-stu-id="38025-130">String</span></span>|<span data-ttu-id="38025-131">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="38025-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="38025-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="38025-132">isCommitted</span></span>|<span data-ttu-id="38025-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="38025-133">Boolean</span></span>|<span data-ttu-id="38025-134">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="38025-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="38025-135">id</span><span class="sxs-lookup"><span data-stu-id="38025-135">id</span></span>|<span data-ttu-id="38025-136">String</span><span class="sxs-lookup"><span data-stu-id="38025-136">String</span></span>|<span data-ttu-id="38025-137">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="38025-137">The File Id.</span></span>|
|<span data-ttu-id="38025-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38025-138">createdDateTime</span></span>|<span data-ttu-id="38025-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38025-139">DateTimeOffset</span></span>|<span data-ttu-id="38025-140">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="38025-140">The time the file was created.</span></span>|
|<span data-ttu-id="38025-141">name</span><span class="sxs-lookup"><span data-stu-id="38025-141">name</span></span>|<span data-ttu-id="38025-142">String</span><span class="sxs-lookup"><span data-stu-id="38025-142">String</span></span>|<span data-ttu-id="38025-143">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="38025-143">The file name.</span></span>|
|<span data-ttu-id="38025-144">size</span><span class="sxs-lookup"><span data-stu-id="38025-144">size</span></span>|<span data-ttu-id="38025-145">Int64</span><span class="sxs-lookup"><span data-stu-id="38025-145">Int64</span></span>|<span data-ttu-id="38025-146">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="38025-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="38025-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="38025-147">sizeEncrypted</span></span>|<span data-ttu-id="38025-148">Int64</span><span class="sxs-lookup"><span data-stu-id="38025-148">Int64</span></span>|<span data-ttu-id="38025-149">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="38025-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="38025-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="38025-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="38025-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38025-151">DateTimeOffset</span></span>|<span data-ttu-id="38025-152">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="38025-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="38025-153">manifest</span><span class="sxs-lookup"><span data-stu-id="38025-153">manifest</span></span>|<span data-ttu-id="38025-154">Binary</span><span class="sxs-lookup"><span data-stu-id="38025-154">Binary</span></span>|<span data-ttu-id="38025-155">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="38025-155">The manifest information.</span></span>|
|<span data-ttu-id="38025-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="38025-156">uploadState</span></span>|<span data-ttu-id="38025-157">String</span><span class="sxs-lookup"><span data-stu-id="38025-157">String</span></span>|<span data-ttu-id="38025-158">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="38025-158">The state of the current upload request.</span></span> <span data-ttu-id="38025-159">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="38025-159">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="38025-160">Ответ</span><span class="sxs-lookup"><span data-stu-id="38025-160">Response</span></span>
<span data-ttu-id="38025-161">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="38025-161">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38025-162">Пример</span><span class="sxs-lookup"><span data-stu-id="38025-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="38025-163">Запрос</span><span class="sxs-lookup"><span data-stu-id="38025-163">Request</span></span>
<span data-ttu-id="38025-164">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="38025-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 283

{
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

### <a name="response"></a><span data-ttu-id="38025-165">Ответ</span><span class="sxs-lookup"><span data-stu-id="38025-165">Response</span></span>
<span data-ttu-id="38025-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="38025-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



