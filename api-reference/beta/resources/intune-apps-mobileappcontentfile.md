---
title: Тип ресурса mobileAppContentFile
description: Содержит свойства для одного файла установщика, связанного с заданной версией mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 444c2824755d97b78e2ca2e3f1711f2809dacd30
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972917"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="23522-103">Тип ресурса mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23522-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="23522-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23522-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23522-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23522-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23522-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23522-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23522-107">Содержит свойства для одного файла установщика, связанного с заданной версией mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="23522-107">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>
## <a name="methods"></a><span data-ttu-id="23522-108">Методы</span><span class="sxs-lookup"><span data-stu-id="23522-108">Methods</span></span>
|<span data-ttu-id="23522-109">Метод</span><span class="sxs-lookup"><span data-stu-id="23522-109">Method</span></span>|<span data-ttu-id="23522-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="23522-110">Return Type</span></span>|<span data-ttu-id="23522-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23522-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23522-112">Перечисление mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="23522-112">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="23522-113">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="23522-113">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="23522-114">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="23522-114">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="23522-115">Получение mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23522-115">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|[<span data-ttu-id="23522-116">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23522-116">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="23522-117">Считывание свойств и связей объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="23522-117">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="23522-118">Создание mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23522-118">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|[<span data-ttu-id="23522-119">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23522-119">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="23522-120">Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="23522-120">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="23522-121">Удаление mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23522-121">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="23522-122">None</span><span class="sxs-lookup"><span data-stu-id="23522-122">None</span></span>|<span data-ttu-id="23522-123">Удаление экземпляра [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="23522-123">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="23522-124">Обновление mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23522-124">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="23522-125">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="23522-125">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="23522-126">Обновление свойств объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="23522-126">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="23522-127">Действие commit</span><span class="sxs-lookup"><span data-stu-id="23522-127">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="23522-128">None</span><span class="sxs-lookup"><span data-stu-id="23522-128">None</span></span>|<span data-ttu-id="23522-129">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="23522-129">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="23522-130">Действие renewUpload</span><span class="sxs-lookup"><span data-stu-id="23522-130">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="23522-131">None</span><span class="sxs-lookup"><span data-stu-id="23522-131">None</span></span>|<span data-ttu-id="23522-132">Обновляет URI SAS для отправки файла приложения.</span><span class="sxs-lookup"><span data-stu-id="23522-132">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="23522-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="23522-133">Properties</span></span>
|<span data-ttu-id="23522-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="23522-134">Property</span></span>|<span data-ttu-id="23522-135">Тип</span><span class="sxs-lookup"><span data-stu-id="23522-135">Type</span></span>|<span data-ttu-id="23522-136">Описание</span><span class="sxs-lookup"><span data-stu-id="23522-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23522-137">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="23522-137">azureStorageUri</span></span>|<span data-ttu-id="23522-138">String</span><span class="sxs-lookup"><span data-stu-id="23522-138">String</span></span>|<span data-ttu-id="23522-139">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="23522-139">The Azure Storage URI.</span></span>|
|<span data-ttu-id="23522-140">isCommitted</span><span class="sxs-lookup"><span data-stu-id="23522-140">isCommitted</span></span>|<span data-ttu-id="23522-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="23522-141">Boolean</span></span>|<span data-ttu-id="23522-142">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="23522-142">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="23522-143">id</span><span class="sxs-lookup"><span data-stu-id="23522-143">id</span></span>|<span data-ttu-id="23522-144">String</span><span class="sxs-lookup"><span data-stu-id="23522-144">String</span></span>|<span data-ttu-id="23522-145">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="23522-145">The File Id.</span></span>|
|<span data-ttu-id="23522-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23522-146">createdDateTime</span></span>|<span data-ttu-id="23522-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23522-147">DateTimeOffset</span></span>|<span data-ttu-id="23522-148">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="23522-148">The time the file was created.</span></span>|
|<span data-ttu-id="23522-149">name</span><span class="sxs-lookup"><span data-stu-id="23522-149">name</span></span>|<span data-ttu-id="23522-150">String</span><span class="sxs-lookup"><span data-stu-id="23522-150">String</span></span>|<span data-ttu-id="23522-151">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="23522-151">the file name.</span></span>|
|<span data-ttu-id="23522-152">size</span><span class="sxs-lookup"><span data-stu-id="23522-152">size</span></span>|<span data-ttu-id="23522-153">Int64</span><span class="sxs-lookup"><span data-stu-id="23522-153">Int64</span></span>|<span data-ttu-id="23522-154">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="23522-154">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="23522-155">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="23522-155">sizeEncrypted</span></span>|<span data-ttu-id="23522-156">Int64</span><span class="sxs-lookup"><span data-stu-id="23522-156">Int64</span></span>|<span data-ttu-id="23522-157">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="23522-157">The size of the file after encryption.</span></span>|
|<span data-ttu-id="23522-158">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="23522-158">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="23522-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23522-159">DateTimeOffset</span></span>|<span data-ttu-id="23522-160">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="23522-160">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="23522-161">manifest</span><span class="sxs-lookup"><span data-stu-id="23522-161">manifest</span></span>|<span data-ttu-id="23522-162">Binary</span><span class="sxs-lookup"><span data-stu-id="23522-162">Binary</span></span>|<span data-ttu-id="23522-163">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="23522-163">The manifest information.</span></span>|
|<span data-ttu-id="23522-164">uploadState</span><span class="sxs-lookup"><span data-stu-id="23522-164">uploadState</span></span>|[<span data-ttu-id="23522-165">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="23522-165">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="23522-166">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="23522-166">The state of the current upload request.</span></span> <span data-ttu-id="23522-167">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="23522-167">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="23522-168">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="23522-168">isFrameworkFile</span></span>|<span data-ttu-id="23522-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="23522-169">Boolean</span></span>|<span data-ttu-id="23522-170">Значение, указывающее, является ли файл файлом framework.</span><span class="sxs-lookup"><span data-stu-id="23522-170">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="23522-171">isDependency</span><span class="sxs-lookup"><span data-stu-id="23522-171">isDependency</span></span>|<span data-ttu-id="23522-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="23522-172">Boolean</span></span>|<span data-ttu-id="23522-173">Является ли содержимое файла зависимостей для основного содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="23522-173">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23522-174">Связи</span><span class="sxs-lookup"><span data-stu-id="23522-174">Relationships</span></span>
<span data-ttu-id="23522-175">Нет</span><span class="sxs-lookup"><span data-stu-id="23522-175">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23522-176">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23522-176">JSON Representation</span></span>
<span data-ttu-id="23522-177">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23522-177">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContentFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "String",
  "isCommitted": true,
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "sizeEncrypted": 1024,
  "azureStorageUriExpirationDateTime": "String (timestamp)",
  "manifest": "binary",
  "uploadState": "String",
  "isFrameworkFile": true,
  "isDependency": true
}
```





