---
title: Обновление объекта windowsInformationProtectionAppLockerFile
description: Обновление свойств объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d42d85d1ca2151239dd9e96b8337d0dab6538ce0
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263184"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="45964-103">Обновление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="45964-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="45964-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45964-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45964-105">Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="45964-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45964-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="45964-106">Prerequisites</span></span>
<span data-ttu-id="45964-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="45964-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="45964-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45964-109">Permission type</span></span>|<span data-ttu-id="45964-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45964-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45964-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45964-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45964-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45964-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45964-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45964-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45964-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45964-114">Not supported.</span></span>|
|<span data-ttu-id="45964-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45964-115">Application</span></span>|<span data-ttu-id="45964-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45964-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45964-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45964-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="45964-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45964-118">Request headers</span></span>
|<span data-ttu-id="45964-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45964-119">Header</span></span>|<span data-ttu-id="45964-120">Значение</span><span class="sxs-lookup"><span data-stu-id="45964-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45964-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45964-121">Authorization</span></span>|<span data-ttu-id="45964-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="45964-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45964-123">Accept</span><span class="sxs-lookup"><span data-stu-id="45964-123">Accept</span></span>|<span data-ttu-id="45964-124">application/json</span><span class="sxs-lookup"><span data-stu-id="45964-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45964-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45964-125">Request body</span></span>
<span data-ttu-id="45964-126">В теле запроса добавьте представление объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45964-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="45964-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="45964-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="45964-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="45964-128">Property</span></span>|<span data-ttu-id="45964-129">Тип</span><span class="sxs-lookup"><span data-stu-id="45964-129">Type</span></span>|<span data-ttu-id="45964-130">Описание</span><span class="sxs-lookup"><span data-stu-id="45964-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45964-131">displayName</span><span class="sxs-lookup"><span data-stu-id="45964-131">displayName</span></span>|<span data-ttu-id="45964-132">String</span><span class="sxs-lookup"><span data-stu-id="45964-132">String</span></span>|<span data-ttu-id="45964-133">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="45964-133">The friendly name</span></span>|
|<span data-ttu-id="45964-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="45964-134">fileHash</span></span>|<span data-ttu-id="45964-135">String</span><span class="sxs-lookup"><span data-stu-id="45964-135">String</span></span>|<span data-ttu-id="45964-136">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="45964-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="45964-137">file</span><span class="sxs-lookup"><span data-stu-id="45964-137">file</span></span>|<span data-ttu-id="45964-138">Binary</span><span class="sxs-lookup"><span data-stu-id="45964-138">Binary</span></span>|<span data-ttu-id="45964-139">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="45964-139">File as a byte array</span></span>|
|<span data-ttu-id="45964-140">id</span><span class="sxs-lookup"><span data-stu-id="45964-140">id</span></span>|<span data-ttu-id="45964-141">String</span><span class="sxs-lookup"><span data-stu-id="45964-141">String</span></span>|<span data-ttu-id="45964-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="45964-142">Key of the entity.</span></span>|
|<span data-ttu-id="45964-143">version</span><span class="sxs-lookup"><span data-stu-id="45964-143">version</span></span>|<span data-ttu-id="45964-144">Строка</span><span class="sxs-lookup"><span data-stu-id="45964-144">String</span></span>|<span data-ttu-id="45964-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="45964-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="45964-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="45964-146">Response</span></span>
<span data-ttu-id="45964-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="45964-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45964-148">Пример</span><span class="sxs-lookup"><span data-stu-id="45964-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="45964-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="45964-149">Request</span></span>
<span data-ttu-id="45964-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45964-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="45964-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="45964-151">Response</span></span>
<span data-ttu-id="45964-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="45964-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



