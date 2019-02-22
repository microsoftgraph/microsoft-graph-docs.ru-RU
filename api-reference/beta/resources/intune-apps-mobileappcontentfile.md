---
title: Тип ресурса mobileAppContentFile
description: Содержит свойства для одного файла установщика, связанного с заданной версией mobileAppContent.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9ca5286214f73540472230c64005f8b8b99236d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148113"
---
# <a name="mobileappcontentfile-resource-type"></a><span data-ttu-id="0fc04-103">Тип ресурса mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0fc04-103">mobileAppContentFile resource type</span></span>

> <span data-ttu-id="0fc04-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0fc04-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0fc04-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0fc04-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fc04-106">Содержит свойства для одного файла установщика, связанного с заданной версией mobileAppContent.</span><span class="sxs-lookup"><span data-stu-id="0fc04-106">Contains properties for a single installer file that is associated with a given mobileAppContent version.</span></span>

## <a name="methods"></a><span data-ttu-id="0fc04-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0fc04-107">Methods</span></span>
|<span data-ttu-id="0fc04-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0fc04-108">Method</span></span>|<span data-ttu-id="0fc04-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0fc04-109">Return Type</span></span>|<span data-ttu-id="0fc04-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0fc04-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0fc04-111">Перечисление mobileAppContentFiles</span><span class="sxs-lookup"><span data-stu-id="0fc04-111">List mobileAppContentFiles</span></span>](../api/intune-apps-mobileappcontentfile-list.md)|<span data-ttu-id="0fc04-112">Коллекция [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span><span class="sxs-lookup"><span data-stu-id="0fc04-112">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="0fc04-113">Список свойств и связей объектов [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0fc04-113">List properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) objects.</span></span>|
|[<span data-ttu-id="0fc04-114">Получение mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0fc04-114">Get mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-get.md)|<span data-ttu-id="0fc04-115">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md);</span><span class="sxs-lookup"><span data-stu-id="0fc04-115">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span></span>|<span data-ttu-id="0fc04-116">Считывание свойств и связей объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0fc04-116">Read properties and relationships of the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="0fc04-117">Создание mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0fc04-117">Create mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-create.md)|<span data-ttu-id="0fc04-118">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md);</span><span class="sxs-lookup"><span data-stu-id="0fc04-118">[mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md)</span></span>|<span data-ttu-id="0fc04-119">Создание объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0fc04-119">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="0fc04-120">Удаление mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0fc04-120">Delete mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-delete.md)|<span data-ttu-id="0fc04-121">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc04-121">None</span></span>|<span data-ttu-id="0fc04-122">Удаление экземпляра [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0fc04-122">Deletes a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>|
|[<span data-ttu-id="0fc04-123">Обновление mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0fc04-123">Update mobileAppContentFile</span></span>](../api/intune-apps-mobileappcontentfile-update.md)|[<span data-ttu-id="0fc04-124">mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="0fc04-124">mobileAppContentFile</span></span>](../resources/intune-apps-mobileappcontentfile.md)|<span data-ttu-id="0fc04-125">Обновление свойств объекта [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span><span class="sxs-lookup"><span data-stu-id="0fc04-125">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>|
|[<span data-ttu-id="0fc04-126">Действие commit</span><span class="sxs-lookup"><span data-stu-id="0fc04-126">commit action</span></span>](../api/intune-apps-mobileappcontentfile-commit.md)|<span data-ttu-id="0fc04-127">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc04-127">None</span></span>|<span data-ttu-id="0fc04-128">Подтверждает файл заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="0fc04-128">Commits a file of a given app.</span></span>|
|[<span data-ttu-id="0fc04-129">Действие renewUpload</span><span class="sxs-lookup"><span data-stu-id="0fc04-129">renewUpload action</span></span>](../api/intune-apps-mobileappcontentfile-renewupload.md)|<span data-ttu-id="0fc04-130">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc04-130">None</span></span>|<span data-ttu-id="0fc04-131">Обновляет URI SAS для отправки файла приложения.</span><span class="sxs-lookup"><span data-stu-id="0fc04-131">Renews the SAS URI for an application file upload.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fc04-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="0fc04-132">Properties</span></span>
|<span data-ttu-id="0fc04-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="0fc04-133">Property</span></span>|<span data-ttu-id="0fc04-134">Тип</span><span class="sxs-lookup"><span data-stu-id="0fc04-134">Type</span></span>|<span data-ttu-id="0fc04-135">Описание</span><span class="sxs-lookup"><span data-stu-id="0fc04-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fc04-136">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="0fc04-136">azureStorageUri</span></span>|<span data-ttu-id="0fc04-137">String</span><span class="sxs-lookup"><span data-stu-id="0fc04-137">String</span></span>|<span data-ttu-id="0fc04-138">URI службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="0fc04-138">The Azure Storage URI.</span></span>|
|<span data-ttu-id="0fc04-139">isCommitted</span><span class="sxs-lookup"><span data-stu-id="0fc04-139">isCommitted</span></span>|<span data-ttu-id="0fc04-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="0fc04-140">Boolean</span></span>|<span data-ttu-id="0fc04-141">Значение, указывающее, является ли файл подтвержденным.</span><span class="sxs-lookup"><span data-stu-id="0fc04-141">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="0fc04-142">id</span><span class="sxs-lookup"><span data-stu-id="0fc04-142">id</span></span>|<span data-ttu-id="0fc04-143">String</span><span class="sxs-lookup"><span data-stu-id="0fc04-143">String</span></span>|<span data-ttu-id="0fc04-144">Идентификатор файла.</span><span class="sxs-lookup"><span data-stu-id="0fc04-144">The File Id.</span></span>|
|<span data-ttu-id="0fc04-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0fc04-145">createdDateTime</span></span>|<span data-ttu-id="0fc04-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc04-146">DateTimeOffset</span></span>|<span data-ttu-id="0fc04-147">Время создания файла.</span><span class="sxs-lookup"><span data-stu-id="0fc04-147">The time the file was created.</span></span>|
|<span data-ttu-id="0fc04-148">name</span><span class="sxs-lookup"><span data-stu-id="0fc04-148">name</span></span>|<span data-ttu-id="0fc04-149">String</span><span class="sxs-lookup"><span data-stu-id="0fc04-149">String</span></span>|<span data-ttu-id="0fc04-150">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="0fc04-150">the file name.</span></span>|
|<span data-ttu-id="0fc04-151">size</span><span class="sxs-lookup"><span data-stu-id="0fc04-151">size</span></span>|<span data-ttu-id="0fc04-152">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc04-152">Int64</span></span>|<span data-ttu-id="0fc04-153">Размер файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="0fc04-153">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="0fc04-154">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="0fc04-154">sizeEncrypted</span></span>|<span data-ttu-id="0fc04-155">Int64</span><span class="sxs-lookup"><span data-stu-id="0fc04-155">Int64</span></span>|<span data-ttu-id="0fc04-156">Размер файла после шифрования.</span><span class="sxs-lookup"><span data-stu-id="0fc04-156">The size of the file after encryption.</span></span>|
|<span data-ttu-id="0fc04-157">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0fc04-157">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="0fc04-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0fc04-158">DateTimeOffset</span></span>|<span data-ttu-id="0fc04-159">Время, когда заканчивается срок действия URI для службы хранилища Azure.</span><span class="sxs-lookup"><span data-stu-id="0fc04-159">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="0fc04-160">manifest</span><span class="sxs-lookup"><span data-stu-id="0fc04-160">manifest</span></span>|<span data-ttu-id="0fc04-161">Binary</span><span class="sxs-lookup"><span data-stu-id="0fc04-161">Binary</span></span>|<span data-ttu-id="0fc04-162">Данные манифеста.</span><span class="sxs-lookup"><span data-stu-id="0fc04-162">The manifest information.</span></span>|
|<span data-ttu-id="0fc04-163">uploadState</span><span class="sxs-lookup"><span data-stu-id="0fc04-163">uploadState</span></span>|[<span data-ttu-id="0fc04-164">Мобилеаппконтентфилеуплоадстате</span><span class="sxs-lookup"><span data-stu-id="0fc04-164">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="0fc04-165">Состояние текущего запроса на отправку.</span><span class="sxs-lookup"><span data-stu-id="0fc04-165">The state of the current upload request.</span></span> <span data-ttu-id="0fc04-166">Возможные значения: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span><span class="sxs-lookup"><span data-stu-id="0fc04-166">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="0fc04-167">Исфрамеворкфиле</span><span class="sxs-lookup"><span data-stu-id="0fc04-167">isFrameworkFile</span></span>|<span data-ttu-id="0fc04-168">Логический</span><span class="sxs-lookup"><span data-stu-id="0fc04-168">Boolean</span></span>|<span data-ttu-id="0fc04-169">Значение, указывающее, является ли файл файлом платформы.</span><span class="sxs-lookup"><span data-stu-id="0fc04-169">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="0fc04-170">Dependency</span><span class="sxs-lookup"><span data-stu-id="0fc04-170">isDependency</span></span>|<span data-ttu-id="0fc04-171">Логический</span><span class="sxs-lookup"><span data-stu-id="0fc04-171">Boolean</span></span>|<span data-ttu-id="0fc04-172">Является ли файл содержимого зависимостью от основного файла содержимого.</span><span class="sxs-lookup"><span data-stu-id="0fc04-172">Whether the content file is a dependency for the main content file.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fc04-173">Отношения</span><span class="sxs-lookup"><span data-stu-id="0fc04-173">Relationships</span></span>
<span data-ttu-id="0fc04-174">Нет</span><span class="sxs-lookup"><span data-stu-id="0fc04-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fc04-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0fc04-175">JSON Representation</span></span>
<span data-ttu-id="0fc04-176">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0fc04-176">Here is a JSON representation of the resource.</span></span>
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




