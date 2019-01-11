---
title: Обновление объекта windowsInformationProtectionAppLockerFile
description: Обновление свойств объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 59b5fef4b2fd82f1275e14321c46aec0130ddb9a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826189"
---
# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="c2859-103">Обновление объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="c2859-103">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="c2859-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2859-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2859-105">Обновление свойств объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c2859-105">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c2859-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="c2859-106">Prerequisites</span></span>
<span data-ttu-id="c2859-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2859-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2859-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2859-109">Permission type</span></span>|<span data-ttu-id="c2859-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2859-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2859-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2859-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2859-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2859-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2859-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2859-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2859-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2859-114">Not supported.</span></span>|
|<span data-ttu-id="c2859-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2859-115">Application</span></span>|<span data-ttu-id="c2859-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2859-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2859-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2859-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c2859-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2859-118">Request headers</span></span>
|<span data-ttu-id="c2859-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2859-119">Header</span></span>|<span data-ttu-id="c2859-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c2859-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2859-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2859-121">Authorization</span></span>|<span data-ttu-id="c2859-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c2859-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2859-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c2859-123">Accept</span></span>|<span data-ttu-id="c2859-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c2859-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2859-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2859-125">Request body</span></span>
<span data-ttu-id="c2859-126">В теле запроса добавьте представление объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2859-126">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="c2859-127">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="c2859-127">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="c2859-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2859-128">Property</span></span>|<span data-ttu-id="c2859-129">Тип</span><span class="sxs-lookup"><span data-stu-id="c2859-129">Type</span></span>|<span data-ttu-id="c2859-130">Описание</span><span class="sxs-lookup"><span data-stu-id="c2859-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2859-131">displayName</span><span class="sxs-lookup"><span data-stu-id="c2859-131">displayName</span></span>|<span data-ttu-id="c2859-132">String</span><span class="sxs-lookup"><span data-stu-id="c2859-132">String</span></span>|<span data-ttu-id="c2859-133">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="c2859-133">The friendly name</span></span>|
|<span data-ttu-id="c2859-134">fileHash</span><span class="sxs-lookup"><span data-stu-id="c2859-134">fileHash</span></span>|<span data-ttu-id="c2859-135">String</span><span class="sxs-lookup"><span data-stu-id="c2859-135">String</span></span>|<span data-ttu-id="c2859-136">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="c2859-136">SHA256 hash of the file</span></span>|
|<span data-ttu-id="c2859-137">file</span><span class="sxs-lookup"><span data-stu-id="c2859-137">file</span></span>|<span data-ttu-id="c2859-138">Binary</span><span class="sxs-lookup"><span data-stu-id="c2859-138">Binary</span></span>|<span data-ttu-id="c2859-139">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="c2859-139">File as a byte array</span></span>|
|<span data-ttu-id="c2859-140">id</span><span class="sxs-lookup"><span data-stu-id="c2859-140">id</span></span>|<span data-ttu-id="c2859-141">Строка</span><span class="sxs-lookup"><span data-stu-id="c2859-141">String</span></span>|<span data-ttu-id="c2859-142">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c2859-142">Key of the entity.</span></span>|
|<span data-ttu-id="c2859-143">version</span><span class="sxs-lookup"><span data-stu-id="c2859-143">version</span></span>|<span data-ttu-id="c2859-144">Строка</span><span class="sxs-lookup"><span data-stu-id="c2859-144">String</span></span>|<span data-ttu-id="c2859-145">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="c2859-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="c2859-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2859-146">Response</span></span>
<span data-ttu-id="c2859-147">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c2859-147">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2859-148">Пример</span><span class="sxs-lookup"><span data-stu-id="c2859-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="c2859-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2859-149">Request</span></span>
<span data-ttu-id="c2859-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2859-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2859-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="c2859-151">Response</span></span>
<span data-ttu-id="c2859-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c2859-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



