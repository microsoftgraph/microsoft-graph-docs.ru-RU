---
title: Update mobileAppContentFile
description: Обновление свойств объекта mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9800ef98c33051f7c2faf173bc7f61ebb75849c0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355003"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="3e7d9-103">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="3e7d9-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="3e7d9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e7d9-105">Обновление свойств объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="3e7d9-105">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e7d9-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7d9-106">Prerequisites</span></span>
<span data-ttu-id="3e7d9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e7d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e7d9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7d9-109">Permission type</span></span>|<span data-ttu-id="3e7d9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e7d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e7d9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e7d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3e7d9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e7d9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3e7d9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e7d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e7d9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-114">Not supported.</span></span>|
|<span data-ttu-id="3e7d9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e7d9-115">Application</span></span>|<span data-ttu-id="3e7d9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e7d9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e7d9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="3e7d9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e7d9-118">Request headers</span></span>
|<span data-ttu-id="3e7d9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e7d9-119">Header</span></span>|<span data-ttu-id="3e7d9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3e7d9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e7d9-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3e7d9-121">Authorization</span></span>|<span data-ttu-id="3e7d9-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e7d9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3e7d9-123">Accept</span></span>|<span data-ttu-id="3e7d9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3e7d9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e7d9-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3e7d9-125">Request body</span></span>
<span data-ttu-id="3e7d9-126">В теле запроса добавьте представление объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-126">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="3e7d9-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="3e7d9-127">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="3e7d9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e7d9-128">Property</span></span>|<span data-ttu-id="3e7d9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3e7d9-129">Type</span></span>|<span data-ttu-id="3e7d9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3e7d9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e7d9-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="3e7d9-131">azureStorageUri</span></span>|<span data-ttu-id="3e7d9-132">String</span><span class="sxs-lookup"><span data-stu-id="3e7d9-132">String</span></span>|<span data-ttu-id="3e7d9-133">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="3e7d9-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="3e7d9-134">isCommitted</span></span>|<span data-ttu-id="3e7d9-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e7d9-135">Boolean</span></span>|<span data-ttu-id="3e7d9-136">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="3e7d9-137">id</span><span class="sxs-lookup"><span data-stu-id="3e7d9-137">id</span></span>|<span data-ttu-id="3e7d9-138">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7d9-138">String</span></span>|<span data-ttu-id="3e7d9-139">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-139">The File Id.</span></span>|
|<span data-ttu-id="3e7d9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e7d9-140">createdDateTime</span></span>|<span data-ttu-id="3e7d9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e7d9-141">DateTimeOffset</span></span>|<span data-ttu-id="3e7d9-142">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-142">The time the file was created.</span></span>|
|<span data-ttu-id="3e7d9-143">name</span><span class="sxs-lookup"><span data-stu-id="3e7d9-143">name</span></span>|<span data-ttu-id="3e7d9-144">String</span><span class="sxs-lookup"><span data-stu-id="3e7d9-144">String</span></span>|<span data-ttu-id="3e7d9-145">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-145">the file name.</span></span>|
|<span data-ttu-id="3e7d9-146">size</span><span class="sxs-lookup"><span data-stu-id="3e7d9-146">size</span></span>|<span data-ttu-id="3e7d9-147">Int64</span><span class="sxs-lookup"><span data-stu-id="3e7d9-147">Int64</span></span>|<span data-ttu-id="3e7d9-148">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="3e7d9-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="3e7d9-149">sizeEncrypted</span></span>|<span data-ttu-id="3e7d9-150">Int64</span><span class="sxs-lookup"><span data-stu-id="3e7d9-150">Int64</span></span>|<span data-ttu-id="3e7d9-151">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="3e7d9-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3e7d9-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="3e7d9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e7d9-153">DateTimeOffset</span></span>|<span data-ttu-id="3e7d9-154">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="3e7d9-155">manifest</span><span class="sxs-lookup"><span data-stu-id="3e7d9-155">manifest</span></span>|<span data-ttu-id="3e7d9-156">Binary</span><span class="sxs-lookup"><span data-stu-id="3e7d9-156">Binary</span></span>|<span data-ttu-id="3e7d9-157">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-157">The manifest information.</span></span>|
|<span data-ttu-id="3e7d9-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="3e7d9-158">uploadState</span></span>|[<span data-ttu-id="3e7d9-159">мобилеаппконтентфилеуплоадстате</span><span class="sxs-lookup"><span data-stu-id="3e7d9-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="3e7d9-160">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-160">The state of the current upload request.</span></span> <span data-ttu-id="3e7d9-161">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="3e7d9-162">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e7d9-162">Response</span></span>
<span data-ttu-id="3e7d9-163">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-163">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e7d9-164">Пример</span><span class="sxs-lookup"><span data-stu-id="3e7d9-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e7d9-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e7d9-165">Request</span></span>
<span data-ttu-id="3e7d9-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3e7d9-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="3e7d9-167">Response</span></span>
<span data-ttu-id="3e7d9-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3e7d9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




