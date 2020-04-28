---
title: Обновление Макосвппаппассигнедлиценсе
description: Обновление свойств объекта Макосвппаппассигнедлиценсе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8033e840c4bfda4108f97f3e7b57e52a0586fb7d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43406440"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="e1710-103">Обновление Макосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="e1710-103">Update macOsVppAppAssignedLicense</span></span>

<span data-ttu-id="e1710-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1710-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1710-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1710-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1710-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1710-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1710-107">Обновление свойств объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="e1710-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1710-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e1710-108">Prerequisites</span></span>
<span data-ttu-id="e1710-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1710-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e1710-111">Permission type</span></span>|<span data-ttu-id="e1710-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e1710-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1710-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e1710-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1710-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1710-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e1710-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e1710-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1710-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1710-116">Not supported.</span></span>|
|<span data-ttu-id="e1710-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e1710-117">Application</span></span>|<span data-ttu-id="e1710-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1710-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1710-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e1710-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="e1710-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e1710-120">Request headers</span></span>
|<span data-ttu-id="e1710-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e1710-121">Header</span></span>|<span data-ttu-id="e1710-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e1710-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1710-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e1710-123">Authorization</span></span>|<span data-ttu-id="e1710-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e1710-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1710-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e1710-125">Accept</span></span>|<span data-ttu-id="e1710-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1710-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1710-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e1710-127">Request body</span></span>
<span data-ttu-id="e1710-128">В тексте запроса добавьте представление объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1710-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="e1710-129">В следующей таблице приведены свойства, необходимые при создании [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="e1710-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="e1710-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1710-130">Property</span></span>|<span data-ttu-id="e1710-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e1710-131">Type</span></span>|<span data-ttu-id="e1710-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e1710-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1710-133">id</span><span class="sxs-lookup"><span data-stu-id="e1710-133">id</span></span>|<span data-ttu-id="e1710-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e1710-134">String</span></span>|<span data-ttu-id="e1710-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e1710-135">Key of the entity.</span></span>|
|<span data-ttu-id="e1710-136">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="e1710-136">userEmailAddress</span></span>|<span data-ttu-id="e1710-137">String</span><span class="sxs-lookup"><span data-stu-id="e1710-137">String</span></span>|<span data-ttu-id="e1710-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1710-138">The user email address.</span></span>|
|<span data-ttu-id="e1710-139">userId</span><span class="sxs-lookup"><span data-stu-id="e1710-139">userId</span></span>|<span data-ttu-id="e1710-140">String</span><span class="sxs-lookup"><span data-stu-id="e1710-140">String</span></span>|<span data-ttu-id="e1710-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1710-141">The user ID.</span></span>|
|<span data-ttu-id="e1710-142">userName</span><span class="sxs-lookup"><span data-stu-id="e1710-142">userName</span></span>|<span data-ttu-id="e1710-143">String</span><span class="sxs-lookup"><span data-stu-id="e1710-143">String</span></span>|<span data-ttu-id="e1710-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1710-144">The user name.</span></span>|
|<span data-ttu-id="e1710-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1710-145">userPrincipalName</span></span>|<span data-ttu-id="e1710-146">Строка</span><span class="sxs-lookup"><span data-stu-id="e1710-146">String</span></span>|<span data-ttu-id="e1710-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="e1710-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="e1710-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="e1710-148">Response</span></span>
<span data-ttu-id="e1710-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e1710-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1710-150">Пример</span><span class="sxs-lookup"><span data-stu-id="e1710-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1710-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="e1710-151">Request</span></span>
<span data-ttu-id="e1710-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e1710-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="e1710-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="e1710-153">Response</span></span>
<span data-ttu-id="e1710-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e1710-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



