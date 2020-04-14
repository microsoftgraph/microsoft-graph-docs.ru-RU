---
title: Создание Макосвппаппассигнедлиценсе
description: Создание нового объекта Макосвппаппассигнедлиценсе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c2c3b21dcf8d7240a697b52af000bf27f48fce5c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416033"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="8e2c9-103">Создание Макосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="8e2c9-103">Create macOsVppAppAssignedLicense</span></span>

<span data-ttu-id="8e2c9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e2c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e2c9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e2c9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e2c9-107">Создание нового объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="8e2c9-107">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e2c9-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8e2c9-108">Prerequisites</span></span>
<span data-ttu-id="8e2c9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8e2c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e2c9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8e2c9-111">Permission type</span></span>|<span data-ttu-id="8e2c9-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8e2c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e2c9-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8e2c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e2c9-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e2c9-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e2c9-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8e2c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e2c9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-116">Not supported.</span></span>|
|<span data-ttu-id="8e2c9-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="8e2c9-117">Application</span></span>|<span data-ttu-id="8e2c9-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e2c9-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e2c9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8e2c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="8e2c9-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="8e2c9-120">Request headers</span></span>
|<span data-ttu-id="8e2c9-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8e2c9-121">Header</span></span>|<span data-ttu-id="8e2c9-122">Значение</span><span class="sxs-lookup"><span data-stu-id="8e2c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e2c9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e2c9-123">Authorization</span></span>|<span data-ttu-id="8e2c9-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e2c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e2c9-125">Accept</span></span>|<span data-ttu-id="8e2c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e2c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e2c9-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8e2c9-127">Request body</span></span>
<span data-ttu-id="8e2c9-128">В тексте запроса добавьте представление объекта Макосвппаппассигнедлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-128">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="8e2c9-129">В следующей таблице приведены свойства, необходимые при создании Макосвппаппассигнедлиценсе.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-129">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="8e2c9-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8e2c9-130">Property</span></span>|<span data-ttu-id="8e2c9-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8e2c9-131">Type</span></span>|<span data-ttu-id="8e2c9-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8e2c9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e2c9-133">id</span><span class="sxs-lookup"><span data-stu-id="8e2c9-133">id</span></span>|<span data-ttu-id="8e2c9-134">Строка</span><span class="sxs-lookup"><span data-stu-id="8e2c9-134">String</span></span>|<span data-ttu-id="8e2c9-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-135">Key of the entity.</span></span>|
|<span data-ttu-id="8e2c9-136">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="8e2c9-136">userEmailAddress</span></span>|<span data-ttu-id="8e2c9-137">String</span><span class="sxs-lookup"><span data-stu-id="8e2c9-137">String</span></span>|<span data-ttu-id="8e2c9-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-138">The user email address.</span></span>|
|<span data-ttu-id="8e2c9-139">userId</span><span class="sxs-lookup"><span data-stu-id="8e2c9-139">userId</span></span>|<span data-ttu-id="8e2c9-140">String</span><span class="sxs-lookup"><span data-stu-id="8e2c9-140">String</span></span>|<span data-ttu-id="8e2c9-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-141">The user ID.</span></span>|
|<span data-ttu-id="8e2c9-142">userName</span><span class="sxs-lookup"><span data-stu-id="8e2c9-142">userName</span></span>|<span data-ttu-id="8e2c9-143">String</span><span class="sxs-lookup"><span data-stu-id="8e2c9-143">String</span></span>|<span data-ttu-id="8e2c9-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-144">The user name.</span></span>|
|<span data-ttu-id="8e2c9-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8e2c9-145">userPrincipalName</span></span>|<span data-ttu-id="8e2c9-146">Строка</span><span class="sxs-lookup"><span data-stu-id="8e2c9-146">String</span></span>|<span data-ttu-id="8e2c9-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="8e2c9-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e2c9-148">Response</span></span>
<span data-ttu-id="8e2c9-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-149">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e2c9-150">Пример</span><span class="sxs-lookup"><span data-stu-id="8e2c9-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e2c9-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="8e2c9-151">Request</span></span>
<span data-ttu-id="8e2c9-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="8e2c9-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="8e2c9-153">Response</span></span>
<span data-ttu-id="8e2c9-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8e2c9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```



