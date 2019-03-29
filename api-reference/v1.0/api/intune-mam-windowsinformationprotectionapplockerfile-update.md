---
title: Обновление объекта windowsInformationProtectionAppLockerFile
description: Обновление свойств объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97afdcc7a7d0f0025b19ed33e9df2e10e9b275fa
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979601"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="53905-103">Обновление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="53905-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="53905-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="53905-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53905-105">Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="53905-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53905-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="53905-106">Prerequisites</span></span>
<span data-ttu-id="53905-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53905-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53905-109">Permission type</span></span>|<span data-ttu-id="53905-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="53905-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53905-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53905-111">Delegated (work or school account)</span></span>|<span data-ttu-id="53905-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53905-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53905-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53905-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53905-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53905-114">Not supported.</span></span>|
|<span data-ttu-id="53905-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53905-115">Application</span></span>|<span data-ttu-id="53905-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53905-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53905-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53905-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="53905-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53905-118">Request headers</span></span>
|<span data-ttu-id="53905-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53905-119">Header</span></span>|<span data-ttu-id="53905-120">Значение</span><span class="sxs-lookup"><span data-stu-id="53905-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53905-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53905-121">Authorization</span></span>|<span data-ttu-id="53905-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53905-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53905-123">Accept</span><span class="sxs-lookup"><span data-stu-id="53905-123">Accept</span></span>|<span data-ttu-id="53905-124">application/json</span><span class="sxs-lookup"><span data-stu-id="53905-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53905-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53905-125">Request body</span></span>
<span data-ttu-id="53905-126">В теле запроса добавьте представление объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="53905-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="53905-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="53905-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="53905-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="53905-128">Property</span></span>|<span data-ttu-id="53905-129">Тип</span><span class="sxs-lookup"><span data-stu-id="53905-129">Type</span></span>|<span data-ttu-id="53905-130">Описание</span><span class="sxs-lookup"><span data-stu-id="53905-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53905-131">displayName</span><span class="sxs-lookup"><span data-stu-id="53905-131">displayName</span></span>|<span data-ttu-id="53905-132">String</span><span class="sxs-lookup"><span data-stu-id="53905-132">String</span></span>|<span data-ttu-id="53905-133">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="53905-133">The friendly name</span></span>|
|<span data-ttu-id="53905-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="53905-134">fileHash</span></span>|<span data-ttu-id="53905-135">String</span><span class="sxs-lookup"><span data-stu-id="53905-135">String</span></span>|<span data-ttu-id="53905-136">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="53905-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="53905-137">file</span><span class="sxs-lookup"><span data-stu-id="53905-137">file</span></span>|<span data-ttu-id="53905-138">Binary</span><span class="sxs-lookup"><span data-stu-id="53905-138">Binary</span></span>|<span data-ttu-id="53905-139">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="53905-139">File as a byte array</span></span>|
|<span data-ttu-id="53905-140">id</span><span class="sxs-lookup"><span data-stu-id="53905-140">id</span></span>|<span data-ttu-id="53905-141">String</span><span class="sxs-lookup"><span data-stu-id="53905-141">String</span></span>|<span data-ttu-id="53905-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="53905-142">Key of the entity.</span></span>|
|<span data-ttu-id="53905-143">version</span><span class="sxs-lookup"><span data-stu-id="53905-143">version</span></span>|<span data-ttu-id="53905-144">Строка</span><span class="sxs-lookup"><span data-stu-id="53905-144">String</span></span>|<span data-ttu-id="53905-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="53905-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="53905-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="53905-146">Response</span></span>
<span data-ttu-id="53905-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53905-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53905-148">Пример</span><span class="sxs-lookup"><span data-stu-id="53905-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="53905-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="53905-149">Request</span></span>
<span data-ttu-id="53905-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53905-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53905-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="53905-151">Response</span></span>
<span data-ttu-id="53905-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="53905-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



