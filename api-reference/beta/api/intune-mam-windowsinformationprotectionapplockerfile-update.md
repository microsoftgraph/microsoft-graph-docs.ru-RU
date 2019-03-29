---
title: Обновление объекта windowsInformationProtectionAppLockerFile
description: Обновление свойств объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc465df11d9f0299f1074094f78058b48bc1df3a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971411"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="46257-103">Обновление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="46257-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="46257-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46257-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46257-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46257-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46257-106">Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="46257-106">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46257-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="46257-107">Prerequisites</span></span>
<span data-ttu-id="46257-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46257-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46257-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46257-110">Permission type</span></span>|<span data-ttu-id="46257-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46257-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46257-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46257-112">Delegated (work or school account)</span></span>|<span data-ttu-id="46257-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46257-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46257-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46257-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46257-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46257-115">Not supported.</span></span>|
|<span data-ttu-id="46257-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46257-116">Application</span></span>|<span data-ttu-id="46257-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46257-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46257-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46257-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="46257-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46257-119">Request headers</span></span>
|<span data-ttu-id="46257-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46257-120">Header</span></span>|<span data-ttu-id="46257-121">Значение</span><span class="sxs-lookup"><span data-stu-id="46257-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46257-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46257-122">Authorization</span></span>|<span data-ttu-id="46257-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46257-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46257-124">Accept</span><span class="sxs-lookup"><span data-stu-id="46257-124">Accept</span></span>|<span data-ttu-id="46257-125">application/json</span><span class="sxs-lookup"><span data-stu-id="46257-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46257-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46257-126">Request body</span></span>
<span data-ttu-id="46257-127">В теле запроса добавьте представление объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46257-127">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="46257-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="46257-128">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="46257-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="46257-129">Property</span></span>|<span data-ttu-id="46257-130">Тип</span><span class="sxs-lookup"><span data-stu-id="46257-130">Type</span></span>|<span data-ttu-id="46257-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46257-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46257-132">displayName</span><span class="sxs-lookup"><span data-stu-id="46257-132">displayName</span></span>|<span data-ttu-id="46257-133">String</span><span class="sxs-lookup"><span data-stu-id="46257-133">String</span></span>|<span data-ttu-id="46257-134">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="46257-134">The friendly name</span></span>|
|<span data-ttu-id="46257-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="46257-135">fileHash</span></span>|<span data-ttu-id="46257-136">String</span><span class="sxs-lookup"><span data-stu-id="46257-136">String</span></span>|<span data-ttu-id="46257-137">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="46257-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="46257-138">file</span><span class="sxs-lookup"><span data-stu-id="46257-138">file</span></span>|<span data-ttu-id="46257-139">Binary</span><span class="sxs-lookup"><span data-stu-id="46257-139">Binary</span></span>|<span data-ttu-id="46257-140">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="46257-140">File as a byte array</span></span>|
|<span data-ttu-id="46257-141">id</span><span class="sxs-lookup"><span data-stu-id="46257-141">id</span></span>|<span data-ttu-id="46257-142">String</span><span class="sxs-lookup"><span data-stu-id="46257-142">String</span></span>|<span data-ttu-id="46257-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="46257-143">Key of the entity.</span></span>|
|<span data-ttu-id="46257-144">version</span><span class="sxs-lookup"><span data-stu-id="46257-144">version</span></span>|<span data-ttu-id="46257-145">Строка</span><span class="sxs-lookup"><span data-stu-id="46257-145">String</span></span>|<span data-ttu-id="46257-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="46257-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="46257-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="46257-147">Response</span></span>
<span data-ttu-id="46257-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="46257-148">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46257-149">Пример</span><span class="sxs-lookup"><span data-stu-id="46257-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="46257-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="46257-150">Request</span></span>
<span data-ttu-id="46257-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46257-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="46257-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="46257-152">Response</span></span>
<span data-ttu-id="46257-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46257-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




