---
title: Создание Иосвппаппассигнедусерлиценсе
description: Создание нового объекта Иосвппаппассигнедусерлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 95f731739557aa14e14073fe1998fca0e7a75fa1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42445448"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="5548c-103">Создание Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="5548c-103">Create iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="5548c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5548c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5548c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5548c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5548c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5548c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5548c-107">Создание нового объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="5548c-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5548c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="5548c-108">Prerequisites</span></span>
<span data-ttu-id="5548c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5548c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5548c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5548c-111">Permission type</span></span>|<span data-ttu-id="5548c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5548c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5548c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5548c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5548c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5548c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5548c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5548c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5548c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5548c-116">Not supported.</span></span>|
|<span data-ttu-id="5548c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5548c-117">Application</span></span>|<span data-ttu-id="5548c-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5548c-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5548c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5548c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="5548c-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="5548c-120">Request headers</span></span>
|<span data-ttu-id="5548c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5548c-121">Header</span></span>|<span data-ttu-id="5548c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="5548c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5548c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5548c-123">Authorization</span></span>|<span data-ttu-id="5548c-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5548c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5548c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5548c-125">Accept</span></span>|<span data-ttu-id="5548c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5548c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5548c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5548c-127">Request body</span></span>
<span data-ttu-id="5548c-128">В тексте запроса добавьте представление объекта Иосвппаппассигнедусерлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5548c-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="5548c-129">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнедусерлиценсе.</span><span class="sxs-lookup"><span data-stu-id="5548c-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="5548c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5548c-130">Property</span></span>|<span data-ttu-id="5548c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5548c-131">Type</span></span>|<span data-ttu-id="5548c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5548c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5548c-133">id</span><span class="sxs-lookup"><span data-stu-id="5548c-133">id</span></span>|<span data-ttu-id="5548c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="5548c-134">String</span></span>|<span data-ttu-id="5548c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="5548c-135">Key of the entity.</span></span> <span data-ttu-id="5548c-136">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5548c-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="5548c-137">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="5548c-137">userEmailAddress</span></span>|<span data-ttu-id="5548c-138">String</span><span class="sxs-lookup"><span data-stu-id="5548c-138">String</span></span>|<span data-ttu-id="5548c-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="5548c-139">The user email address.</span></span> <span data-ttu-id="5548c-140">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5548c-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="5548c-141">userId</span><span class="sxs-lookup"><span data-stu-id="5548c-141">userId</span></span>|<span data-ttu-id="5548c-142">String</span><span class="sxs-lookup"><span data-stu-id="5548c-142">String</span></span>|<span data-ttu-id="5548c-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="5548c-143">The user ID.</span></span> <span data-ttu-id="5548c-144">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5548c-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="5548c-145">userName</span><span class="sxs-lookup"><span data-stu-id="5548c-145">userName</span></span>|<span data-ttu-id="5548c-146">String</span><span class="sxs-lookup"><span data-stu-id="5548c-146">String</span></span>|<span data-ttu-id="5548c-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="5548c-147">The user name.</span></span> <span data-ttu-id="5548c-148">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5548c-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="5548c-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5548c-149">userPrincipalName</span></span>|<span data-ttu-id="5548c-150">Строка</span><span class="sxs-lookup"><span data-stu-id="5548c-150">String</span></span>|<span data-ttu-id="5548c-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="5548c-151">The user principal name.</span></span> <span data-ttu-id="5548c-152">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="5548c-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5548c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="5548c-153">Response</span></span>
<span data-ttu-id="5548c-154">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5548c-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5548c-155">Пример</span><span class="sxs-lookup"><span data-stu-id="5548c-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="5548c-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="5548c-156">Request</span></span>
<span data-ttu-id="5548c-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5548c-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5548c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="5548c-158">Response</span></span>
<span data-ttu-id="5548c-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5548c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





