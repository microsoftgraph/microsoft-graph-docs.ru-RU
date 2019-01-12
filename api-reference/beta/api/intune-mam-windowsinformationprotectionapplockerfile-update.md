---
title: Обновление объекта windowsInformationProtectionAppLockerFile
description: Обновление свойств объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1787544bd84ca1037dafae5c26ec5f19e80fc2d0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990315"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="1d8c2-103">Обновление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="1d8c2-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="1d8c2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d8c2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1d8c2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d8c2-107">Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="1d8c2-107">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d8c2-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="1d8c2-108">Prerequisites</span></span>
<span data-ttu-id="1d8c2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d8c2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d8c2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1d8c2-111">Permission type</span></span>|<span data-ttu-id="1d8c2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="1d8c2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d8c2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1d8c2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1d8c2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d8c2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d8c2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1d8c2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d8c2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-116">Not supported.</span></span>|
|<span data-ttu-id="1d8c2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1d8c2-117">Application</span></span>|<span data-ttu-id="1d8c2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d8c2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1d8c2-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="1d8c2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1d8c2-120">Request headers</span></span>
|<span data-ttu-id="1d8c2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="1d8c2-121">Header</span></span>|<span data-ttu-id="1d8c2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1d8c2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d8c2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d8c2-123">Authorization</span></span>|<span data-ttu-id="1d8c2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="1d8c2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d8c2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1d8c2-125">Accept</span></span>|<span data-ttu-id="1d8c2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1d8c2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d8c2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1d8c2-127">Request body</span></span>
<span data-ttu-id="1d8c2-128">В теле запроса добавьте представление объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-128">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="1d8c2-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="1d8c2-129">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="1d8c2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d8c2-130">Property</span></span>|<span data-ttu-id="1d8c2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="1d8c2-131">Type</span></span>|<span data-ttu-id="1d8c2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="1d8c2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d8c2-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1d8c2-133">displayName</span></span>|<span data-ttu-id="1d8c2-134">String</span><span class="sxs-lookup"><span data-stu-id="1d8c2-134">String</span></span>|<span data-ttu-id="1d8c2-135">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="1d8c2-135">The friendly name</span></span>|
|<span data-ttu-id="1d8c2-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="1d8c2-136">fileHash</span></span>|<span data-ttu-id="1d8c2-137">String</span><span class="sxs-lookup"><span data-stu-id="1d8c2-137">String</span></span>|<span data-ttu-id="1d8c2-138">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="1d8c2-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="1d8c2-139">file</span><span class="sxs-lookup"><span data-stu-id="1d8c2-139">file</span></span>|<span data-ttu-id="1d8c2-140">Binary</span><span class="sxs-lookup"><span data-stu-id="1d8c2-140">Binary</span></span>|<span data-ttu-id="1d8c2-141">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="1d8c2-141">File as a byte array</span></span>|
|<span data-ttu-id="1d8c2-142">id</span><span class="sxs-lookup"><span data-stu-id="1d8c2-142">id</span></span>|<span data-ttu-id="1d8c2-143">String</span><span class="sxs-lookup"><span data-stu-id="1d8c2-143">String</span></span>|<span data-ttu-id="1d8c2-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-144">Key of the entity.</span></span>|
|<span data-ttu-id="1d8c2-145">version</span><span class="sxs-lookup"><span data-stu-id="1d8c2-145">version</span></span>|<span data-ttu-id="1d8c2-146">String</span><span class="sxs-lookup"><span data-stu-id="1d8c2-146">String</span></span>|<span data-ttu-id="1d8c2-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="1d8c2-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="1d8c2-148">Response</span></span>
<span data-ttu-id="1d8c2-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-149">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d8c2-150">Пример</span><span class="sxs-lookup"><span data-stu-id="1d8c2-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d8c2-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="1d8c2-151">Request</span></span>
<span data-ttu-id="1d8c2-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1d8c2-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="1d8c2-153">Response</span></span>
<span data-ttu-id="1d8c2-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="1d8c2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





