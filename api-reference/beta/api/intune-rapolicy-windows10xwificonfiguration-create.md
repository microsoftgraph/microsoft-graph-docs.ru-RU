---
title: Создание windows10XWifiConfiguration
description: Создайте новый объект Windows10XWifiConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 08735db11e3cb1c656f80685917d14fb9b58493c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148534"
---
# <a name="create-windows10xwificonfiguration"></a><span data-ttu-id="4fc97-103">Создание windows10XWifiConfiguration</span><span class="sxs-lookup"><span data-stu-id="4fc97-103">Create windows10XWifiConfiguration</span></span>

<span data-ttu-id="4fc97-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fc97-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fc97-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fc97-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fc97-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4fc97-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fc97-107">Создайте [новый объект Windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4fc97-107">Create a new [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fc97-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="4fc97-108">Prerequisites</span></span>
<span data-ttu-id="4fc97-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4fc97-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fc97-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4fc97-111">Permission type</span></span>|<span data-ttu-id="4fc97-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4fc97-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fc97-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4fc97-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fc97-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc97-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4fc97-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4fc97-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fc97-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4fc97-116">Not supported.</span></span>|
|<span data-ttu-id="4fc97-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="4fc97-117">Application</span></span>|<span data-ttu-id="4fc97-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc97-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fc97-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4fc97-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="4fc97-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4fc97-120">Request headers</span></span>
|<span data-ttu-id="4fc97-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4fc97-121">Header</span></span>|<span data-ttu-id="4fc97-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4fc97-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fc97-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fc97-123">Authorization</span></span>|<span data-ttu-id="4fc97-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4fc97-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fc97-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4fc97-125">Accept</span></span>|<span data-ttu-id="4fc97-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fc97-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc97-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4fc97-127">Request body</span></span>
<span data-ttu-id="4fc97-128">В теле запроса поставляем представление JSON для объекта Windows10XWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4fc97-128">In the request body, supply a JSON representation for the windows10XWifiConfiguration object.</span></span>

<span data-ttu-id="4fc97-129">В следующей таблице показаны свойства, необходимые при создании windows10XWifiConfiguration.</span><span class="sxs-lookup"><span data-stu-id="4fc97-129">The following table shows the properties that are required when you create the windows10XWifiConfiguration.</span></span>

|<span data-ttu-id="4fc97-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4fc97-130">Property</span></span>|<span data-ttu-id="4fc97-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4fc97-131">Type</span></span>|<span data-ttu-id="4fc97-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4fc97-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc97-133">id</span><span class="sxs-lookup"><span data-stu-id="4fc97-133">id</span></span>|<span data-ttu-id="4fc97-134">Строка</span><span class="sxs-lookup"><span data-stu-id="4fc97-134">String</span></span>|<span data-ttu-id="4fc97-135">Идентификатор профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4fc97-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="4fc97-136">version</span><span class="sxs-lookup"><span data-stu-id="4fc97-136">version</span></span>|<span data-ttu-id="4fc97-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4fc97-137">Int32</span></span>|<span data-ttu-id="4fc97-138">Версия профиля, унаследованной от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4fc97-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="4fc97-139">displayName</span><span class="sxs-lookup"><span data-stu-id="4fc97-139">displayName</span></span>|<span data-ttu-id="4fc97-140">Строка</span><span class="sxs-lookup"><span data-stu-id="4fc97-140">String</span></span>|<span data-ttu-id="4fc97-141">Имя отображения профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4fc97-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="4fc97-142">description</span><span class="sxs-lookup"><span data-stu-id="4fc97-142">description</span></span>|<span data-ttu-id="4fc97-143">Строка</span><span class="sxs-lookup"><span data-stu-id="4fc97-143">String</span></span>|<span data-ttu-id="4fc97-144">Описание профиля, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4fc97-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="4fc97-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc97-145">creationDateTime</span></span>|<span data-ttu-id="4fc97-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc97-146">DateTimeOffset</span></span>|<span data-ttu-id="4fc97-147">Профиль DateTime был создан по наследству от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4fc97-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="4fc97-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fc97-148">lastModifiedDateTime</span></span>|<span data-ttu-id="4fc97-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fc97-149">DateTimeOffset</span></span>|<span data-ttu-id="4fc97-150">Последний раз был изменен профиль DateTime, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4fc97-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="4fc97-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4fc97-151">roleScopeTagIds</span></span>|<span data-ttu-id="4fc97-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4fc97-152">String collection</span></span>|<span data-ttu-id="4fc97-153">Теги области, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4fc97-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="4fc97-154">authenticationCertificateId</span><span class="sxs-lookup"><span data-stu-id="4fc97-154">authenticationCertificateId</span></span>|<span data-ttu-id="4fc97-155">Guid</span><span class="sxs-lookup"><span data-stu-id="4fc97-155">Guid</span></span>|<span data-ttu-id="4fc97-156">ID к сертификату проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="4fc97-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="4fc97-157">customXmlFileName</span><span class="sxs-lookup"><span data-stu-id="4fc97-157">customXmlFileName</span></span>|<span data-ttu-id="4fc97-158">Строка</span><span class="sxs-lookup"><span data-stu-id="4fc97-158">String</span></span>|<span data-ttu-id="4fc97-159">Пользовательское имя файла Xml.</span><span class="sxs-lookup"><span data-stu-id="4fc97-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="4fc97-160">customXml</span><span class="sxs-lookup"><span data-stu-id="4fc97-160">customXml</span></span>|<span data-ttu-id="4fc97-161">Binary</span><span class="sxs-lookup"><span data-stu-id="4fc97-161">Binary</span></span>|<span data-ttu-id="4fc97-162">Настраиваемые XML-команды, настраиваемые vpn-подключением.</span><span class="sxs-lookup"><span data-stu-id="4fc97-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="4fc97-163">(кодификат byte UTF8)</span><span class="sxs-lookup"><span data-stu-id="4fc97-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="4fc97-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fc97-164">Response</span></span>
<span data-ttu-id="4fc97-165">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4fc97-165">If successful, this method returns a `201 Created` response code and a [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc97-166">Пример</span><span class="sxs-lookup"><span data-stu-id="4fc97-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fc97-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="4fc97-167">Request</span></span>
<span data-ttu-id="4fc97-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4fc97-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
Content-type: application/json
Content-length: 447

{
  "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "authenticationCertificateId": "39b4cd38-cd38-39b4-38cd-b43938cdb439",
  "customXmlFileName": "Custom Xml File Name value",
  "customXml": "Y3VzdG9tWG1s"
}
```

### <a name="response"></a><span data-ttu-id="4fc97-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="4fc97-169">Response</span></span>
<span data-ttu-id="4fc97-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4fc97-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
  "id": "31063b86-3b86-3106-863b-0631863b0631",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "authenticationCertificateId": "39b4cd38-cd38-39b4-38cd-b43938cdb439",
  "customXmlFileName": "Custom Xml File Name value",
  "customXml": "Y3VzdG9tWG1s"
}
```




