---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 13b6d9a0e8fc6e23b2a5b7b85e257ef8d3ac9c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853321"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="e635d-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="e635d-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="e635d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e635d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e635d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e635d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e635d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e635d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e635d-107">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="e635d-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e635d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="e635d-108">Prerequisites</span></span>
<span data-ttu-id="e635d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e635d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e635d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e635d-111">Permission type</span></span>|<span data-ttu-id="e635d-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e635d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e635d-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e635d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e635d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e635d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e635d-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e635d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e635d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e635d-116">Not supported.</span></span>|
|<span data-ttu-id="e635d-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e635d-117">Application</span></span>|<span data-ttu-id="e635d-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e635d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e635d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e635d-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e635d-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e635d-120">Request headers</span></span>
|<span data-ttu-id="e635d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e635d-121">Header</span></span>|<span data-ttu-id="e635d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e635d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e635d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e635d-123">Authorization</span></span>|<span data-ttu-id="e635d-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e635d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e635d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e635d-125">Accept</span></span>|<span data-ttu-id="e635d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e635d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e635d-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e635d-127">Request body</span></span>
<span data-ttu-id="e635d-128">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e635d-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="e635d-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="e635d-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="e635d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e635d-130">Property</span></span>|<span data-ttu-id="e635d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e635d-131">Type</span></span>|<span data-ttu-id="e635d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e635d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e635d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e635d-133">displayName</span></span>|<span data-ttu-id="e635d-134">String</span><span class="sxs-lookup"><span data-stu-id="e635d-134">String</span></span>|<span data-ttu-id="e635d-135">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="e635d-135">The friendly name</span></span>|
|<span data-ttu-id="e635d-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="e635d-136">fileHash</span></span>|<span data-ttu-id="e635d-137">String</span><span class="sxs-lookup"><span data-stu-id="e635d-137">String</span></span>|<span data-ttu-id="e635d-138">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="e635d-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="e635d-139">file</span><span class="sxs-lookup"><span data-stu-id="e635d-139">file</span></span>|<span data-ttu-id="e635d-140">Binary</span><span class="sxs-lookup"><span data-stu-id="e635d-140">Binary</span></span>|<span data-ttu-id="e635d-141">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="e635d-141">File as a byte array</span></span>|
|<span data-ttu-id="e635d-142">id</span><span class="sxs-lookup"><span data-stu-id="e635d-142">id</span></span>|<span data-ttu-id="e635d-143">Строка</span><span class="sxs-lookup"><span data-stu-id="e635d-143">String</span></span>|<span data-ttu-id="e635d-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e635d-144">Key of the entity.</span></span>|
|<span data-ttu-id="e635d-145">version</span><span class="sxs-lookup"><span data-stu-id="e635d-145">version</span></span>|<span data-ttu-id="e635d-146">Строка</span><span class="sxs-lookup"><span data-stu-id="e635d-146">String</span></span>|<span data-ttu-id="e635d-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="e635d-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="e635d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e635d-148">Response</span></span>
<span data-ttu-id="e635d-149">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e635d-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e635d-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e635d-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="e635d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e635d-151">Request</span></span>
<span data-ttu-id="e635d-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e635d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e635d-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="e635d-153">Response</span></span>
<span data-ttu-id="e635d-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e635d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





