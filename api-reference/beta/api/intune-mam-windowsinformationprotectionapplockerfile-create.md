---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 576e6a284c65cfe9e21aae1f33ce7ed50e56183e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51148878"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="bd1c9-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="bd1c9-103">Create windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="bd1c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd1c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd1c9-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd1c9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd1c9-107">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="bd1c9-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd1c9-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bd1c9-108">Prerequisites</span></span>
<span data-ttu-id="bd1c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd1c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd1c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bd1c9-111">Permission type</span></span>|<span data-ttu-id="bd1c9-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bd1c9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd1c9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bd1c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd1c9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd1c9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd1c9-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bd1c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd1c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-116">Not supported.</span></span>|
|<span data-ttu-id="bd1c9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="bd1c9-117">Application</span></span>|<span data-ttu-id="bd1c9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd1c9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd1c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bd1c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="bd1c9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="bd1c9-120">Request headers</span></span>
|<span data-ttu-id="bd1c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bd1c9-121">Header</span></span>|<span data-ttu-id="bd1c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="bd1c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd1c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd1c9-123">Authorization</span></span>|<span data-ttu-id="bd1c9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd1c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bd1c9-125">Accept</span></span>|<span data-ttu-id="bd1c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd1c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd1c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bd1c9-127">Request body</span></span>
<span data-ttu-id="bd1c9-128">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="bd1c9-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="bd1c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd1c9-130">Property</span></span>|<span data-ttu-id="bd1c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="bd1c9-131">Type</span></span>|<span data-ttu-id="bd1c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="bd1c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd1c9-133">displayName</span><span class="sxs-lookup"><span data-stu-id="bd1c9-133">displayName</span></span>|<span data-ttu-id="bd1c9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="bd1c9-134">String</span></span>|<span data-ttu-id="bd1c9-135">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="bd1c9-135">The friendly name</span></span>|
|<span data-ttu-id="bd1c9-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="bd1c9-136">fileHash</span></span>|<span data-ttu-id="bd1c9-137">String</span><span class="sxs-lookup"><span data-stu-id="bd1c9-137">String</span></span>|<span data-ttu-id="bd1c9-138">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="bd1c9-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="bd1c9-139">file</span><span class="sxs-lookup"><span data-stu-id="bd1c9-139">file</span></span>|<span data-ttu-id="bd1c9-140">Binary</span><span class="sxs-lookup"><span data-stu-id="bd1c9-140">Binary</span></span>|<span data-ttu-id="bd1c9-141">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="bd1c9-141">File as a byte array</span></span>|
|<span data-ttu-id="bd1c9-142">id</span><span class="sxs-lookup"><span data-stu-id="bd1c9-142">id</span></span>|<span data-ttu-id="bd1c9-143">Строка</span><span class="sxs-lookup"><span data-stu-id="bd1c9-143">String</span></span>|<span data-ttu-id="bd1c9-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-144">Key of the entity.</span></span>|
|<span data-ttu-id="bd1c9-145">version</span><span class="sxs-lookup"><span data-stu-id="bd1c9-145">version</span></span>|<span data-ttu-id="bd1c9-146">String</span><span class="sxs-lookup"><span data-stu-id="bd1c9-146">String</span></span>|<span data-ttu-id="bd1c9-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="bd1c9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd1c9-148">Response</span></span>
<span data-ttu-id="bd1c9-149">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd1c9-150">Пример</span><span class="sxs-lookup"><span data-stu-id="bd1c9-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd1c9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="bd1c9-151">Request</span></span>
<span data-ttu-id="bd1c9-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
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

### <a name="response"></a><span data-ttu-id="bd1c9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="bd1c9-153">Response</span></span>
<span data-ttu-id="bd1c9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bd1c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




