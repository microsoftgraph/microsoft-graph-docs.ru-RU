---
title: Обновление объекта windowsInformationProtectionAppLockerFile
description: Обновление свойств объекта windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ae8932a6594ed396eecec28863ec80d5b8ed652
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465519"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="6cbb1-103">Обновление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="6cbb1-103">Update windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="6cbb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cbb1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cbb1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cbb1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cbb1-107">Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="6cbb1-107">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6cbb1-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6cbb1-108">Prerequisites</span></span>
<span data-ttu-id="6cbb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cbb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cbb1-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6cbb1-111">Permission type</span></span>|<span data-ttu-id="6cbb1-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6cbb1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6cbb1-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6cbb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6cbb1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cbb1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6cbb1-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6cbb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6cbb1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-116">Not supported.</span></span>|
|<span data-ttu-id="6cbb1-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6cbb1-117">Application</span></span>|<span data-ttu-id="6cbb1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6cbb1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6cbb1-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6cbb1-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="6cbb1-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="6cbb1-120">Request headers</span></span>
|<span data-ttu-id="6cbb1-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6cbb1-121">Header</span></span>|<span data-ttu-id="6cbb1-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6cbb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6cbb1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cbb1-123">Authorization</span></span>|<span data-ttu-id="6cbb1-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6cbb1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6cbb1-125">Accept</span></span>|<span data-ttu-id="6cbb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6cbb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6cbb1-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6cbb1-127">Request body</span></span>
<span data-ttu-id="6cbb1-128">В теле запроса добавьте представление объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="6cbb1-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="6cbb1-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="6cbb1-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6cbb1-130">Property</span></span>|<span data-ttu-id="6cbb1-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6cbb1-131">Type</span></span>|<span data-ttu-id="6cbb1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6cbb1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cbb1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="6cbb1-133">displayName</span></span>|<span data-ttu-id="6cbb1-134">Строка</span><span class="sxs-lookup"><span data-stu-id="6cbb1-134">String</span></span>|<span data-ttu-id="6cbb1-135">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="6cbb1-135">The friendly name</span></span>|
|<span data-ttu-id="6cbb1-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="6cbb1-136">fileHash</span></span>|<span data-ttu-id="6cbb1-137">String</span><span class="sxs-lookup"><span data-stu-id="6cbb1-137">String</span></span>|<span data-ttu-id="6cbb1-138">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="6cbb1-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="6cbb1-139">file</span><span class="sxs-lookup"><span data-stu-id="6cbb1-139">file</span></span>|<span data-ttu-id="6cbb1-140">Binary</span><span class="sxs-lookup"><span data-stu-id="6cbb1-140">Binary</span></span>|<span data-ttu-id="6cbb1-141">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="6cbb1-141">File as a byte array</span></span>|
|<span data-ttu-id="6cbb1-142">id</span><span class="sxs-lookup"><span data-stu-id="6cbb1-142">id</span></span>|<span data-ttu-id="6cbb1-143">String</span><span class="sxs-lookup"><span data-stu-id="6cbb1-143">String</span></span>|<span data-ttu-id="6cbb1-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-144">Key of the entity.</span></span>|
|<span data-ttu-id="6cbb1-145">version</span><span class="sxs-lookup"><span data-stu-id="6cbb1-145">version</span></span>|<span data-ttu-id="6cbb1-146">Строка</span><span class="sxs-lookup"><span data-stu-id="6cbb1-146">String</span></span>|<span data-ttu-id="6cbb1-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="6cbb1-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cbb1-148">Response</span></span>
<span data-ttu-id="6cbb1-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-149">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cbb1-150">Пример</span><span class="sxs-lookup"><span data-stu-id="6cbb1-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="6cbb1-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="6cbb1-151">Request</span></span>
<span data-ttu-id="6cbb1-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
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

### <a name="response"></a><span data-ttu-id="6cbb1-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="6cbb1-153">Response</span></span>
<span data-ttu-id="6cbb1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6cbb1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



