---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5c28ff97747f6132edbd89951c4fdfd6aa13941a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919255"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="9d46e-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="9d46e-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="9d46e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d46e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d46e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d46e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d46e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d46e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d46e-107">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="9d46e-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d46e-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9d46e-108">Prerequisites</span></span>
<span data-ttu-id="9d46e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d46e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d46e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9d46e-111">Permission type</span></span>|<span data-ttu-id="9d46e-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9d46e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d46e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9d46e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d46e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d46e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9d46e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9d46e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d46e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d46e-116">Not supported.</span></span>|
|<span data-ttu-id="9d46e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9d46e-117">Application</span></span>|<span data-ttu-id="9d46e-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d46e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d46e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9d46e-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9d46e-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9d46e-120">Request headers</span></span>
|<span data-ttu-id="9d46e-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9d46e-121">Header</span></span>|<span data-ttu-id="9d46e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9d46e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d46e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d46e-123">Authorization</span></span>|<span data-ttu-id="9d46e-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9d46e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d46e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9d46e-125">Accept</span></span>|<span data-ttu-id="9d46e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9d46e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d46e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9d46e-127">Request body</span></span>
<span data-ttu-id="9d46e-128">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d46e-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="9d46e-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="9d46e-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="9d46e-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d46e-130">Property</span></span>|<span data-ttu-id="9d46e-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9d46e-131">Type</span></span>|<span data-ttu-id="9d46e-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9d46e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d46e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="9d46e-133">displayName</span></span>|<span data-ttu-id="9d46e-134">String</span><span class="sxs-lookup"><span data-stu-id="9d46e-134">String</span></span>|<span data-ttu-id="9d46e-135">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="9d46e-135">The friendly name</span></span>|
|<span data-ttu-id="9d46e-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="9d46e-136">fileHash</span></span>|<span data-ttu-id="9d46e-137">String</span><span class="sxs-lookup"><span data-stu-id="9d46e-137">String</span></span>|<span data-ttu-id="9d46e-138">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="9d46e-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="9d46e-139">file</span><span class="sxs-lookup"><span data-stu-id="9d46e-139">file</span></span>|<span data-ttu-id="9d46e-140">Binary</span><span class="sxs-lookup"><span data-stu-id="9d46e-140">Binary</span></span>|<span data-ttu-id="9d46e-141">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="9d46e-141">File as a byte array</span></span>|
|<span data-ttu-id="9d46e-142">id</span><span class="sxs-lookup"><span data-stu-id="9d46e-142">id</span></span>|<span data-ttu-id="9d46e-143">String</span><span class="sxs-lookup"><span data-stu-id="9d46e-143">String</span></span>|<span data-ttu-id="9d46e-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9d46e-144">Key of the entity.</span></span>|
|<span data-ttu-id="9d46e-145">version</span><span class="sxs-lookup"><span data-stu-id="9d46e-145">version</span></span>|<span data-ttu-id="9d46e-146">String</span><span class="sxs-lookup"><span data-stu-id="9d46e-146">String</span></span>|<span data-ttu-id="9d46e-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="9d46e-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="9d46e-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="9d46e-148">Response</span></span>
<span data-ttu-id="9d46e-149">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9d46e-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d46e-150">Пример</span><span class="sxs-lookup"><span data-stu-id="9d46e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d46e-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="9d46e-151">Request</span></span>
<span data-ttu-id="9d46e-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9d46e-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9d46e-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="9d46e-153">Response</span></span>
<span data-ttu-id="9d46e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9d46e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





