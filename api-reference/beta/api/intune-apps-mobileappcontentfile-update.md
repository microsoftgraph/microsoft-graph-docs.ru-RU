---
title: Update mobileAppContentFile
description: Обновление свойств объекта mobileAppContentFile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7ea27b495c8ca3213eb46a1cfc60dc6045d63526
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413180"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="0c840-103">Update mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0c840-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="0c840-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c840-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c840-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c840-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c840-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c840-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c840-107">Обновление свойств объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0c840-107">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c840-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0c840-108">Prerequisites</span></span>
<span data-ttu-id="0c840-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0c840-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0c840-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0c840-111">Permission type</span></span>|<span data-ttu-id="0c840-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0c840-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c840-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0c840-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c840-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c840-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c840-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0c840-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c840-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c840-116">Not supported.</span></span>|
|<span data-ttu-id="0c840-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0c840-117">Application</span></span>|<span data-ttu-id="0c840-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c840-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c840-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0c840-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="0c840-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0c840-120">Request headers</span></span>
|<span data-ttu-id="0c840-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0c840-121">Header</span></span>|<span data-ttu-id="0c840-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0c840-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c840-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c840-123">Authorization</span></span>|<span data-ttu-id="0c840-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0c840-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c840-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c840-125">Accept</span></span>|<span data-ttu-id="0c840-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c840-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c840-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0c840-127">Request body</span></span>
<span data-ttu-id="0c840-128">В теле запроса добавьте представление объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c840-128">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="0c840-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0c840-129">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="0c840-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c840-130">Property</span></span>|<span data-ttu-id="0c840-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0c840-131">Type</span></span>|<span data-ttu-id="0c840-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0c840-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c840-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="0c840-133">azureStorageUri</span></span>|<span data-ttu-id="0c840-134">String</span><span class="sxs-lookup"><span data-stu-id="0c840-134">String</span></span>|<span data-ttu-id="0c840-135">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="0c840-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="0c840-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="0c840-136">isCommitted</span></span>|<span data-ttu-id="0c840-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c840-137">Boolean</span></span>|<span data-ttu-id="0c840-138">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="0c840-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="0c840-139">id</span><span class="sxs-lookup"><span data-stu-id="0c840-139">id</span></span>|<span data-ttu-id="0c840-140">String</span><span class="sxs-lookup"><span data-stu-id="0c840-140">String</span></span>|<span data-ttu-id="0c840-141">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="0c840-141">The File Id.</span></span>|
|<span data-ttu-id="0c840-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0c840-142">createdDateTime</span></span>|<span data-ttu-id="0c840-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c840-143">DateTimeOffset</span></span>|<span data-ttu-id="0c840-144">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="0c840-144">The time the file was created.</span></span>|
|<span data-ttu-id="0c840-145">name</span><span class="sxs-lookup"><span data-stu-id="0c840-145">name</span></span>|<span data-ttu-id="0c840-146">String</span><span class="sxs-lookup"><span data-stu-id="0c840-146">String</span></span>|<span data-ttu-id="0c840-147">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="0c840-147">the file name.</span></span>|
|<span data-ttu-id="0c840-148">size</span><span class="sxs-lookup"><span data-stu-id="0c840-148">size</span></span>|<span data-ttu-id="0c840-149">Int64</span><span class="sxs-lookup"><span data-stu-id="0c840-149">Int64</span></span>|<span data-ttu-id="0c840-150">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="0c840-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="0c840-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="0c840-151">sizeEncrypted</span></span>|<span data-ttu-id="0c840-152">Int64</span><span class="sxs-lookup"><span data-stu-id="0c840-152">Int64</span></span>|<span data-ttu-id="0c840-153">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="0c840-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="0c840-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0c840-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="0c840-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c840-155">DateTimeOffset</span></span>|<span data-ttu-id="0c840-156">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="0c840-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="0c840-157">manifest</span><span class="sxs-lookup"><span data-stu-id="0c840-157">manifest</span></span>|<span data-ttu-id="0c840-158">Binary</span><span class="sxs-lookup"><span data-stu-id="0c840-158">Binary</span></span>|<span data-ttu-id="0c840-159">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="0c840-159">The manifest information.</span></span>|
|<span data-ttu-id="0c840-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="0c840-160">uploadState</span></span>|[<span data-ttu-id="0c840-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="0c840-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="0c840-162">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="0c840-162">The state of the current upload request.</span></span> <span data-ttu-id="0c840-163">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="0c840-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="0c840-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="0c840-164">isFrameworkFile</span></span>|<span data-ttu-id="0c840-165">Логический</span><span class="sxs-lookup"><span data-stu-id="0c840-165">Boolean</span></span>|<span data-ttu-id="0c840-166">Значение, указывающее, является ли файл файлом framework.</span><span class="sxs-lookup"><span data-stu-id="0c840-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="0c840-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="0c840-167">isDependency</span></span>|<span data-ttu-id="0c840-168">Логический</span><span class="sxs-lookup"><span data-stu-id="0c840-168">Boolean</span></span>|<span data-ttu-id="0c840-169">Является ли содержимое файла зависимостей для основного содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="0c840-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="0c840-170">Ответ</span><span class="sxs-lookup"><span data-stu-id="0c840-170">Response</span></span>
<span data-ttu-id="0c840-171">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0c840-171">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c840-172">Пример</span><span class="sxs-lookup"><span data-stu-id="0c840-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c840-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="0c840-173">Request</span></span>
<span data-ttu-id="0c840-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0c840-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c840-175">Отклик</span><span class="sxs-lookup"><span data-stu-id="0c840-175">Response</span></span>
<span data-ttu-id="0c840-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0c840-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




