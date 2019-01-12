---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a7b6bfb8271e6b462be1d18fd509da33aea836b3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967597"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="35fb9-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="35fb9-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="35fb9-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35fb9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35fb9-105">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="35fb9-105">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35fb9-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="35fb9-106">Prerequisites</span></span>
<span data-ttu-id="35fb9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35fb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35fb9-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35fb9-109">Permission type</span></span>|<span data-ttu-id="35fb9-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="35fb9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35fb9-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35fb9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="35fb9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35fb9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="35fb9-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35fb9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35fb9-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35fb9-114">Not supported.</span></span>|
|<span data-ttu-id="35fb9-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35fb9-115">Application</span></span>|<span data-ttu-id="35fb9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35fb9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35fb9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35fb9-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="35fb9-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35fb9-118">Request headers</span></span>
|<span data-ttu-id="35fb9-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="35fb9-119">Header</span></span>|<span data-ttu-id="35fb9-120">Значение</span><span class="sxs-lookup"><span data-stu-id="35fb9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35fb9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="35fb9-121">Authorization</span></span>|<span data-ttu-id="35fb9-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="35fb9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35fb9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="35fb9-123">Accept</span></span>|<span data-ttu-id="35fb9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="35fb9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35fb9-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="35fb9-125">Request body</span></span>
<span data-ttu-id="35fb9-126">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35fb9-126">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="35fb9-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="35fb9-127">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="35fb9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="35fb9-128">Property</span></span>|<span data-ttu-id="35fb9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="35fb9-129">Type</span></span>|<span data-ttu-id="35fb9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="35fb9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35fb9-131">displayName</span><span class="sxs-lookup"><span data-stu-id="35fb9-131">displayName</span></span>|<span data-ttu-id="35fb9-132">String</span><span class="sxs-lookup"><span data-stu-id="35fb9-132">String</span></span>|<span data-ttu-id="35fb9-133">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="35fb9-133">The friendly name</span></span>|
|<span data-ttu-id="35fb9-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="35fb9-134">fileHash</span></span>|<span data-ttu-id="35fb9-135">String</span><span class="sxs-lookup"><span data-stu-id="35fb9-135">String</span></span>|<span data-ttu-id="35fb9-136">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="35fb9-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="35fb9-137">file</span><span class="sxs-lookup"><span data-stu-id="35fb9-137">file</span></span>|<span data-ttu-id="35fb9-138">Binary</span><span class="sxs-lookup"><span data-stu-id="35fb9-138">Binary</span></span>|<span data-ttu-id="35fb9-139">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="35fb9-139">File as a byte array</span></span>|
|<span data-ttu-id="35fb9-140">id</span><span class="sxs-lookup"><span data-stu-id="35fb9-140">id</span></span>|<span data-ttu-id="35fb9-141">Строка</span><span class="sxs-lookup"><span data-stu-id="35fb9-141">String</span></span>|<span data-ttu-id="35fb9-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="35fb9-142">Key of the entity.</span></span>|
|<span data-ttu-id="35fb9-143">version</span><span class="sxs-lookup"><span data-stu-id="35fb9-143">version</span></span>|<span data-ttu-id="35fb9-144">Строка</span><span class="sxs-lookup"><span data-stu-id="35fb9-144">String</span></span>|<span data-ttu-id="35fb9-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="35fb9-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="35fb9-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="35fb9-146">Response</span></span>
<span data-ttu-id="35fb9-147">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="35fb9-147">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35fb9-148">Пример</span><span class="sxs-lookup"><span data-stu-id="35fb9-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="35fb9-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="35fb9-149">Request</span></span>
<span data-ttu-id="35fb9-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35fb9-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="35fb9-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="35fb9-151">Response</span></span>
<span data-ttu-id="35fb9-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="35fb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



