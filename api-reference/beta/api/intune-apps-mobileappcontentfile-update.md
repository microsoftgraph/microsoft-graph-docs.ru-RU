---
title: Update mobileAppContentFile
description: Обновление свойств объекта mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0fe430fb9d646a47ecc53acac46441d9cf7b1cf6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977315"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="8b9cc-103">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="8b9cc-103">Update mobileAppContentFile</span></span>

<span data-ttu-id="8b9cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b9cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b9cc-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b9cc-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b9cc-107">Обновление свойств объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="8b9cc-107">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b9cc-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="8b9cc-108">Prerequisites</span></span>
<span data-ttu-id="8b9cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b9cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b9cc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b9cc-111">Permission type</span></span>|<span data-ttu-id="8b9cc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b9cc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b9cc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b9cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8b9cc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9cc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8b9cc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b9cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b9cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-116">Not supported.</span></span>|
|<span data-ttu-id="8b9cc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b9cc-117">Application</span></span>|<span data-ttu-id="8b9cc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b9cc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b9cc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b9cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="8b9cc-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8b9cc-120">Request headers</span></span>
|<span data-ttu-id="8b9cc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b9cc-121">Header</span></span>|<span data-ttu-id="8b9cc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8b9cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b9cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b9cc-123">Authorization</span></span>|<span data-ttu-id="8b9cc-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b9cc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8b9cc-125">Accept</span></span>|<span data-ttu-id="8b9cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8b9cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b9cc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b9cc-127">Request body</span></span>
<span data-ttu-id="8b9cc-128">В теле запроса добавьте представление объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-128">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="8b9cc-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="8b9cc-129">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="8b9cc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b9cc-130">Property</span></span>|<span data-ttu-id="8b9cc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8b9cc-131">Type</span></span>|<span data-ttu-id="8b9cc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8b9cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b9cc-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="8b9cc-133">azureStorageUri</span></span>|<span data-ttu-id="8b9cc-134">String</span><span class="sxs-lookup"><span data-stu-id="8b9cc-134">String</span></span>|<span data-ttu-id="8b9cc-135">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="8b9cc-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="8b9cc-136">isCommitted</span></span>|<span data-ttu-id="8b9cc-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b9cc-137">Boolean</span></span>|<span data-ttu-id="8b9cc-138">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="8b9cc-139">id</span><span class="sxs-lookup"><span data-stu-id="8b9cc-139">id</span></span>|<span data-ttu-id="8b9cc-140">String</span><span class="sxs-lookup"><span data-stu-id="8b9cc-140">String</span></span>|<span data-ttu-id="8b9cc-141">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-141">The File Id.</span></span>|
|<span data-ttu-id="8b9cc-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b9cc-142">createdDateTime</span></span>|<span data-ttu-id="8b9cc-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b9cc-143">DateTimeOffset</span></span>|<span data-ttu-id="8b9cc-144">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-144">The time the file was created.</span></span>|
|<span data-ttu-id="8b9cc-145">name</span><span class="sxs-lookup"><span data-stu-id="8b9cc-145">name</span></span>|<span data-ttu-id="8b9cc-146">String</span><span class="sxs-lookup"><span data-stu-id="8b9cc-146">String</span></span>|<span data-ttu-id="8b9cc-147">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-147">the file name.</span></span>|
|<span data-ttu-id="8b9cc-148">size</span><span class="sxs-lookup"><span data-stu-id="8b9cc-148">size</span></span>|<span data-ttu-id="8b9cc-149">Int64</span><span class="sxs-lookup"><span data-stu-id="8b9cc-149">Int64</span></span>|<span data-ttu-id="8b9cc-150">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="8b9cc-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="8b9cc-151">sizeEncrypted</span></span>|<span data-ttu-id="8b9cc-152">Int64</span><span class="sxs-lookup"><span data-stu-id="8b9cc-152">Int64</span></span>|<span data-ttu-id="8b9cc-153">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="8b9cc-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8b9cc-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="8b9cc-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b9cc-155">DateTimeOffset</span></span>|<span data-ttu-id="8b9cc-156">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="8b9cc-157">manifest</span><span class="sxs-lookup"><span data-stu-id="8b9cc-157">manifest</span></span>|<span data-ttu-id="8b9cc-158">Binary</span><span class="sxs-lookup"><span data-stu-id="8b9cc-158">Binary</span></span>|<span data-ttu-id="8b9cc-159">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-159">The manifest information.</span></span>|
|<span data-ttu-id="8b9cc-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="8b9cc-160">uploadState</span></span>|[<span data-ttu-id="8b9cc-161">мобилеаппконтентфилеуплоадстате</span><span class="sxs-lookup"><span data-stu-id="8b9cc-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="8b9cc-162">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-162">The state of the current upload request.</span></span> <span data-ttu-id="8b9cc-163">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="8b9cc-164">исфрамеворкфиле</span><span class="sxs-lookup"><span data-stu-id="8b9cc-164">isFrameworkFile</span></span>|<span data-ttu-id="8b9cc-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b9cc-165">Boolean</span></span>|<span data-ttu-id="8b9cc-166">Значение, указывающее, является ли файл файлом платформы.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="8b9cc-167">Dependency</span><span class="sxs-lookup"><span data-stu-id="8b9cc-167">isDependency</span></span>|<span data-ttu-id="8b9cc-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b9cc-168">Boolean</span></span>|<span data-ttu-id="8b9cc-169">Является ли файл содержимого зависимостью от основного файла содержимого.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="8b9cc-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="8b9cc-170">Response</span></span>
<span data-ttu-id="8b9cc-171">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-171">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b9cc-172">Пример</span><span class="sxs-lookup"><span data-stu-id="8b9cc-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b9cc-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b9cc-173">Request</span></span>
<span data-ttu-id="8b9cc-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```

### <a name="response"></a><span data-ttu-id="8b9cc-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b9cc-175">Response</span></span>
<span data-ttu-id="8b9cc-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b9cc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 503

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
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```






