---
title: Создание объекта mobileAppContentFile
description: Создание объекта mobileAppContentFile.
author: tfitzmac
ms.openlocfilehash: 456ac0f136c8d118dcc0b3fcbe165170da918aa6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356632"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="76b7d-103">Создание объекта mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="76b7d-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="76b7d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="76b7d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76b7d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76b7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76b7d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="76b7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76b7d-107">Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="76b7d-107">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="76b7d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="76b7d-108">Prerequisites</span></span>
<span data-ttu-id="76b7d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76b7d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76b7d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76b7d-111">Permission type</span></span>|<span data-ttu-id="76b7d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="76b7d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76b7d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76b7d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76b7d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76b7d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="76b7d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76b7d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76b7d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76b7d-116">Not supported.</span></span>|
|<span data-ttu-id="76b7d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76b7d-117">Application</span></span>|<span data-ttu-id="76b7d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76b7d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76b7d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76b7d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="76b7d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76b7d-120">Request headers</span></span>
|<span data-ttu-id="76b7d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="76b7d-121">Header</span></span>|<span data-ttu-id="76b7d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="76b7d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76b7d-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76b7d-123">Authorization</span></span>|<span data-ttu-id="76b7d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="76b7d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76b7d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76b7d-125">Accept</span></span>|<span data-ttu-id="76b7d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76b7d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76b7d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76b7d-127">Request body</span></span>
<span data-ttu-id="76b7d-128">В тексте запроса добавьте представление объекта mobileAppContentFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76b7d-128">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="76b7d-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта mobileAppContentFile.</span><span class="sxs-lookup"><span data-stu-id="76b7d-129">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="76b7d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="76b7d-130">Property</span></span>|<span data-ttu-id="76b7d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="76b7d-131">Type</span></span>|<span data-ttu-id="76b7d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="76b7d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b7d-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="76b7d-133">azureStorageUri</span></span>|<span data-ttu-id="76b7d-134">String</span><span class="sxs-lookup"><span data-stu-id="76b7d-134">String</span></span>|<span data-ttu-id="76b7d-135">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="76b7d-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="76b7d-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="76b7d-136">isCommitted</span></span>|<span data-ttu-id="76b7d-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="76b7d-137">Boolean</span></span>|<span data-ttu-id="76b7d-138">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="76b7d-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="76b7d-139">id</span><span class="sxs-lookup"><span data-stu-id="76b7d-139">id</span></span>|<span data-ttu-id="76b7d-140">String</span><span class="sxs-lookup"><span data-stu-id="76b7d-140">String</span></span>|<span data-ttu-id="76b7d-141">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="76b7d-141">The File Id.</span></span>|
|<span data-ttu-id="76b7d-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76b7d-142">createdDateTime</span></span>|<span data-ttu-id="76b7d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76b7d-143">DateTimeOffset</span></span>|<span data-ttu-id="76b7d-144">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="76b7d-144">The time the file was created.</span></span>|
|<span data-ttu-id="76b7d-145">name</span><span class="sxs-lookup"><span data-stu-id="76b7d-145">name</span></span>|<span data-ttu-id="76b7d-146">String</span><span class="sxs-lookup"><span data-stu-id="76b7d-146">String</span></span>|<span data-ttu-id="76b7d-147">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="76b7d-147">the file name.</span></span>|
|<span data-ttu-id="76b7d-148">size</span><span class="sxs-lookup"><span data-stu-id="76b7d-148">size</span></span>|<span data-ttu-id="76b7d-149">Int64</span><span class="sxs-lookup"><span data-stu-id="76b7d-149">Int64</span></span>|<span data-ttu-id="76b7d-150">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="76b7d-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="76b7d-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="76b7d-151">sizeEncrypted</span></span>|<span data-ttu-id="76b7d-152">Int64</span><span class="sxs-lookup"><span data-stu-id="76b7d-152">Int64</span></span>|<span data-ttu-id="76b7d-153">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="76b7d-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="76b7d-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="76b7d-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="76b7d-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76b7d-155">DateTimeOffset</span></span>|<span data-ttu-id="76b7d-156">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="76b7d-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="76b7d-157">manifest</span><span class="sxs-lookup"><span data-stu-id="76b7d-157">manifest</span></span>|<span data-ttu-id="76b7d-158">Binary</span><span class="sxs-lookup"><span data-stu-id="76b7d-158">Binary</span></span>|<span data-ttu-id="76b7d-159">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="76b7d-159">The manifest information.</span></span>|
|<span data-ttu-id="76b7d-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="76b7d-160">uploadState</span></span>|[<span data-ttu-id="76b7d-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="76b7d-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="76b7d-162">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="76b7d-162">The state of the current upload request.</span></span> <span data-ttu-id="76b7d-163">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="76b7d-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="76b7d-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="76b7d-164">isFrameworkFile</span></span>|<span data-ttu-id="76b7d-165">Boolean.</span><span class="sxs-lookup"><span data-stu-id="76b7d-165">Boolean</span></span>|<span data-ttu-id="76b7d-166">Значение, указывающее, является ли файл файлом framework.</span><span class="sxs-lookup"><span data-stu-id="76b7d-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="76b7d-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="76b7d-167">isDependency</span></span>|<span data-ttu-id="76b7d-168">Boolean.</span><span class="sxs-lookup"><span data-stu-id="76b7d-168">Boolean</span></span>|<span data-ttu-id="76b7d-169">Является ли содержимое файла зависимостей для основного содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="76b7d-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="76b7d-170">Отклик</span><span class="sxs-lookup"><span data-stu-id="76b7d-170">Response</span></span>
<span data-ttu-id="76b7d-171">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76b7d-171">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76b7d-172">Пример</span><span class="sxs-lookup"><span data-stu-id="76b7d-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="76b7d-173">Запрос</span><span class="sxs-lookup"><span data-stu-id="76b7d-173">Request</span></span>
<span data-ttu-id="76b7d-174">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76b7d-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76b7d-175">Ответ</span><span class="sxs-lookup"><span data-stu-id="76b7d-175">Response</span></span>
<span data-ttu-id="76b7d-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="76b7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





