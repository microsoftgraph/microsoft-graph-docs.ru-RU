---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d22e4be6d282ba7750b6c896b2592ea8b0b71a62
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453569"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="5b5d6-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="5b5d6-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="5b5d6-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b5d6-105">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5b5d6-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b5d6-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5b5d6-106">Prerequisites</span></span>
<span data-ttu-id="5b5d6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b5d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b5d6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5b5d6-109">Permission type</span></span>|<span data-ttu-id="5b5d6-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5b5d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b5d6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5b5d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b5d6-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b5d6-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5b5d6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5b5d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b5d6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-114">Not supported.</span></span>|
|<span data-ttu-id="5b5d6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5b5d6-115">Application</span></span>|<span data-ttu-id="5b5d6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b5d6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5b5d6-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5b5d6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5b5d6-118">Request headers</span></span>
|<span data-ttu-id="5b5d6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5b5d6-119">Header</span></span>|<span data-ttu-id="5b5d6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="5b5d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b5d6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5b5d6-121">Authorization</span></span>|<span data-ttu-id="5b5d6-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b5d6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5b5d6-123">Accept</span></span>|<span data-ttu-id="5b5d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5b5d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b5d6-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5b5d6-125">Request body</span></span>
<span data-ttu-id="5b5d6-126">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="5b5d6-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="5b5d6-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b5d6-128">Property</span></span>|<span data-ttu-id="5b5d6-129">Тип</span><span class="sxs-lookup"><span data-stu-id="5b5d6-129">Type</span></span>|<span data-ttu-id="5b5d6-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5b5d6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b5d6-131">displayName</span><span class="sxs-lookup"><span data-stu-id="5b5d6-131">displayName</span></span>|<span data-ttu-id="5b5d6-132">Строка</span><span class="sxs-lookup"><span data-stu-id="5b5d6-132">String</span></span>|<span data-ttu-id="5b5d6-133">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="5b5d6-133">The friendly name</span></span>|
|<span data-ttu-id="5b5d6-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="5b5d6-134">fileHash</span></span>|<span data-ttu-id="5b5d6-135">String</span><span class="sxs-lookup"><span data-stu-id="5b5d6-135">String</span></span>|<span data-ttu-id="5b5d6-136">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="5b5d6-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="5b5d6-137">file</span><span class="sxs-lookup"><span data-stu-id="5b5d6-137">file</span></span>|<span data-ttu-id="5b5d6-138">Binary</span><span class="sxs-lookup"><span data-stu-id="5b5d6-138">Binary</span></span>|<span data-ttu-id="5b5d6-139">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="5b5d6-139">File as a byte array</span></span>|
|<span data-ttu-id="5b5d6-140">id</span><span class="sxs-lookup"><span data-stu-id="5b5d6-140">id</span></span>|<span data-ttu-id="5b5d6-141">Строка</span><span class="sxs-lookup"><span data-stu-id="5b5d6-141">String</span></span>|<span data-ttu-id="5b5d6-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-142">Key of the entity.</span></span>|
|<span data-ttu-id="5b5d6-143">version</span><span class="sxs-lookup"><span data-stu-id="5b5d6-143">version</span></span>|<span data-ttu-id="5b5d6-144">Строка</span><span class="sxs-lookup"><span data-stu-id="5b5d6-144">String</span></span>|<span data-ttu-id="5b5d6-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5b5d6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b5d6-146">Response</span></span>
<span data-ttu-id="5b5d6-147">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b5d6-148">Пример</span><span class="sxs-lookup"><span data-stu-id="5b5d6-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b5d6-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="5b5d6-149">Request</span></span>
<span data-ttu-id="5b5d6-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b5d6-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="5b5d6-151">Response</span></span>
<span data-ttu-id="5b5d6-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5b5d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



