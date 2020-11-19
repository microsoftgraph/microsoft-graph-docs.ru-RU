---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d396416da77cc0469fb2e295f3527f39b950d5d9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49277255"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="c2b34-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="c2b34-103">Create windowsInformationProtectionAppLockerFile</span></span>

<span data-ttu-id="c2b34-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2b34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2b34-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2b34-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2b34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2b34-107">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c2b34-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2b34-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2b34-108">Prerequisites</span></span>
<span data-ttu-id="c2b34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2b34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2b34-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2b34-111">Permission type</span></span>|<span data-ttu-id="c2b34-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2b34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2b34-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2b34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2b34-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b34-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2b34-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2b34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2b34-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2b34-116">Not supported.</span></span>|
|<span data-ttu-id="c2b34-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2b34-117">Application</span></span>|<span data-ttu-id="c2b34-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2b34-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2b34-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2b34-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c2b34-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c2b34-120">Request headers</span></span>
|<span data-ttu-id="c2b34-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2b34-121">Header</span></span>|<span data-ttu-id="c2b34-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c2b34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2b34-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2b34-123">Authorization</span></span>|<span data-ttu-id="c2b34-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2b34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2b34-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c2b34-125">Accept</span></span>|<span data-ttu-id="c2b34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2b34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2b34-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2b34-127">Request body</span></span>
<span data-ttu-id="c2b34-128">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2b34-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="c2b34-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="c2b34-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="c2b34-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2b34-130">Property</span></span>|<span data-ttu-id="c2b34-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c2b34-131">Type</span></span>|<span data-ttu-id="c2b34-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c2b34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2b34-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c2b34-133">displayName</span></span>|<span data-ttu-id="c2b34-134">String</span><span class="sxs-lookup"><span data-stu-id="c2b34-134">String</span></span>|<span data-ttu-id="c2b34-135">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="c2b34-135">The friendly name</span></span>|
|<span data-ttu-id="c2b34-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="c2b34-136">fileHash</span></span>|<span data-ttu-id="c2b34-137">String</span><span class="sxs-lookup"><span data-stu-id="c2b34-137">String</span></span>|<span data-ttu-id="c2b34-138">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="c2b34-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="c2b34-139">file</span><span class="sxs-lookup"><span data-stu-id="c2b34-139">file</span></span>|<span data-ttu-id="c2b34-140">Binary</span><span class="sxs-lookup"><span data-stu-id="c2b34-140">Binary</span></span>|<span data-ttu-id="c2b34-141">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="c2b34-141">File as a byte array</span></span>|
|<span data-ttu-id="c2b34-142">id</span><span class="sxs-lookup"><span data-stu-id="c2b34-142">id</span></span>|<span data-ttu-id="c2b34-143">String</span><span class="sxs-lookup"><span data-stu-id="c2b34-143">String</span></span>|<span data-ttu-id="c2b34-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2b34-144">Key of the entity.</span></span>|
|<span data-ttu-id="c2b34-145">version</span><span class="sxs-lookup"><span data-stu-id="c2b34-145">version</span></span>|<span data-ttu-id="c2b34-146">String</span><span class="sxs-lookup"><span data-stu-id="c2b34-146">String</span></span>|<span data-ttu-id="c2b34-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="c2b34-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c2b34-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b34-148">Response</span></span>
<span data-ttu-id="c2b34-149">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c2b34-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2b34-150">Пример</span><span class="sxs-lookup"><span data-stu-id="c2b34-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2b34-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2b34-151">Request</span></span>
<span data-ttu-id="c2b34-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2b34-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2b34-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2b34-153">Response</span></span>
<span data-ttu-id="c2b34-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2b34-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




