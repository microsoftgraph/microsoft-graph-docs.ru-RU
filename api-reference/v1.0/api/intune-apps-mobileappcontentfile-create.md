---
title: Создание объекта mobileAppContentFile
description: Создание объекта mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9061a3b44d80d7182af321502afa84a3a8cb68fb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972637"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="7d7cf-103">Создание объекта mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="7d7cf-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="7d7cf-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d7cf-105">Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="7d7cf-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d7cf-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7d7cf-106">Prerequisites</span></span>
<span data-ttu-id="7d7cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d7cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d7cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7d7cf-109">Permission type</span></span>|<span data-ttu-id="7d7cf-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7d7cf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d7cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7d7cf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7d7cf-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d7cf-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d7cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7d7cf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d7cf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-114">Not supported.</span></span>|
|<span data-ttu-id="7d7cf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7d7cf-115">Application</span></span>|<span data-ttu-id="7d7cf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d7cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7d7cf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="7d7cf-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7d7cf-118">Request headers</span></span>
|<span data-ttu-id="7d7cf-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7d7cf-119">Header</span></span>|<span data-ttu-id="7d7cf-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7d7cf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d7cf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d7cf-121">Authorization</span></span>|<span data-ttu-id="7d7cf-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7d7cf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d7cf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7d7cf-123">Accept</span></span>|<span data-ttu-id="7d7cf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7d7cf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d7cf-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7d7cf-125">Request body</span></span>
<span data-ttu-id="7d7cf-126">В тексте запроса добавьте представление объекта mobileAppContentFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="7d7cf-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="7d7cf-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="7d7cf-128">Property</span></span>|<span data-ttu-id="7d7cf-129">Тип</span><span class="sxs-lookup"><span data-stu-id="7d7cf-129">Type</span></span>|<span data-ttu-id="7d7cf-130">Описание</span><span class="sxs-lookup"><span data-stu-id="7d7cf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d7cf-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="7d7cf-131">azureStorageUri</span></span>|<span data-ttu-id="7d7cf-132">String</span><span class="sxs-lookup"><span data-stu-id="7d7cf-132">String</span></span>|<span data-ttu-id="7d7cf-133">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="7d7cf-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="7d7cf-134">isCommitted</span></span>|<span data-ttu-id="7d7cf-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="7d7cf-135">Boolean</span></span>|<span data-ttu-id="7d7cf-136">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="7d7cf-137">id</span><span class="sxs-lookup"><span data-stu-id="7d7cf-137">id</span></span>|<span data-ttu-id="7d7cf-138">String</span><span class="sxs-lookup"><span data-stu-id="7d7cf-138">String</span></span>|<span data-ttu-id="7d7cf-139">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-139">The File Id.</span></span>|
|<span data-ttu-id="7d7cf-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7cf-140">createdDateTime</span></span>|<span data-ttu-id="7d7cf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7cf-141">DateTimeOffset</span></span>|<span data-ttu-id="7d7cf-142">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-142">The time the file was created.</span></span>|
|<span data-ttu-id="7d7cf-143">name</span><span class="sxs-lookup"><span data-stu-id="7d7cf-143">name</span></span>|<span data-ttu-id="7d7cf-144">String</span><span class="sxs-lookup"><span data-stu-id="7d7cf-144">String</span></span>|<span data-ttu-id="7d7cf-145">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-145">the file name.</span></span>|
|<span data-ttu-id="7d7cf-146">size</span><span class="sxs-lookup"><span data-stu-id="7d7cf-146">size</span></span>|<span data-ttu-id="7d7cf-147">Int64</span><span class="sxs-lookup"><span data-stu-id="7d7cf-147">Int64</span></span>|<span data-ttu-id="7d7cf-148">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="7d7cf-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="7d7cf-149">sizeEncrypted</span></span>|<span data-ttu-id="7d7cf-150">Int64</span><span class="sxs-lookup"><span data-stu-id="7d7cf-150">Int64</span></span>|<span data-ttu-id="7d7cf-151">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="7d7cf-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7d7cf-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="7d7cf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d7cf-153">DateTimeOffset</span></span>|<span data-ttu-id="7d7cf-154">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="7d7cf-155">manifest</span><span class="sxs-lookup"><span data-stu-id="7d7cf-155">manifest</span></span>|<span data-ttu-id="7d7cf-156">Binary</span><span class="sxs-lookup"><span data-stu-id="7d7cf-156">Binary</span></span>|<span data-ttu-id="7d7cf-157">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-157">The manifest information.</span></span>|
|<span data-ttu-id="7d7cf-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="7d7cf-158">uploadState</span></span>|[<span data-ttu-id="7d7cf-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="7d7cf-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="7d7cf-160">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-160">The state of the current upload request.</span></span> <span data-ttu-id="7d7cf-161">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="7d7cf-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d7cf-162">Response</span></span>
<span data-ttu-id="7d7cf-163">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d7cf-164">Пример</span><span class="sxs-lookup"><span data-stu-id="7d7cf-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d7cf-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="7d7cf-165">Request</span></span>
<span data-ttu-id="7d7cf-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7d7cf-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="7d7cf-167">Response</span></span>
<span data-ttu-id="7d7cf-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7d7cf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



