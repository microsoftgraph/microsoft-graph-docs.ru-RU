---
title: Обновление объекта windowsInformationProtectionAppLockerFile
description: Обновление свойств объекта windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: cf6df3ff89702d3ab78a5ccad1575bbfbdd4b90a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43450079"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="4c86c-103">Обновление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="4c86c-103">Update windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="4c86c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c86c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c86c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c86c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c86c-106">Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="4c86c-106">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c86c-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c86c-107">Prerequisites</span></span>
<span data-ttu-id="4c86c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c86c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c86c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c86c-110">Permission type</span></span>|<span data-ttu-id="4c86c-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c86c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c86c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c86c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c86c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c86c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c86c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c86c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c86c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c86c-115">Not supported.</span></span>|
|<span data-ttu-id="4c86c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c86c-116">Application</span></span>|<span data-ttu-id="4c86c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c86c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c86c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c86c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="4c86c-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4c86c-119">Request headers</span></span>
|<span data-ttu-id="4c86c-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c86c-120">Header</span></span>|<span data-ttu-id="4c86c-121">Значение</span><span class="sxs-lookup"><span data-stu-id="4c86c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c86c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c86c-122">Authorization</span></span>|<span data-ttu-id="4c86c-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4c86c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c86c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4c86c-124">Accept</span></span>|<span data-ttu-id="4c86c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c86c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c86c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="4c86c-126">Request body</span></span>
<span data-ttu-id="4c86c-127">В теле запроса добавьте представление объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c86c-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="4c86c-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="4c86c-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="4c86c-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c86c-129">Property</span></span>|<span data-ttu-id="4c86c-130">Тип</span><span class="sxs-lookup"><span data-stu-id="4c86c-130">Type</span></span>|<span data-ttu-id="4c86c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="4c86c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c86c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4c86c-132">displayName</span></span>|<span data-ttu-id="4c86c-133">Строка</span><span class="sxs-lookup"><span data-stu-id="4c86c-133">String</span></span>|<span data-ttu-id="4c86c-134">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="4c86c-134">The friendly name</span></span>|
|<span data-ttu-id="4c86c-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="4c86c-135">fileHash</span></span>|<span data-ttu-id="4c86c-136">String</span><span class="sxs-lookup"><span data-stu-id="4c86c-136">String</span></span>|<span data-ttu-id="4c86c-137">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="4c86c-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="4c86c-138">file</span><span class="sxs-lookup"><span data-stu-id="4c86c-138">file</span></span>|<span data-ttu-id="4c86c-139">Binary</span><span class="sxs-lookup"><span data-stu-id="4c86c-139">Binary</span></span>|<span data-ttu-id="4c86c-140">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="4c86c-140">File as a byte array</span></span>|
|<span data-ttu-id="4c86c-141">id</span><span class="sxs-lookup"><span data-stu-id="4c86c-141">id</span></span>|<span data-ttu-id="4c86c-142">String</span><span class="sxs-lookup"><span data-stu-id="4c86c-142">String</span></span>|<span data-ttu-id="4c86c-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4c86c-143">Key of the entity.</span></span>|
|<span data-ttu-id="4c86c-144">version</span><span class="sxs-lookup"><span data-stu-id="4c86c-144">version</span></span>|<span data-ttu-id="4c86c-145">Строка</span><span class="sxs-lookup"><span data-stu-id="4c86c-145">String</span></span>|<span data-ttu-id="4c86c-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="4c86c-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="4c86c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c86c-147">Response</span></span>
<span data-ttu-id="4c86c-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4c86c-148">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c86c-149">Пример</span><span class="sxs-lookup"><span data-stu-id="4c86c-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c86c-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c86c-150">Request</span></span>
<span data-ttu-id="4c86c-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c86c-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="4c86c-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c86c-152">Response</span></span>
<span data-ttu-id="4c86c-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="4c86c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```






