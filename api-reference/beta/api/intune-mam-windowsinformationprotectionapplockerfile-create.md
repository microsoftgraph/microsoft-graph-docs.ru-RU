---
title: Создание объекта windowsInformationProtectionAppLockerFile
description: Создание объекта windowsInformationProtectionAppLockerFile.
author: tfitzmac
ms.openlocfilehash: f2cbed922d6f2ac130169e5d9c85e3a5231184a5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317124"
---
# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="631de-103">Создание объекта windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="631de-103">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="631de-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="631de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="631de-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="631de-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="631de-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="631de-107">Создание объекта [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span><span class="sxs-lookup"><span data-stu-id="631de-107">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="631de-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="631de-108">Prerequisites</span></span>
<span data-ttu-id="631de-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="631de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="631de-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="631de-111">Permission type</span></span>|<span data-ttu-id="631de-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="631de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="631de-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="631de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="631de-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="631de-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="631de-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="631de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="631de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631de-116">Not supported.</span></span>|
|<span data-ttu-id="631de-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="631de-117">Application</span></span>|<span data-ttu-id="631de-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="631de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="631de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="631de-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="631de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="631de-120">Request headers</span></span>
|<span data-ttu-id="631de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="631de-121">Header</span></span>|<span data-ttu-id="631de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="631de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="631de-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="631de-123">Authorization</span></span>|<span data-ttu-id="631de-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="631de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="631de-125">Accept</span><span class="sxs-lookup"><span data-stu-id="631de-125">Accept</span></span>|<span data-ttu-id="631de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="631de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="631de-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="631de-127">Request body</span></span>
<span data-ttu-id="631de-128">В теле запроса добавьте представление объекта windowsInformationProtectionAppLockerFile в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="631de-128">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="631de-129">В приведенной ниже таблице указаны свойства, необходимые при создании объекта windowsInformationProtectionAppLockerFile.</span><span class="sxs-lookup"><span data-stu-id="631de-129">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="631de-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="631de-130">Property</span></span>|<span data-ttu-id="631de-131">Тип</span><span class="sxs-lookup"><span data-stu-id="631de-131">Type</span></span>|<span data-ttu-id="631de-132">Описание</span><span class="sxs-lookup"><span data-stu-id="631de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="631de-133">displayName</span><span class="sxs-lookup"><span data-stu-id="631de-133">displayName</span></span>|<span data-ttu-id="631de-134">String</span><span class="sxs-lookup"><span data-stu-id="631de-134">String</span></span>|<span data-ttu-id="631de-135">Понятное имя</span><span class="sxs-lookup"><span data-stu-id="631de-135">The friendly name</span></span>|
|<span data-ttu-id="631de-136">fileHash</span><span class="sxs-lookup"><span data-stu-id="631de-136">fileHash</span></span>|<span data-ttu-id="631de-137">String</span><span class="sxs-lookup"><span data-stu-id="631de-137">String</span></span>|<span data-ttu-id="631de-138">Хэш SHA256 для файла</span><span class="sxs-lookup"><span data-stu-id="631de-138">SHA256 hash of the file</span></span>|
|<span data-ttu-id="631de-139">file</span><span class="sxs-lookup"><span data-stu-id="631de-139">file</span></span>|<span data-ttu-id="631de-140">Binary</span><span class="sxs-lookup"><span data-stu-id="631de-140">Binary</span></span>|<span data-ttu-id="631de-141">Файл в виде массива байтов</span><span class="sxs-lookup"><span data-stu-id="631de-141">File as a byte array</span></span>|
|<span data-ttu-id="631de-142">id</span><span class="sxs-lookup"><span data-stu-id="631de-142">id</span></span>|<span data-ttu-id="631de-143">Строка</span><span class="sxs-lookup"><span data-stu-id="631de-143">String</span></span>|<span data-ttu-id="631de-144">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="631de-144">Key of the entity.</span></span>|
|<span data-ttu-id="631de-145">version</span><span class="sxs-lookup"><span data-stu-id="631de-145">version</span></span>|<span data-ttu-id="631de-146">Строка</span><span class="sxs-lookup"><span data-stu-id="631de-146">String</span></span>|<span data-ttu-id="631de-147">Версия объекта.</span><span class="sxs-lookup"><span data-stu-id="631de-147">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="631de-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="631de-148">Response</span></span>
<span data-ttu-id="631de-149">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="631de-149">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="631de-150">Пример</span><span class="sxs-lookup"><span data-stu-id="631de-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="631de-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="631de-151">Request</span></span>
<span data-ttu-id="631de-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="631de-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="631de-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="631de-153">Response</span></span>
<span data-ttu-id="631de-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="631de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





