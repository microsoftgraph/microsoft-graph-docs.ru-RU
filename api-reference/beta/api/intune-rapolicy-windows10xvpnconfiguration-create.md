---
title: Создание windows10XVpnConfiguration
description: Создание нового объекта windows10XVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c30a7a18bf159891ed3331fa8722404823116b29
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242372"
---
# <a name="create-windows10xvpnconfiguration"></a><span data-ttu-id="00038-103">Создание windows10XVpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="00038-103">Create windows10XVpnConfiguration</span></span>

<span data-ttu-id="00038-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00038-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00038-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00038-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00038-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00038-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00038-107">Создание нового объекта [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="00038-107">Create a new [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00038-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="00038-108">Prerequisites</span></span>
<span data-ttu-id="00038-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00038-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00038-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00038-111">Permission type</span></span>|<span data-ttu-id="00038-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="00038-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00038-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00038-113">Delegated (work or school account)</span></span>|<span data-ttu-id="00038-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00038-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="00038-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00038-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00038-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00038-116">Not supported.</span></span>|
|<span data-ttu-id="00038-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="00038-117">Application</span></span>|<span data-ttu-id="00038-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00038-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00038-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00038-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="00038-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="00038-120">Request headers</span></span>
|<span data-ttu-id="00038-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="00038-121">Header</span></span>|<span data-ttu-id="00038-122">Значение</span><span class="sxs-lookup"><span data-stu-id="00038-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00038-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00038-123">Authorization</span></span>|<span data-ttu-id="00038-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00038-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00038-125">Accept</span><span class="sxs-lookup"><span data-stu-id="00038-125">Accept</span></span>|<span data-ttu-id="00038-126">application/json</span><span class="sxs-lookup"><span data-stu-id="00038-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00038-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00038-127">Request body</span></span>
<span data-ttu-id="00038-128">В тексте запроса добавьте представление объекта windows10XVpnConfiguration в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00038-128">In the request body, supply a JSON representation for the windows10XVpnConfiguration object.</span></span>

<span data-ttu-id="00038-129">В следующей таблице приведены свойства, необходимые при создании windows10XVpnConfiguration.</span><span class="sxs-lookup"><span data-stu-id="00038-129">The following table shows the properties that are required when you create the windows10XVpnConfiguration.</span></span>

|<span data-ttu-id="00038-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="00038-130">Property</span></span>|<span data-ttu-id="00038-131">Тип</span><span class="sxs-lookup"><span data-stu-id="00038-131">Type</span></span>|<span data-ttu-id="00038-132">Описание</span><span class="sxs-lookup"><span data-stu-id="00038-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00038-133">id</span><span class="sxs-lookup"><span data-stu-id="00038-133">id</span></span>|<span data-ttu-id="00038-134">String</span><span class="sxs-lookup"><span data-stu-id="00038-134">String</span></span>|<span data-ttu-id="00038-135">Идентификатор профиля унаследован от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="00038-135">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="00038-136">version</span><span class="sxs-lookup"><span data-stu-id="00038-136">version</span></span>|<span data-ttu-id="00038-137">Int32</span><span class="sxs-lookup"><span data-stu-id="00038-137">Int32</span></span>|<span data-ttu-id="00038-138">Версия профиля, унаследованного от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="00038-138">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="00038-139">displayName</span><span class="sxs-lookup"><span data-stu-id="00038-139">displayName</span></span>|<span data-ttu-id="00038-140">String</span><span class="sxs-lookup"><span data-stu-id="00038-140">String</span></span>|<span data-ttu-id="00038-141">Отображаемое имя профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="00038-141">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="00038-142">description</span><span class="sxs-lookup"><span data-stu-id="00038-142">description</span></span>|<span data-ttu-id="00038-143">String</span><span class="sxs-lookup"><span data-stu-id="00038-143">String</span></span>|<span data-ttu-id="00038-144">Описание профиля, унаследованное от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="00038-144">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="00038-145">креатиондатетиме</span><span class="sxs-lookup"><span data-stu-id="00038-145">creationDateTime</span></span>|<span data-ttu-id="00038-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00038-146">DateTimeOffset</span></span>|<span data-ttu-id="00038-147">Создан профиль DateTime, наследуемый от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="00038-147">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="00038-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00038-148">lastModifiedDateTime</span></span>|<span data-ttu-id="00038-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00038-149">DateTimeOffset</span></span>|<span data-ttu-id="00038-150">Последнее изменение профиля DateTime унаследовано от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="00038-150">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="00038-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="00038-151">roleScopeTagIds</span></span>|<span data-ttu-id="00038-152">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="00038-152">String collection</span></span>|<span data-ttu-id="00038-153">Теги областей унаследованы от [девицеманажементресаурцеакцесспрофилебасе](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="00038-153">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="00038-154">аусентикатионцертификатеид</span><span class="sxs-lookup"><span data-stu-id="00038-154">authenticationCertificateId</span></span>|<span data-ttu-id="00038-155">Guid</span><span class="sxs-lookup"><span data-stu-id="00038-155">Guid</span></span>|<span data-ttu-id="00038-156">Идентификатор сертификата проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="00038-156">ID to the Authentication Certificate</span></span>|
|<span data-ttu-id="00038-157">кустомксмлфиленаме</span><span class="sxs-lookup"><span data-stu-id="00038-157">customXmlFileName</span></span>|<span data-ttu-id="00038-158">String</span><span class="sxs-lookup"><span data-stu-id="00038-158">String</span></span>|<span data-ttu-id="00038-159">Имя настраиваемого XML-файла.</span><span class="sxs-lookup"><span data-stu-id="00038-159">Custom Xml file name.</span></span>|
|<span data-ttu-id="00038-160">customXml</span><span class="sxs-lookup"><span data-stu-id="00038-160">customXml</span></span>|<span data-ttu-id="00038-161">Binary</span><span class="sxs-lookup"><span data-stu-id="00038-161">Binary</span></span>|<span data-ttu-id="00038-162">Настраиваемые XML-команды, которые настраивают VPN-подключение.</span><span class="sxs-lookup"><span data-stu-id="00038-162">Custom XML commands that configures the VPN connection.</span></span> <span data-ttu-id="00038-163">(Кодирование байтов в кодировке UTF8)</span><span class="sxs-lookup"><span data-stu-id="00038-163">(UTF8 byte encoding)</span></span>|



## <a name="response"></a><span data-ttu-id="00038-164">Отклик</span><span class="sxs-lookup"><span data-stu-id="00038-164">Response</span></span>
<span data-ttu-id="00038-165">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="00038-165">If successful, this method returns a `201 Created` response code and a [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00038-166">Пример</span><span class="sxs-lookup"><span data-stu-id="00038-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="00038-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="00038-167">Request</span></span>
<span data-ttu-id="00038-168">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00038-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
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

### <a name="response"></a><span data-ttu-id="00038-169">Отклик</span><span class="sxs-lookup"><span data-stu-id="00038-169">Response</span></span>
<span data-ttu-id="00038-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="00038-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




