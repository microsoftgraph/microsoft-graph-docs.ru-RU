---
title: Создание windows10XTrustedRootCertificate
description: Создайте новый объект Windows10XTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f6ad900d55dface17c96fbfb4ccd3cd7e31ed1ee
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151916"
---
# <a name="create-windows10xtrustedrootcertificate"></a><span data-ttu-id="11b0c-103">Создание windows10XTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="11b0c-103">Create windows10XTrustedRootCertificate</span></span>

<span data-ttu-id="11b0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11b0c-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b0c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11b0c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="11b0c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11b0c-107">Создайте [новый объект Windows10XTrustedRootCertificate.](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md)</span><span class="sxs-lookup"><span data-stu-id="11b0c-107">Create a new [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11b0c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="11b0c-108">Prerequisites</span></span>
<span data-ttu-id="11b0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11b0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11b0c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11b0c-111">Permission type</span></span>|<span data-ttu-id="11b0c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11b0c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11b0c-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11b0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="11b0c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b0c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="11b0c-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11b0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11b0c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11b0c-116">Not supported.</span></span>|
|<span data-ttu-id="11b0c-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="11b0c-117">Application</span></span>|<span data-ttu-id="11b0c-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11b0c-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11b0c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11b0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="11b0c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="11b0c-120">Request headers</span></span>
|<span data-ttu-id="11b0c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="11b0c-121">Header</span></span>|<span data-ttu-id="11b0c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="11b0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11b0c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="11b0c-123">Authorization</span></span>|<span data-ttu-id="11b0c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11b0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11b0c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="11b0c-125">Accept</span></span>|<span data-ttu-id="11b0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="11b0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11b0c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="11b0c-127">Request body</span></span>
<span data-ttu-id="11b0c-128">В теле запроса поставляем представление JSON для объекта Windows10XTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="11b0c-128">In the request body, supply a JSON representation for the windows10XTrustedRootCertificate object.</span></span>

<span data-ttu-id="11b0c-129">В следующей таблице показаны свойства, необходимые при создании windows10XTrustedRootCertificate.</span><span class="sxs-lookup"><span data-stu-id="11b0c-129">The following table shows the properties that are required when you create the windows10XTrustedRootCertificate.</span></span>

|<span data-ttu-id="11b0c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="11b0c-130">Property</span></span>|<span data-ttu-id="11b0c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="11b0c-131">Type</span></span>|<span data-ttu-id="11b0c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="11b0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11b0c-133">id</span><span class="sxs-lookup"><span data-stu-id="11b0c-133">id</span></span>|<span data-ttu-id="11b0c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="11b0c-134">String</span></span>|<span data-ttu-id="11b0c-135">Идентификатор профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="11b0c-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="11b0c-136">version</span><span class="sxs-lookup"><span data-stu-id="11b0c-136">version</span></span>|<span data-ttu-id="11b0c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="11b0c-137">Int32</span></span>|<span data-ttu-id="11b0c-138">Версия профиля, унаследованной от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="11b0c-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="11b0c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="11b0c-139">displayName</span></span>|<span data-ttu-id="11b0c-140">Строка</span><span class="sxs-lookup"><span data-stu-id="11b0c-140">String</span></span>|<span data-ttu-id="11b0c-141">Имя отображения профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="11b0c-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="11b0c-142">description</span><span class="sxs-lookup"><span data-stu-id="11b0c-142">description</span></span>|<span data-ttu-id="11b0c-143">Строка</span><span class="sxs-lookup"><span data-stu-id="11b0c-143">String</span></span>|<span data-ttu-id="11b0c-144">Описание профиля, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="11b0c-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="11b0c-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="11b0c-145">creationDateTime</span></span>|<span data-ttu-id="11b0c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b0c-146">DateTimeOffset</span></span>|<span data-ttu-id="11b0c-147">Профиль DateTime был создан по наследству от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="11b0c-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="11b0c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="11b0c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="11b0c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b0c-149">DateTimeOffset</span></span>|<span data-ttu-id="11b0c-150">Последний раз был изменен профиль DateTime, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="11b0c-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="11b0c-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="11b0c-151">roleScopeTagIds</span></span>|<span data-ttu-id="11b0c-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="11b0c-152">String collection</span></span>|<span data-ttu-id="11b0c-153">Теги области, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="11b0c-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="11b0c-154">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="11b0c-154">trustedRootCertificate</span></span>|<span data-ttu-id="11b0c-155">Binary</span><span class="sxs-lookup"><span data-stu-id="11b0c-155">Binary</span></span>|<span data-ttu-id="11b0c-156">Надежный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="11b0c-156">Trusted Root Certificate</span></span>|
|<span data-ttu-id="11b0c-157">certFileName</span><span class="sxs-lookup"><span data-stu-id="11b0c-157">certFileName</span></span>|<span data-ttu-id="11b0c-158">Строка</span><span class="sxs-lookup"><span data-stu-id="11b0c-158">String</span></span>|<span data-ttu-id="11b0c-159">Имя файла для отображения в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="11b0c-159">File name to display in UI.</span></span>|
|<span data-ttu-id="11b0c-160">destinationStore</span><span class="sxs-lookup"><span data-stu-id="11b0c-160">destinationStore</span></span>|[<span data-ttu-id="11b0c-161">certificateDestinationStore</span><span class="sxs-lookup"><span data-stu-id="11b0c-161">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="11b0c-162">Расположение магазина назначения для доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="11b0c-162">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="11b0c-163">Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="11b0c-163">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="11b0c-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b0c-164">Response</span></span>
<span data-ttu-id="11b0c-165">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект Windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="11b0c-165">If successful, this method returns a `201 Created` response code and a [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11b0c-166">Пример</span><span class="sxs-lookup"><span data-stu-id="11b0c-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="11b0c-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="11b0c-167">Request</span></span>
<span data-ttu-id="11b0c-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="11b0c-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 456

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```

### <a name="response"></a><span data-ttu-id="11b0c-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="11b0c-169">Response</span></span>
<span data-ttu-id="11b0c-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="11b0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 569

{
  "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
  "id": "be0bfd01-fd01-be0b-01fd-0bbe01fd0bbe",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
  "certFileName": "Cert File Name value",
  "destinationStore": "computerCertStoreIntermediate"
}
```




