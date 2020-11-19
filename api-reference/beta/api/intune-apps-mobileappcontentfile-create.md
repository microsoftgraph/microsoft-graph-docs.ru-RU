---
title: Создание объекта mobileAppContentFile
description: Создание объекта mobileAppContentFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b81d338601629cbf2de871907d5e9245a500196
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248772"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="ad35e-103">Создание объекта mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="ad35e-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="ad35e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad35e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ad35e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad35e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad35e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad35e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad35e-107">Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="ad35e-107">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ad35e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ad35e-108">Prerequisites</span></span>
<span data-ttu-id="ad35e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad35e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad35e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad35e-111">Permission type</span></span>|<span data-ttu-id="ad35e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad35e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad35e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad35e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad35e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad35e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad35e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad35e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad35e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad35e-116">Not supported.</span></span>|
|<span data-ttu-id="ad35e-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ad35e-117">Application</span></span>|<span data-ttu-id="ad35e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad35e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad35e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad35e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="ad35e-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ad35e-120">Request headers</span></span>
|<span data-ttu-id="ad35e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ad35e-121">Header</span></span>|<span data-ttu-id="ad35e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ad35e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad35e-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad35e-123">Authorization</span></span>|<span data-ttu-id="ad35e-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad35e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad35e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad35e-125">Accept</span></span>|<span data-ttu-id="ad35e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad35e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad35e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad35e-127">Request body</span></span>
<span data-ttu-id="ad35e-128">В тексте запроса добавьте представление объекта mobileAppContentFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad35e-128">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="ad35e-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="ad35e-129">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="ad35e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad35e-130">Property</span></span>|<span data-ttu-id="ad35e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad35e-131">Type</span></span>|<span data-ttu-id="ad35e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad35e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad35e-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="ad35e-133">azureStorageUri</span></span>|<span data-ttu-id="ad35e-134">String</span><span class="sxs-lookup"><span data-stu-id="ad35e-134">String</span></span>|<span data-ttu-id="ad35e-135">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="ad35e-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="ad35e-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="ad35e-136">isCommitted</span></span>|<span data-ttu-id="ad35e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad35e-137">Boolean</span></span>|<span data-ttu-id="ad35e-138">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="ad35e-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="ad35e-139">id</span><span class="sxs-lookup"><span data-stu-id="ad35e-139">id</span></span>|<span data-ttu-id="ad35e-140">String</span><span class="sxs-lookup"><span data-stu-id="ad35e-140">String</span></span>|<span data-ttu-id="ad35e-141">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="ad35e-141">The File Id.</span></span>|
|<span data-ttu-id="ad35e-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad35e-142">createdDateTime</span></span>|<span data-ttu-id="ad35e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad35e-143">DateTimeOffset</span></span>|<span data-ttu-id="ad35e-144">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="ad35e-144">The time the file was created.</span></span>|
|<span data-ttu-id="ad35e-145">name</span><span class="sxs-lookup"><span data-stu-id="ad35e-145">name</span></span>|<span data-ttu-id="ad35e-146">String</span><span class="sxs-lookup"><span data-stu-id="ad35e-146">String</span></span>|<span data-ttu-id="ad35e-147">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="ad35e-147">the file name.</span></span>|
|<span data-ttu-id="ad35e-148">size</span><span class="sxs-lookup"><span data-stu-id="ad35e-148">size</span></span>|<span data-ttu-id="ad35e-149">Int64</span><span class="sxs-lookup"><span data-stu-id="ad35e-149">Int64</span></span>|<span data-ttu-id="ad35e-150">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="ad35e-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="ad35e-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="ad35e-151">sizeEncrypted</span></span>|<span data-ttu-id="ad35e-152">Int64</span><span class="sxs-lookup"><span data-stu-id="ad35e-152">Int64</span></span>|<span data-ttu-id="ad35e-153">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="ad35e-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="ad35e-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ad35e-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="ad35e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad35e-155">DateTimeOffset</span></span>|<span data-ttu-id="ad35e-156">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="ad35e-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="ad35e-157">manifest</span><span class="sxs-lookup"><span data-stu-id="ad35e-157">manifest</span></span>|<span data-ttu-id="ad35e-158">Binary</span><span class="sxs-lookup"><span data-stu-id="ad35e-158">Binary</span></span>|<span data-ttu-id="ad35e-159">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="ad35e-159">The manifest information.</span></span>|
|<span data-ttu-id="ad35e-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="ad35e-160">uploadState</span></span>|[<span data-ttu-id="ad35e-161">мобилеаппконтентфилеуплоадстате</span><span class="sxs-lookup"><span data-stu-id="ad35e-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="ad35e-162">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="ad35e-162">The state of the current upload request.</span></span> <span data-ttu-id="ad35e-163">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="ad35e-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="ad35e-164">исфрамеворкфиле</span><span class="sxs-lookup"><span data-stu-id="ad35e-164">isFrameworkFile</span></span>|<span data-ttu-id="ad35e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad35e-165">Boolean</span></span>|<span data-ttu-id="ad35e-166">Значение, указывающее, является ли файл файлом платформы.</span><span class="sxs-lookup"><span data-stu-id="ad35e-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="ad35e-167">Dependency</span><span class="sxs-lookup"><span data-stu-id="ad35e-167">isDependency</span></span>|<span data-ttu-id="ad35e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad35e-168">Boolean</span></span>|<span data-ttu-id="ad35e-169">Является ли файл содержимого зависимостью от основного файла содержимого.</span><span class="sxs-lookup"><span data-stu-id="ad35e-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="ad35e-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad35e-170">Response</span></span>
<span data-ttu-id="ad35e-171">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ad35e-171">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad35e-172">Пример</span><span class="sxs-lookup"><span data-stu-id="ad35e-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="ad35e-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad35e-173">Request</span></span>
<span data-ttu-id="ad35e-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ad35e-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
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

### <a name="response"></a><span data-ttu-id="ad35e-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad35e-175">Response</span></span>
<span data-ttu-id="ad35e-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ad35e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




