---
title: Обновление Иосвппаппассигнедусерлиценсе
description: Обновление свойств объекта Иосвппаппассигнедусерлиценсе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2eb8517c66b945b3bb0dda3f8b8e83f2f6cf68d0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43394379"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="c3537-103">Обновление Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="c3537-103">Update iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="c3537-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3537-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3537-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3537-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3537-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c3537-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3537-107">Обновление свойств объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="c3537-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3537-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c3537-108">Prerequisites</span></span>
<span data-ttu-id="c3537-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3537-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3537-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3537-111">Permission type</span></span>|<span data-ttu-id="c3537-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3537-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3537-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3537-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3537-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3537-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3537-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3537-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3537-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3537-116">Not supported.</span></span>|
|<span data-ttu-id="c3537-117">Для приложения</span><span class="sxs-lookup"><span data-stu-id="c3537-117">Application</span></span>|<span data-ttu-id="c3537-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3537-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3537-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3537-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="c3537-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="c3537-120">Request headers</span></span>
|<span data-ttu-id="c3537-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c3537-121">Header</span></span>|<span data-ttu-id="c3537-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c3537-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3537-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3537-123">Authorization</span></span>|<span data-ttu-id="c3537-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3537-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3537-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3537-125">Accept</span></span>|<span data-ttu-id="c3537-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3537-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3537-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3537-127">Request body</span></span>
<span data-ttu-id="c3537-128">В тексте запроса добавьте представление объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3537-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="c3537-129">В следующей таблице приведены свойства, необходимые при создании [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="c3537-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="c3537-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3537-130">Property</span></span>|<span data-ttu-id="c3537-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c3537-131">Type</span></span>|<span data-ttu-id="c3537-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c3537-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3537-133">id</span><span class="sxs-lookup"><span data-stu-id="c3537-133">id</span></span>|<span data-ttu-id="c3537-134">Строка</span><span class="sxs-lookup"><span data-stu-id="c3537-134">String</span></span>|<span data-ttu-id="c3537-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c3537-135">Key of the entity.</span></span> <span data-ttu-id="c3537-136">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c3537-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c3537-137">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="c3537-137">userEmailAddress</span></span>|<span data-ttu-id="c3537-138">String</span><span class="sxs-lookup"><span data-stu-id="c3537-138">String</span></span>|<span data-ttu-id="c3537-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3537-139">The user email address.</span></span> <span data-ttu-id="c3537-140">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c3537-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c3537-141">userId</span><span class="sxs-lookup"><span data-stu-id="c3537-141">userId</span></span>|<span data-ttu-id="c3537-142">String</span><span class="sxs-lookup"><span data-stu-id="c3537-142">String</span></span>|<span data-ttu-id="c3537-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3537-143">The user ID.</span></span> <span data-ttu-id="c3537-144">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c3537-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c3537-145">userName</span><span class="sxs-lookup"><span data-stu-id="c3537-145">userName</span></span>|<span data-ttu-id="c3537-146">String</span><span class="sxs-lookup"><span data-stu-id="c3537-146">String</span></span>|<span data-ttu-id="c3537-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3537-147">The user name.</span></span> <span data-ttu-id="c3537-148">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c3537-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c3537-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c3537-149">userPrincipalName</span></span>|<span data-ttu-id="c3537-150">Строка</span><span class="sxs-lookup"><span data-stu-id="c3537-150">String</span></span>|<span data-ttu-id="c3537-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3537-151">The user principal name.</span></span> <span data-ttu-id="c3537-152">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c3537-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c3537-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3537-153">Response</span></span>
<span data-ttu-id="c3537-154">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c3537-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3537-155">Пример</span><span class="sxs-lookup"><span data-stu-id="c3537-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3537-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3537-156">Request</span></span>
<span data-ttu-id="c3537-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3537-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="c3537-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3537-158">Response</span></span>
<span data-ttu-id="c3537-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3537-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```



