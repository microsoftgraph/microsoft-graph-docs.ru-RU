---
title: Создание объекта mobileAppContentFile
description: Создание объекта mobileAppContentFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43e56cbf1fd3419cae2d0b88ac64225985e07b5f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167006"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="30bbd-103">Создание объекта mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="30bbd-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="30bbd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30bbd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30bbd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30bbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30bbd-106">Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="30bbd-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="30bbd-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="30bbd-107">Prerequisites</span></span>
<span data-ttu-id="30bbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="30bbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="30bbd-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30bbd-110">Permission type</span></span>|<span data-ttu-id="30bbd-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30bbd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30bbd-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30bbd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="30bbd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30bbd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30bbd-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30bbd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30bbd-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30bbd-115">Not supported.</span></span>|
|<span data-ttu-id="30bbd-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30bbd-116">Application</span></span>|<span data-ttu-id="30bbd-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30bbd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30bbd-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30bbd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="30bbd-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30bbd-119">Request headers</span></span>
|<span data-ttu-id="30bbd-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30bbd-120">Header</span></span>|<span data-ttu-id="30bbd-121">Значение</span><span class="sxs-lookup"><span data-stu-id="30bbd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30bbd-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="30bbd-122">Authorization</span></span>|<span data-ttu-id="30bbd-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="30bbd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30bbd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="30bbd-124">Accept</span></span>|<span data-ttu-id="30bbd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="30bbd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30bbd-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="30bbd-126">Request body</span></span>
<span data-ttu-id="30bbd-127">В тексте запроса добавьте представление объекта mobileAppContentFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30bbd-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="30bbd-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="30bbd-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="30bbd-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="30bbd-129">Property</span></span>|<span data-ttu-id="30bbd-130">Тип</span><span class="sxs-lookup"><span data-stu-id="30bbd-130">Type</span></span>|<span data-ttu-id="30bbd-131">Описание</span><span class="sxs-lookup"><span data-stu-id="30bbd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30bbd-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="30bbd-132">azureStorageUri</span></span>|<span data-ttu-id="30bbd-133">String</span><span class="sxs-lookup"><span data-stu-id="30bbd-133">String</span></span>|<span data-ttu-id="30bbd-134">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="30bbd-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="30bbd-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="30bbd-135">isCommitted</span></span>|<span data-ttu-id="30bbd-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="30bbd-136">Boolean</span></span>|<span data-ttu-id="30bbd-137">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="30bbd-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="30bbd-138">id</span><span class="sxs-lookup"><span data-stu-id="30bbd-138">id</span></span>|<span data-ttu-id="30bbd-139">String</span><span class="sxs-lookup"><span data-stu-id="30bbd-139">String</span></span>|<span data-ttu-id="30bbd-140">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="30bbd-140">The File Id.</span></span>|
|<span data-ttu-id="30bbd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30bbd-141">createdDateTime</span></span>|<span data-ttu-id="30bbd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30bbd-142">DateTimeOffset</span></span>|<span data-ttu-id="30bbd-143">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="30bbd-143">The time the file was created.</span></span>|
|<span data-ttu-id="30bbd-144">name</span><span class="sxs-lookup"><span data-stu-id="30bbd-144">name</span></span>|<span data-ttu-id="30bbd-145">String</span><span class="sxs-lookup"><span data-stu-id="30bbd-145">String</span></span>|<span data-ttu-id="30bbd-146">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="30bbd-146">the file name.</span></span>|
|<span data-ttu-id="30bbd-147">size</span><span class="sxs-lookup"><span data-stu-id="30bbd-147">size</span></span>|<span data-ttu-id="30bbd-148">Int64</span><span class="sxs-lookup"><span data-stu-id="30bbd-148">Int64</span></span>|<span data-ttu-id="30bbd-149">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="30bbd-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="30bbd-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="30bbd-150">sizeEncrypted</span></span>|<span data-ttu-id="30bbd-151">Int64</span><span class="sxs-lookup"><span data-stu-id="30bbd-151">Int64</span></span>|<span data-ttu-id="30bbd-152">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="30bbd-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="30bbd-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="30bbd-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="30bbd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30bbd-154">DateTimeOffset</span></span>|<span data-ttu-id="30bbd-155">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="30bbd-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="30bbd-156">manifest</span><span class="sxs-lookup"><span data-stu-id="30bbd-156">manifest</span></span>|<span data-ttu-id="30bbd-157">Binary</span><span class="sxs-lookup"><span data-stu-id="30bbd-157">Binary</span></span>|<span data-ttu-id="30bbd-158">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="30bbd-158">The manifest information.</span></span>|
|<span data-ttu-id="30bbd-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="30bbd-159">uploadState</span></span>|[<span data-ttu-id="30bbd-160">Мобилеаппконтентфилеуплоадстате</span><span class="sxs-lookup"><span data-stu-id="30bbd-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="30bbd-161">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="30bbd-161">The state of the current upload request.</span></span> <span data-ttu-id="30bbd-162">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="30bbd-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="30bbd-163">Исфрамеворкфиле</span><span class="sxs-lookup"><span data-stu-id="30bbd-163">isFrameworkFile</span></span>|<span data-ttu-id="30bbd-164">Логический</span><span class="sxs-lookup"><span data-stu-id="30bbd-164">Boolean</span></span>|<span data-ttu-id="30bbd-165">Значение, указывающее, является ли файл файлом платформы.</span><span class="sxs-lookup"><span data-stu-id="30bbd-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="30bbd-166">Dependency</span><span class="sxs-lookup"><span data-stu-id="30bbd-166">isDependency</span></span>|<span data-ttu-id="30bbd-167">Логический</span><span class="sxs-lookup"><span data-stu-id="30bbd-167">Boolean</span></span>|<span data-ttu-id="30bbd-168">Является ли файл содержимого зависимостью от основного файла содержимого.</span><span class="sxs-lookup"><span data-stu-id="30bbd-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="30bbd-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="30bbd-169">Response</span></span>
<span data-ttu-id="30bbd-170">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="30bbd-170">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30bbd-171">Пример</span><span class="sxs-lookup"><span data-stu-id="30bbd-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="30bbd-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="30bbd-172">Request</span></span>
<span data-ttu-id="30bbd-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30bbd-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30bbd-174">Ответ</span><span class="sxs-lookup"><span data-stu-id="30bbd-174">Response</span></span>
<span data-ttu-id="30bbd-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="30bbd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




