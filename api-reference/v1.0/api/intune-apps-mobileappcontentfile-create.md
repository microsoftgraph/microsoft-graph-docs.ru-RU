---
title: Создание объекта mobileAppContentFile
description: Создание объекта mobileAppContentFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1423491fcd22901099cf9064a423b1c33a73f428
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37358230"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="1bee6-103">Создание объекта mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="1bee6-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="1bee6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1bee6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bee6-105">Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="1bee6-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1bee6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1bee6-106">Prerequisites</span></span>
<span data-ttu-id="1bee6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bee6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bee6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1bee6-109">Permission type</span></span>|<span data-ttu-id="1bee6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1bee6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bee6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1bee6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1bee6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bee6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1bee6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1bee6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bee6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bee6-114">Not supported.</span></span>|
|<span data-ttu-id="1bee6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1bee6-115">Application</span></span>|<span data-ttu-id="1bee6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1bee6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bee6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1bee6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="1bee6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1bee6-118">Request headers</span></span>
|<span data-ttu-id="1bee6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1bee6-119">Header</span></span>|<span data-ttu-id="1bee6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="1bee6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bee6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="1bee6-121">Authorization</span></span>|<span data-ttu-id="1bee6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1bee6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1bee6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1bee6-123">Accept</span></span>|<span data-ttu-id="1bee6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1bee6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bee6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1bee6-125">Request body</span></span>
<span data-ttu-id="1bee6-126">В тексте запроса добавьте представление объекта mobileAppContentFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1bee6-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="1bee6-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="1bee6-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="1bee6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="1bee6-128">Property</span></span>|<span data-ttu-id="1bee6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="1bee6-129">Type</span></span>|<span data-ttu-id="1bee6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="1bee6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bee6-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="1bee6-131">azureStorageUri</span></span>|<span data-ttu-id="1bee6-132">String</span><span class="sxs-lookup"><span data-stu-id="1bee6-132">String</span></span>|<span data-ttu-id="1bee6-133">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="1bee6-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="1bee6-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="1bee6-134">isCommitted</span></span>|<span data-ttu-id="1bee6-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="1bee6-135">Boolean</span></span>|<span data-ttu-id="1bee6-136">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="1bee6-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="1bee6-137">id</span><span class="sxs-lookup"><span data-stu-id="1bee6-137">id</span></span>|<span data-ttu-id="1bee6-138">Строка</span><span class="sxs-lookup"><span data-stu-id="1bee6-138">String</span></span>|<span data-ttu-id="1bee6-139">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="1bee6-139">The File Id.</span></span>|
|<span data-ttu-id="1bee6-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1bee6-140">createdDateTime</span></span>|<span data-ttu-id="1bee6-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bee6-141">DateTimeOffset</span></span>|<span data-ttu-id="1bee6-142">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="1bee6-142">The time the file was created.</span></span>|
|<span data-ttu-id="1bee6-143">name</span><span class="sxs-lookup"><span data-stu-id="1bee6-143">name</span></span>|<span data-ttu-id="1bee6-144">String</span><span class="sxs-lookup"><span data-stu-id="1bee6-144">String</span></span>|<span data-ttu-id="1bee6-145">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="1bee6-145">the file name.</span></span>|
|<span data-ttu-id="1bee6-146">size</span><span class="sxs-lookup"><span data-stu-id="1bee6-146">size</span></span>|<span data-ttu-id="1bee6-147">Int64</span><span class="sxs-lookup"><span data-stu-id="1bee6-147">Int64</span></span>|<span data-ttu-id="1bee6-148">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="1bee6-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="1bee6-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="1bee6-149">sizeEncrypted</span></span>|<span data-ttu-id="1bee6-150">Int64</span><span class="sxs-lookup"><span data-stu-id="1bee6-150">Int64</span></span>|<span data-ttu-id="1bee6-151">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="1bee6-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="1bee6-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1bee6-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="1bee6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1bee6-153">DateTimeOffset</span></span>|<span data-ttu-id="1bee6-154">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="1bee6-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="1bee6-155">manifest</span><span class="sxs-lookup"><span data-stu-id="1bee6-155">manifest</span></span>|<span data-ttu-id="1bee6-156">Binary</span><span class="sxs-lookup"><span data-stu-id="1bee6-156">Binary</span></span>|<span data-ttu-id="1bee6-157">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="1bee6-157">The manifest information.</span></span>|
|<span data-ttu-id="1bee6-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="1bee6-158">uploadState</span></span>|[<span data-ttu-id="1bee6-159">мобилеаппконтентфилеуплоадстате</span><span class="sxs-lookup"><span data-stu-id="1bee6-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="1bee6-160">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="1bee6-160">The state of the current upload request.</span></span> <span data-ttu-id="1bee6-161">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="1bee6-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="1bee6-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bee6-162">Response</span></span>
<span data-ttu-id="1bee6-163">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1bee6-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bee6-164">Пример</span><span class="sxs-lookup"><span data-stu-id="1bee6-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="1bee6-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="1bee6-165">Request</span></span>
<span data-ttu-id="1bee6-166">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1bee6-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1bee6-167">Отклик</span><span class="sxs-lookup"><span data-stu-id="1bee6-167">Response</span></span>
<span data-ttu-id="1bee6-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1bee6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




