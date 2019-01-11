---
title: Обновление объекта windowsInformationProtectionAppLockerFile
description: Обновление свойств объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a81a42b1245a8723935ac8497e69539b1e5c1df8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885679"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="5e3bc-103">Обновление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="5e3bc-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="5e3bc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e3bc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e3bc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e3bc-107">Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5e3bc-107">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e3bc-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5e3bc-108">Prerequisites</span></span>
<span data-ttu-id="5e3bc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e3bc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e3bc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e3bc-111">Permission type</span></span>|<span data-ttu-id="5e3bc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e3bc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e3bc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e3bc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5e3bc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e3bc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5e3bc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e3bc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e3bc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-116">Not supported.</span></span>|
|<span data-ttu-id="5e3bc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e3bc-117">Application</span></span>|<span data-ttu-id="5e3bc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e3bc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e3bc-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="5e3bc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e3bc-120">Request headers</span></span>
|<span data-ttu-id="5e3bc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e3bc-121">Header</span></span>|<span data-ttu-id="5e3bc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5e3bc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e3bc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e3bc-123">Authorization</span></span>|<span data-ttu-id="5e3bc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="5e3bc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e3bc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5e3bc-125">Accept</span></span>|<span data-ttu-id="5e3bc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5e3bc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e3bc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="5e3bc-127">Request body</span></span>
<span data-ttu-id="5e3bc-128">В теле запроса добавьте представление объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="5e3bc-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="5e3bc-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="5e3bc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e3bc-130">Property</span></span>|<span data-ttu-id="5e3bc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5e3bc-131">Type</span></span>|<span data-ttu-id="5e3bc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5e3bc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e3bc-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5e3bc-133">displayName</span></span>|<span data-ttu-id="5e3bc-134">String</span><span class="sxs-lookup"><span data-stu-id="5e3bc-134">String</span></span>|<span data-ttu-id="5e3bc-135">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="5e3bc-135">The friendly name</span></span>|
|<span data-ttu-id="5e3bc-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="5e3bc-136">fileHash</span></span>|<span data-ttu-id="5e3bc-137">String</span><span class="sxs-lookup"><span data-stu-id="5e3bc-137">String</span></span>|<span data-ttu-id="5e3bc-138">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="5e3bc-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="5e3bc-139">file</span><span class="sxs-lookup"><span data-stu-id="5e3bc-139">file</span></span>|<span data-ttu-id="5e3bc-140">Binary</span><span class="sxs-lookup"><span data-stu-id="5e3bc-140">Binary</span></span>|<span data-ttu-id="5e3bc-141">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="5e3bc-141">File as a byte array</span></span>|
|<span data-ttu-id="5e3bc-142">id</span><span class="sxs-lookup"><span data-stu-id="5e3bc-142">id</span></span>|<span data-ttu-id="5e3bc-143">Строка</span><span class="sxs-lookup"><span data-stu-id="5e3bc-143">String</span></span>|<span data-ttu-id="5e3bc-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-144">Key of the entity.</span></span>|
|<span data-ttu-id="5e3bc-145">version</span><span class="sxs-lookup"><span data-stu-id="5e3bc-145">version</span></span>|<span data-ttu-id="5e3bc-146">Строка</span><span class="sxs-lookup"><span data-stu-id="5e3bc-146">String</span></span>|<span data-ttu-id="5e3bc-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="5e3bc-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e3bc-148">Response</span></span>
<span data-ttu-id="5e3bc-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-149">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e3bc-150">Пример</span><span class="sxs-lookup"><span data-stu-id="5e3bc-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e3bc-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e3bc-151">Request</span></span>
<span data-ttu-id="5e3bc-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 131

{
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="5e3bc-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="5e3bc-153">Response</span></span>
<span data-ttu-id="5e3bc-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="5e3bc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





