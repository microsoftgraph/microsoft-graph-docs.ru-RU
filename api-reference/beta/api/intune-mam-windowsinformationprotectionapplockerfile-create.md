---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea89fc5a17a20b8cf47594d5029f03b59ea70db4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776159"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="66fcc-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="66fcc-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="66fcc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66fcc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66fcc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="66fcc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66fcc-106">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="66fcc-106">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66fcc-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="66fcc-107">Prerequisites</span></span>
<span data-ttu-id="66fcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66fcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66fcc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="66fcc-110">Permission type</span></span>|<span data-ttu-id="66fcc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="66fcc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66fcc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="66fcc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66fcc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66fcc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66fcc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="66fcc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66fcc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66fcc-115">Not supported.</span></span>|
|<span data-ttu-id="66fcc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="66fcc-116">Application</span></span>|<span data-ttu-id="66fcc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="66fcc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66fcc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="66fcc-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="66fcc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="66fcc-119">Request headers</span></span>
|<span data-ttu-id="66fcc-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="66fcc-120">Header</span></span>|<span data-ttu-id="66fcc-121">Значение</span><span class="sxs-lookup"><span data-stu-id="66fcc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66fcc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="66fcc-122">Authorization</span></span>|<span data-ttu-id="66fcc-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="66fcc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66fcc-124">Accept</span><span class="sxs-lookup"><span data-stu-id="66fcc-124">Accept</span></span>|<span data-ttu-id="66fcc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66fcc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66fcc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="66fcc-126">Request body</span></span>
<span data-ttu-id="66fcc-127">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66fcc-127">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="66fcc-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="66fcc-128">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="66fcc-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="66fcc-129">Property</span></span>|<span data-ttu-id="66fcc-130">Тип</span><span class="sxs-lookup"><span data-stu-id="66fcc-130">Type</span></span>|<span data-ttu-id="66fcc-131">Описание</span><span class="sxs-lookup"><span data-stu-id="66fcc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66fcc-132">displayName</span><span class="sxs-lookup"><span data-stu-id="66fcc-132">displayName</span></span>|<span data-ttu-id="66fcc-133">String</span><span class="sxs-lookup"><span data-stu-id="66fcc-133">String</span></span>|<span data-ttu-id="66fcc-134">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="66fcc-134">The friendly name</span></span>|
|<span data-ttu-id="66fcc-135">fileHash</span><span class="sxs-lookup"><span data-stu-id="66fcc-135">fileHash</span></span>|<span data-ttu-id="66fcc-136">String</span><span class="sxs-lookup"><span data-stu-id="66fcc-136">String</span></span>|<span data-ttu-id="66fcc-137">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="66fcc-137">SHA256 hash of the file</span></span>|
|<span data-ttu-id="66fcc-138">file</span><span class="sxs-lookup"><span data-stu-id="66fcc-138">file</span></span>|<span data-ttu-id="66fcc-139">Binary</span><span class="sxs-lookup"><span data-stu-id="66fcc-139">Binary</span></span>|<span data-ttu-id="66fcc-140">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="66fcc-140">File as a byte array</span></span>|
|<span data-ttu-id="66fcc-141">id</span><span class="sxs-lookup"><span data-stu-id="66fcc-141">id</span></span>|<span data-ttu-id="66fcc-142">String</span><span class="sxs-lookup"><span data-stu-id="66fcc-142">String</span></span>|<span data-ttu-id="66fcc-143">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="66fcc-143">Key of the entity.</span></span>|
|<span data-ttu-id="66fcc-144">version</span><span class="sxs-lookup"><span data-stu-id="66fcc-144">version</span></span>|<span data-ttu-id="66fcc-145">Строка</span><span class="sxs-lookup"><span data-stu-id="66fcc-145">String</span></span>|<span data-ttu-id="66fcc-146">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="66fcc-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="66fcc-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="66fcc-147">Response</span></span>
<span data-ttu-id="66fcc-148">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="66fcc-148">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66fcc-149">Пример</span><span class="sxs-lookup"><span data-stu-id="66fcc-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="66fcc-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="66fcc-150">Request</span></span>
<span data-ttu-id="66fcc-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="66fcc-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="66fcc-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="66fcc-152">Response</span></span>
<span data-ttu-id="66fcc-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="66fcc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





