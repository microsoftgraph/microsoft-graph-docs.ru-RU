---
title: Update mobileAppContentFile
description: Обновление свойств объекта mobileAppContentFile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ad2ad1796bd4c4dacb7c07d28882f14da7f8610
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973854"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="5978f-103">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="5978f-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="5978f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5978f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5978f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5978f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5978f-106">Обновление свойств объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="5978f-106">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5978f-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="5978f-107">Prerequisites</span></span>
<span data-ttu-id="5978f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5978f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5978f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5978f-110">Permission type</span></span>|<span data-ttu-id="5978f-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5978f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5978f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5978f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5978f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5978f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5978f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5978f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5978f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5978f-115">Not supported.</span></span>|
|<span data-ttu-id="5978f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5978f-116">Application</span></span>|<span data-ttu-id="5978f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5978f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5978f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5978f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="5978f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5978f-119">Request headers</span></span>
|<span data-ttu-id="5978f-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5978f-120">Header</span></span>|<span data-ttu-id="5978f-121">Значение</span><span class="sxs-lookup"><span data-stu-id="5978f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5978f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5978f-122">Authorization</span></span>|<span data-ttu-id="5978f-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5978f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5978f-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5978f-124">Accept</span></span>|<span data-ttu-id="5978f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5978f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5978f-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5978f-126">Request body</span></span>
<span data-ttu-id="5978f-127">В теле запроса добавьте представление объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5978f-127">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="5978f-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="5978f-128">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="5978f-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="5978f-129">Property</span></span>|<span data-ttu-id="5978f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="5978f-130">Type</span></span>|<span data-ttu-id="5978f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="5978f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5978f-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="5978f-132">azureStorageUri</span></span>|<span data-ttu-id="5978f-133">String</span><span class="sxs-lookup"><span data-stu-id="5978f-133">String</span></span>|<span data-ttu-id="5978f-134">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="5978f-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="5978f-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="5978f-135">isCommitted</span></span>|<span data-ttu-id="5978f-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="5978f-136">Boolean</span></span>|<span data-ttu-id="5978f-137">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="5978f-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="5978f-138">id</span><span class="sxs-lookup"><span data-stu-id="5978f-138">id</span></span>|<span data-ttu-id="5978f-139">Строка</span><span class="sxs-lookup"><span data-stu-id="5978f-139">String</span></span>|<span data-ttu-id="5978f-140">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="5978f-140">The File Id.</span></span>|
|<span data-ttu-id="5978f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5978f-141">createdDateTime</span></span>|<span data-ttu-id="5978f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5978f-142">DateTimeOffset</span></span>|<span data-ttu-id="5978f-143">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="5978f-143">The time the file was created.</span></span>|
|<span data-ttu-id="5978f-144">name</span><span class="sxs-lookup"><span data-stu-id="5978f-144">name</span></span>|<span data-ttu-id="5978f-145">String</span><span class="sxs-lookup"><span data-stu-id="5978f-145">String</span></span>|<span data-ttu-id="5978f-146">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="5978f-146">the file name.</span></span>|
|<span data-ttu-id="5978f-147">size</span><span class="sxs-lookup"><span data-stu-id="5978f-147">size</span></span>|<span data-ttu-id="5978f-148">Int64</span><span class="sxs-lookup"><span data-stu-id="5978f-148">Int64</span></span>|<span data-ttu-id="5978f-149">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="5978f-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="5978f-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="5978f-150">sizeEncrypted</span></span>|<span data-ttu-id="5978f-151">Int64</span><span class="sxs-lookup"><span data-stu-id="5978f-151">Int64</span></span>|<span data-ttu-id="5978f-152">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="5978f-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="5978f-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5978f-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="5978f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5978f-154">DateTimeOffset</span></span>|<span data-ttu-id="5978f-155">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="5978f-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="5978f-156">manifest</span><span class="sxs-lookup"><span data-stu-id="5978f-156">manifest</span></span>|<span data-ttu-id="5978f-157">Binary</span><span class="sxs-lookup"><span data-stu-id="5978f-157">Binary</span></span>|<span data-ttu-id="5978f-158">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="5978f-158">The manifest information.</span></span>|
|<span data-ttu-id="5978f-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="5978f-159">uploadState</span></span>|[<span data-ttu-id="5978f-160">Мобилеаппконтентфилеуплоадстате</span><span class="sxs-lookup"><span data-stu-id="5978f-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="5978f-161">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="5978f-161">The state of the current upload request.</span></span> <span data-ttu-id="5978f-162">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="5978f-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="5978f-163">Исфрамеворкфиле</span><span class="sxs-lookup"><span data-stu-id="5978f-163">isFrameworkFile</span></span>|<span data-ttu-id="5978f-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="5978f-164">Boolean</span></span>|<span data-ttu-id="5978f-165">Значение, указывающее, является ли файл файлом платформы.</span><span class="sxs-lookup"><span data-stu-id="5978f-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="5978f-166">Dependency</span><span class="sxs-lookup"><span data-stu-id="5978f-166">isDependency</span></span>|<span data-ttu-id="5978f-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="5978f-167">Boolean</span></span>|<span data-ttu-id="5978f-168">Является ли файл содержимого зависимостью от основного файла содержимого.</span><span class="sxs-lookup"><span data-stu-id="5978f-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="5978f-169">Ответ</span><span class="sxs-lookup"><span data-stu-id="5978f-169">Response</span></span>
<span data-ttu-id="5978f-170">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5978f-170">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5978f-171">Пример</span><span class="sxs-lookup"><span data-stu-id="5978f-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="5978f-172">Запрос</span><span class="sxs-lookup"><span data-stu-id="5978f-172">Request</span></span>
<span data-ttu-id="5978f-173">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5978f-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5978f-174">Отклик</span><span class="sxs-lookup"><span data-stu-id="5978f-174">Response</span></span>
<span data-ttu-id="5978f-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5978f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





