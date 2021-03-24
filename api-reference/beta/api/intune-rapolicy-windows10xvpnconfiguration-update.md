---
title: Обновление windows10XVpnConfiguration
description: Обновление свойств объекта Windows10XVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c0d4bfc96fb84139175ed9ae32ea54c165eca17e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144986"
---
# <a name="update-windows10xvpnconfiguration"></a><span data-ttu-id="16aaf-103">Обновление windows10XVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="16aaf-103">Update windows10XVpnConfiguration</span></span>

<span data-ttu-id="16aaf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16aaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16aaf-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16aaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16aaf-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16aaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16aaf-107">Обновление свойств объекта [Windows10XVpnConfiguration.](../resources/intune-rapolicy-windows10xvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-107">Update the properties of a [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16aaf-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="16aaf-108">Prerequisites</span></span>
<span data-ttu-id="16aaf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16aaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16aaf-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16aaf-111">Permission type</span></span>|<span data-ttu-id="16aaf-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16aaf-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16aaf-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16aaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16aaf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16aaf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16aaf-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16aaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16aaf-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16aaf-116">Not supported.</span></span>|
|<span data-ttu-id="16aaf-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="16aaf-117">Application</span></span>|<span data-ttu-id="16aaf-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16aaf-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16aaf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16aaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
```

## <a name="request-headers"></a><span data-ttu-id="16aaf-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16aaf-120">Request headers</span></span>
|<span data-ttu-id="16aaf-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16aaf-121">Header</span></span>|<span data-ttu-id="16aaf-122">Значение</span><span class="sxs-lookup"><span data-stu-id="16aaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16aaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16aaf-123">Authorization</span></span>|<span data-ttu-id="16aaf-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16aaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16aaf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16aaf-125">Accept</span></span>|<span data-ttu-id="16aaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16aaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16aaf-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16aaf-127">Request body</span></span>
<span data-ttu-id="16aaf-128">В теле запроса предоставляем представление JSON для [объекта windows10XVpnConfiguration.](../resources/intune-rapolicy-windows10xvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-128">In the request body, supply a JSON representation for the [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object.</span></span>

<span data-ttu-id="16aaf-129">В следующей таблице показаны свойства, необходимые при создании [windows10XVpnConfiguration.](../resources/intune-rapolicy-windows10xvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-129">The following table shows the properties that are required when you create the [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md).</span></span>

|<span data-ttu-id="16aaf-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="16aaf-130">Property</span></span>|<span data-ttu-id="16aaf-131">Тип</span><span class="sxs-lookup"><span data-stu-id="16aaf-131">Type</span></span>|<span data-ttu-id="16aaf-132">Описание</span><span class="sxs-lookup"><span data-stu-id="16aaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16aaf-133">id</span><span class="sxs-lookup"><span data-stu-id="16aaf-133">id</span></span>|<span data-ttu-id="16aaf-134">Строка</span><span class="sxs-lookup"><span data-stu-id="16aaf-134">String</span></span>|<span data-ttu-id="16aaf-135">Идентификатор профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="16aaf-136">version</span><span class="sxs-lookup"><span data-stu-id="16aaf-136">version</span></span>|<span data-ttu-id="16aaf-137">Int32</span><span class="sxs-lookup"><span data-stu-id="16aaf-137">Int32</span></span>|<span data-ttu-id="16aaf-138">Версия профиля, унаследованной от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="16aaf-139">displayName</span><span class="sxs-lookup"><span data-stu-id="16aaf-139">displayName</span></span>|<span data-ttu-id="16aaf-140">Строка</span><span class="sxs-lookup"><span data-stu-id="16aaf-140">String</span></span>|<span data-ttu-id="16aaf-141">Имя отображения профиля, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="16aaf-142">description</span><span class="sxs-lookup"><span data-stu-id="16aaf-142">description</span></span>|<span data-ttu-id="16aaf-143">Строка</span><span class="sxs-lookup"><span data-stu-id="16aaf-143">String</span></span>|<span data-ttu-id="16aaf-144">Описание профиля, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="16aaf-145">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="16aaf-145">creationDateTime</span></span>|<span data-ttu-id="16aaf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16aaf-146">DateTimeOffset</span></span>|<span data-ttu-id="16aaf-147">Профиль DateTime был создан по наследству от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="16aaf-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16aaf-148">lastModifiedDateTime</span></span>|<span data-ttu-id="16aaf-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16aaf-149">DateTimeOffset</span></span>|<span data-ttu-id="16aaf-150">Последний раз был изменен профиль DateTime, унаследованный от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="16aaf-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16aaf-151">roleScopeTagIds</span></span>|<span data-ttu-id="16aaf-152">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="16aaf-152">String collection</span></span>|<span data-ttu-id="16aaf-153">Теги области, унаследованные от [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="16aaf-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="16aaf-154">authenticationCertificateId</span><span class="sxs-lookup"><span data-stu-id="16aaf-154">authenticationCertificateId</span></span>|<span data-ttu-id="16aaf-155">Guid</span><span class="sxs-lookup"><span data-stu-id="16aaf-155">Guid</span></span>|<span data-ttu-id="16aaf-156">ID к сертификату проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="16aaf-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="16aaf-157">customXmlFileName</span><span class="sxs-lookup"><span data-stu-id="16aaf-157">customXmlFileName</span></span>|<span data-ttu-id="16aaf-158">Строка</span><span class="sxs-lookup"><span data-stu-id="16aaf-158">String</span></span>|<span data-ttu-id="16aaf-159">Пользовательское имя файла Xml.</span><span class="sxs-lookup"><span data-stu-id="16aaf-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="16aaf-160">customXml</span><span class="sxs-lookup"><span data-stu-id="16aaf-160">customXml</span></span>|<span data-ttu-id="16aaf-161">Binary</span><span class="sxs-lookup"><span data-stu-id="16aaf-161">Binary</span></span>|<span data-ttu-id="16aaf-162">Настраиваемые XML-команды, настраиваемые vpn-подключением.</span><span class="sxs-lookup"><span data-stu-id="16aaf-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="16aaf-163">(кодификат byte UTF8)</span><span class="sxs-lookup"><span data-stu-id="16aaf-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="16aaf-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="16aaf-164">Response</span></span>
<span data-ttu-id="16aaf-165">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="16aaf-165">If successful, this method returns a `200 OK` response code and an updated [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16aaf-166">Пример</span><span class="sxs-lookup"><span data-stu-id="16aaf-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="16aaf-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="16aaf-167">Request</span></span>
<span data-ttu-id="16aaf-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16aaf-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/{deviceManagementResourceAccessProfileBaseId}
Content-type: application/json
Content-length: 446

{
  "@odata.type": "#microsoft.graph.windows10XVpnConfiguration",
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

### <a name="response"></a><span data-ttu-id="16aaf-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="16aaf-169">Response</span></span>
<span data-ttu-id="16aaf-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16aaf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 559

{
  "@odata.type": "#microsoft.graph.windows10XVpnConfiguration",
  "id": "6ee1c04f-c04f-6ee1-4fc0-e16e4fc0e16e",
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




