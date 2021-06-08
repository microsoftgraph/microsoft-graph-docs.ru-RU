---
title: Создание объекта mobileAppContentFile
description: Создание объекта mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1b525eefdf6349217aaa05a94f2d21849b59a89
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759688"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="edef1-103">Создание объекта mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="edef1-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="edef1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edef1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="edef1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="edef1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="edef1-106">Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="edef1-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="edef1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="edef1-107">Prerequisites</span></span>
<span data-ttu-id="edef1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edef1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edef1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edef1-110">Permission type</span></span>|<span data-ttu-id="edef1-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="edef1-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edef1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edef1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="edef1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edef1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="edef1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edef1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edef1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edef1-115">Not supported.</span></span>|
|<span data-ttu-id="edef1-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="edef1-116">Application</span></span>|<span data-ttu-id="edef1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edef1-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="edef1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edef1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="edef1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="edef1-119">Request headers</span></span>
|<span data-ttu-id="edef1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="edef1-120">Header</span></span>|<span data-ttu-id="edef1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="edef1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edef1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="edef1-122">Authorization</span></span>|<span data-ttu-id="edef1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="edef1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edef1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="edef1-124">Accept</span></span>|<span data-ttu-id="edef1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="edef1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edef1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edef1-126">Request body</span></span>
<span data-ttu-id="edef1-127">В тексте запроса добавьте представление объекта mobileAppContentFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="edef1-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="edef1-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="edef1-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="edef1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="edef1-129">Property</span></span>|<span data-ttu-id="edef1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="edef1-130">Type</span></span>|<span data-ttu-id="edef1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="edef1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edef1-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="edef1-132">azureStorageUri</span></span>|<span data-ttu-id="edef1-133">String</span><span class="sxs-lookup"><span data-stu-id="edef1-133">String</span></span>|<span data-ttu-id="edef1-134">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="edef1-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="edef1-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="edef1-135">isCommitted</span></span>|<span data-ttu-id="edef1-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="edef1-136">Boolean</span></span>|<span data-ttu-id="edef1-137">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="edef1-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="edef1-138">id</span><span class="sxs-lookup"><span data-stu-id="edef1-138">id</span></span>|<span data-ttu-id="edef1-139">String</span><span class="sxs-lookup"><span data-stu-id="edef1-139">String</span></span>|<span data-ttu-id="edef1-140">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="edef1-140">The File Id.</span></span>|
|<span data-ttu-id="edef1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="edef1-141">createdDateTime</span></span>|<span data-ttu-id="edef1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edef1-142">DateTimeOffset</span></span>|<span data-ttu-id="edef1-143">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="edef1-143">The time the file was created.</span></span>|
|<span data-ttu-id="edef1-144">name</span><span class="sxs-lookup"><span data-stu-id="edef1-144">name</span></span>|<span data-ttu-id="edef1-145">String</span><span class="sxs-lookup"><span data-stu-id="edef1-145">String</span></span>|<span data-ttu-id="edef1-146">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="edef1-146">the file name.</span></span>|
|<span data-ttu-id="edef1-147">size</span><span class="sxs-lookup"><span data-stu-id="edef1-147">size</span></span>|<span data-ttu-id="edef1-148">Int64</span><span class="sxs-lookup"><span data-stu-id="edef1-148">Int64</span></span>|<span data-ttu-id="edef1-149">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="edef1-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="edef1-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="edef1-150">sizeEncrypted</span></span>|<span data-ttu-id="edef1-151">Int64</span><span class="sxs-lookup"><span data-stu-id="edef1-151">Int64</span></span>|<span data-ttu-id="edef1-152">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="edef1-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="edef1-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="edef1-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="edef1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="edef1-154">DateTimeOffset</span></span>|<span data-ttu-id="edef1-155">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="edef1-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="edef1-156">manifest</span><span class="sxs-lookup"><span data-stu-id="edef1-156">manifest</span></span>|<span data-ttu-id="edef1-157">Binary</span><span class="sxs-lookup"><span data-stu-id="edef1-157">Binary</span></span>|<span data-ttu-id="edef1-158">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="edef1-158">The manifest information.</span></span>|
|<span data-ttu-id="edef1-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="edef1-159">uploadState</span></span>|[<span data-ttu-id="edef1-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="edef1-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="edef1-161">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="edef1-161">The state of the current upload request.</span></span> <span data-ttu-id="edef1-162">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="edef1-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="edef1-163">Отклик</span><span class="sxs-lookup"><span data-stu-id="edef1-163">Response</span></span>
<span data-ttu-id="edef1-164">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="edef1-164">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="edef1-165">Пример</span><span class="sxs-lookup"><span data-stu-id="edef1-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="edef1-166">Запрос</span><span class="sxs-lookup"><span data-stu-id="edef1-166">Request</span></span>
<span data-ttu-id="edef1-167">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edef1-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
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

### <a name="response"></a><span data-ttu-id="edef1-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="edef1-168">Response</span></span>
<span data-ttu-id="edef1-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="edef1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




