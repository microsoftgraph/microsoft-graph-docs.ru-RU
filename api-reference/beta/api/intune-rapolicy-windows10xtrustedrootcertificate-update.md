---
title: Обновление windows10XTrustedRootCertificate
description: Обновление свойств объекта windows10XTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2ea11d39cd1a5a29a52dca8ef9d1e043c634fed2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242408"
---
# <a name="update-windows10xtrustedrootcertificate"></a><span data-ttu-id="244f6-103">Обновление windows10XTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="244f6-103">Update windows10XTrustedRootCertificate</span></span>

<span data-ttu-id="244f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="244f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="244f6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="244f6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="244f6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="244f6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="244f6-107">Обновление свойств объекта [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) .</span><span class="sxs-lookup"><span data-stu-id="244f6-107">Update the properties of a [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="244f6-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="244f6-108">Prerequisites</span></span>
<span data-ttu-id="244f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="244f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="244f6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="244f6-111">Permission type</span></span>|<span data-ttu-id="244f6-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="244f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="244f6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="244f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="244f6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="244f6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="244f6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="244f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="244f6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="244f6-116">Not supported.</span></span>|
|<span data-ttu-id="244f6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="244f6-117">Application</span></span>|<span data-ttu-id="244f6-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="244f6-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="244f6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="244f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="244f6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="244f6-120">Request headers</span></span>
|<span data-ttu-id="244f6-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="244f6-121">Header</span></span>|<span data-ttu-id="244f6-122">Значение</span><span class="sxs-lookup"><span data-stu-id="244f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="244f6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="244f6-123">Authorization</span></span>|<span data-ttu-id="244f6-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="244f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="244f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="244f6-125">Accept</span></span>|<span data-ttu-id="244f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="244f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="244f6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="244f6-127">Request body</span></span>
<span data-ttu-id="244f6-128">В тексте запроса добавьте представление объекта [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="244f6-128">In the request body, supply a JSON representation for the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object.</span></span>

<span data-ttu-id="244f6-129">В следующей таблице приведены свойства, необходимые при создании [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="244f6-129">The following table shows the properties that are required when you create the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md).</span></span>

|<span data-ttu-id="244f6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="244f6-130">Property</span></span>|<span data-ttu-id="244f6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="244f6-131">Type</span></span>|<span data-ttu-id="244f6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="244f6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="244f6-133">id</span><span class="sxs-lookup"><span data-stu-id="244f6-133">id</span></span>|<span data-ttu-id="244f6-134">String</span><span class="sxs-lookup"><span data-stu-id="244f6-134">String</span></span>|<span data-ttu-id="244f6-135">Идентификатор профиля унаследован от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="244f6-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="244f6-136">version</span><span class="sxs-lookup"><span data-stu-id="244f6-136">version</span></span>|<span data-ttu-id="244f6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="244f6-137">Int32</span></span>|<span data-ttu-id="244f6-138">Версия профиля, унаследованного от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="244f6-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="244f6-139">displayName</span><span class="sxs-lookup"><span data-stu-id="244f6-139">displayName</span></span>|<span data-ttu-id="244f6-140">String</span><span class="sxs-lookup"><span data-stu-id="244f6-140">String</span></span>|<span data-ttu-id="244f6-141">Отображаемое имя профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="244f6-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="244f6-142">description</span><span class="sxs-lookup"><span data-stu-id="244f6-142">description</span></span>|<span data-ttu-id="244f6-143">String</span><span class="sxs-lookup"><span data-stu-id="244f6-143">String</span></span>|<span data-ttu-id="244f6-144">Описание профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="244f6-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="244f6-145">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="244f6-145">creationDateTime</span></span>|<span data-ttu-id="244f6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="244f6-146">DateTimeOffset</span></span>|<span data-ttu-id="244f6-147">Создан профиль DateTime, наследуемый от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="244f6-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="244f6-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="244f6-148">lastModifiedDateTime</span></span>|<span data-ttu-id="244f6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="244f6-149">DateTimeOffset</span></span>|<span data-ttu-id="244f6-150">Последнее изменение профиля DateTime унаследовано от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="244f6-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="244f6-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="244f6-151">roleScopeTagIds</span></span>|<span data-ttu-id="244f6-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="244f6-152">String collection</span></span>|<span data-ttu-id="244f6-153">Теги областей унаследованы от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="244f6-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="244f6-154">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="244f6-154">trustedRootCertificate</span></span>|<span data-ttu-id="244f6-155">Binary</span><span class="sxs-lookup"><span data-stu-id="244f6-155">Binary</span></span>|<span data-ttu-id="244f6-156">Доверенный корневой сертификат</span><span class="sxs-lookup"><span data-stu-id="244f6-156">Trusted Root Certificate</span></span>|
|<span data-ttu-id="244f6-157">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="244f6-157">certFileName</span></span>|<span data-ttu-id="244f6-158">String</span><span class="sxs-lookup"><span data-stu-id="244f6-158">String</span></span>|<span data-ttu-id="244f6-159">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="244f6-159">File name to display in UI.</span></span>|
|<span data-ttu-id="244f6-160">дестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="244f6-160">destinationStore</span></span>|[<span data-ttu-id="244f6-161">цертификатедестинатионсторе</span><span class="sxs-lookup"><span data-stu-id="244f6-161">certificateDestinationStore</span></span>](../resources/intune-shared-certificatedestinationstore.md)|<span data-ttu-id="244f6-162">Расположение хранилища назначения для доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="244f6-162">Destination store location for the Trusted Root Certificate.</span></span> <span data-ttu-id="244f6-163">Возможные значения: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span><span class="sxs-lookup"><span data-stu-id="244f6-163">Possible values are: `computerCertStoreRoot`, `computerCertStoreIntermediate`, `userCertStoreIntermediate`.</span></span>|



## <a name="response"></a><span data-ttu-id="244f6-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="244f6-164">Response</span></span>
<span data-ttu-id="244f6-165">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="244f6-165">If successful, this method returns a `200 OK` response code and an updated [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="244f6-166">Пример</span><span class="sxs-lookup"><span data-stu-id="244f6-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="244f6-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="244f6-167">Request</span></span>
<span data-ttu-id="244f6-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="244f6-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
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

### <a name="response"></a><span data-ttu-id="244f6-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="244f6-169">Response</span></span>
<span data-ttu-id="244f6-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="244f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




