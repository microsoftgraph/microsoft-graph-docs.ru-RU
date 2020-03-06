---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d6ae46c5018fbcf52a9b604ba105a76fd5a8f15
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42512862"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="666f1-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="666f1-103">Create windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="666f1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="666f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="666f1-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="666f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="666f1-106">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="666f1-106">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="666f1-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="666f1-107">Prerequisites</span></span>
<span data-ttu-id="666f1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="666f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="666f1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="666f1-110">Permission type</span></span>|<span data-ttu-id="666f1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="666f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="666f1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="666f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="666f1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="666f1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="666f1-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="666f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="666f1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="666f1-115">Not supported.</span></span>|
|<span data-ttu-id="666f1-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="666f1-116">Application</span></span>|<span data-ttu-id="666f1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="666f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="666f1-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="666f1-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="666f1-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="666f1-119">Request headers</span></span>
|<span data-ttu-id="666f1-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="666f1-120">Header</span></span>|<span data-ttu-id="666f1-121">Значение</span><span class="sxs-lookup"><span data-stu-id="666f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="666f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="666f1-122">Authorization</span></span>|<span data-ttu-id="666f1-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="666f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="666f1-124">Accept</span><span class="sxs-lookup"><span data-stu-id="666f1-124">Accept</span></span>|<span data-ttu-id="666f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="666f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="666f1-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="666f1-126">Request body</span></span>
<span data-ttu-id="666f1-127">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="666f1-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="666f1-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="666f1-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="666f1-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="666f1-129">Property</span></span>|<span data-ttu-id="666f1-130">Тип</span><span class="sxs-lookup"><span data-stu-id="666f1-130">Type</span></span>|<span data-ttu-id="666f1-131">Описание</span><span class="sxs-lookup"><span data-stu-id="666f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="666f1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="666f1-132">displayName</span></span>|<span data-ttu-id="666f1-133">Строка</span><span class="sxs-lookup"><span data-stu-id="666f1-133">String</span></span>|<span data-ttu-id="666f1-134">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="666f1-134">The friendly name</span></span>|
|<span data-ttu-id="666f1-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="666f1-135">fileHash</span></span>|<span data-ttu-id="666f1-136">String</span><span class="sxs-lookup"><span data-stu-id="666f1-136">String</span></span>|<span data-ttu-id="666f1-137">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="666f1-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="666f1-138">file</span><span class="sxs-lookup"><span data-stu-id="666f1-138">file</span></span>|<span data-ttu-id="666f1-139">Binary</span><span class="sxs-lookup"><span data-stu-id="666f1-139">Binary</span></span>|<span data-ttu-id="666f1-140">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="666f1-140">File as a byte array</span></span>|
|<span data-ttu-id="666f1-141">id</span><span class="sxs-lookup"><span data-stu-id="666f1-141">id</span></span>|<span data-ttu-id="666f1-142">String</span><span class="sxs-lookup"><span data-stu-id="666f1-142">String</span></span>|<span data-ttu-id="666f1-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="666f1-143">Key of the entity.</span></span>|
|<span data-ttu-id="666f1-144">version</span><span class="sxs-lookup"><span data-stu-id="666f1-144">version</span></span>|<span data-ttu-id="666f1-145">Строка</span><span class="sxs-lookup"><span data-stu-id="666f1-145">String</span></span>|<span data-ttu-id="666f1-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="666f1-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="666f1-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="666f1-147">Response</span></span>
<span data-ttu-id="666f1-148">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="666f1-148">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="666f1-149">Пример</span><span class="sxs-lookup"><span data-stu-id="666f1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="666f1-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="666f1-150">Request</span></span>
<span data-ttu-id="666f1-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="666f1-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
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

### <a name="response"></a><span data-ttu-id="666f1-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="666f1-152">Response</span></span>
<span data-ttu-id="666f1-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="666f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




