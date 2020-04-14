---
title: Создание Иосвппаппассигнедусерлиценсе
description: Создание нового объекта Иосвппаппассигнедусерлиценсе.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0794c6ecfcd509cff8413c088aad6fa49598e784
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43416516"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="cb234-103">Создание Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="cb234-103">Create iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="cb234-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb234-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb234-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb234-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb234-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cb234-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb234-107">Создание нового объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="cb234-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cb234-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cb234-108">Prerequisites</span></span>
<span data-ttu-id="cb234-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb234-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb234-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb234-111">Permission type</span></span>|<span data-ttu-id="cb234-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb234-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb234-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb234-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cb234-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb234-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cb234-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb234-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb234-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb234-116">Not supported.</span></span>|
|<span data-ttu-id="cb234-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="cb234-117">Application</span></span>|<span data-ttu-id="cb234-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb234-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb234-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb234-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="cb234-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="cb234-120">Request headers</span></span>
|<span data-ttu-id="cb234-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cb234-121">Header</span></span>|<span data-ttu-id="cb234-122">Значение</span><span class="sxs-lookup"><span data-stu-id="cb234-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cb234-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb234-123">Authorization</span></span>|<span data-ttu-id="cb234-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb234-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cb234-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cb234-125">Accept</span></span>|<span data-ttu-id="cb234-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cb234-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb234-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb234-127">Request body</span></span>
<span data-ttu-id="cb234-128">В тексте запроса добавьте представление объекта Иосвппаппассигнедусерлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cb234-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="cb234-129">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнедусерлиценсе.</span><span class="sxs-lookup"><span data-stu-id="cb234-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="cb234-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb234-130">Property</span></span>|<span data-ttu-id="cb234-131">Тип</span><span class="sxs-lookup"><span data-stu-id="cb234-131">Type</span></span>|<span data-ttu-id="cb234-132">Описание</span><span class="sxs-lookup"><span data-stu-id="cb234-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb234-133">id</span><span class="sxs-lookup"><span data-stu-id="cb234-133">id</span></span>|<span data-ttu-id="cb234-134">Строка</span><span class="sxs-lookup"><span data-stu-id="cb234-134">String</span></span>|<span data-ttu-id="cb234-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cb234-135">Key of the entity.</span></span> <span data-ttu-id="cb234-136">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="cb234-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="cb234-137">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="cb234-137">userEmailAddress</span></span>|<span data-ttu-id="cb234-138">String</span><span class="sxs-lookup"><span data-stu-id="cb234-138">String</span></span>|<span data-ttu-id="cb234-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb234-139">The user email address.</span></span> <span data-ttu-id="cb234-140">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="cb234-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="cb234-141">userId</span><span class="sxs-lookup"><span data-stu-id="cb234-141">userId</span></span>|<span data-ttu-id="cb234-142">String</span><span class="sxs-lookup"><span data-stu-id="cb234-142">String</span></span>|<span data-ttu-id="cb234-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb234-143">The user ID.</span></span> <span data-ttu-id="cb234-144">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="cb234-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="cb234-145">userName</span><span class="sxs-lookup"><span data-stu-id="cb234-145">userName</span></span>|<span data-ttu-id="cb234-146">String</span><span class="sxs-lookup"><span data-stu-id="cb234-146">String</span></span>|<span data-ttu-id="cb234-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb234-147">The user name.</span></span> <span data-ttu-id="cb234-148">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="cb234-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="cb234-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cb234-149">userPrincipalName</span></span>|<span data-ttu-id="cb234-150">Строка</span><span class="sxs-lookup"><span data-stu-id="cb234-150">String</span></span>|<span data-ttu-id="cb234-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb234-151">The user principal name.</span></span> <span data-ttu-id="cb234-152">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="cb234-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="cb234-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb234-153">Response</span></span>
<span data-ttu-id="cb234-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cb234-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb234-155">Пример</span><span class="sxs-lookup"><span data-stu-id="cb234-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="cb234-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb234-156">Request</span></span>
<span data-ttu-id="cb234-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb234-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
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

### <a name="response"></a><span data-ttu-id="cb234-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="cb234-158">Response</span></span>
<span data-ttu-id="cb234-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb234-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



