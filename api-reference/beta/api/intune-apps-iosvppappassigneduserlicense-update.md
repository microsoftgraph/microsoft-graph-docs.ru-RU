---
title: Обновление Иосвппаппассигнедусерлиценсе
description: Обновление свойств объекта Иосвппаппассигнедусерлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e024ab6350a94c6707165fc2bae5f3184bd66d9f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177691"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="41dce-103">Обновление Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="41dce-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="41dce-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41dce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41dce-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41dce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41dce-106">Обновление свойств объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="41dce-106">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41dce-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="41dce-107">Prerequisites</span></span>
<span data-ttu-id="41dce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41dce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41dce-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41dce-110">Permission type</span></span>|<span data-ttu-id="41dce-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="41dce-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41dce-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41dce-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41dce-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41dce-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="41dce-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41dce-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41dce-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41dce-115">Not supported.</span></span>|
|<span data-ttu-id="41dce-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41dce-116">Application</span></span>|<span data-ttu-id="41dce-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41dce-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="41dce-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41dce-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="41dce-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41dce-119">Request headers</span></span>
|<span data-ttu-id="41dce-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="41dce-120">Header</span></span>|<span data-ttu-id="41dce-121">Значение</span><span class="sxs-lookup"><span data-stu-id="41dce-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41dce-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41dce-122">Authorization</span></span>|<span data-ttu-id="41dce-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41dce-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41dce-124">Accept</span><span class="sxs-lookup"><span data-stu-id="41dce-124">Accept</span></span>|<span data-ttu-id="41dce-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41dce-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41dce-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41dce-126">Request body</span></span>
<span data-ttu-id="41dce-127">В тексте запроса добавьте представление объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41dce-127">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="41dce-128">В следующей таблице приведены свойства, необходимые при создании [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="41dce-128">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="41dce-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="41dce-129">Property</span></span>|<span data-ttu-id="41dce-130">Тип</span><span class="sxs-lookup"><span data-stu-id="41dce-130">Type</span></span>|<span data-ttu-id="41dce-131">Описание</span><span class="sxs-lookup"><span data-stu-id="41dce-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41dce-132">id</span><span class="sxs-lookup"><span data-stu-id="41dce-132">id</span></span>|<span data-ttu-id="41dce-133">Строка</span><span class="sxs-lookup"><span data-stu-id="41dce-133">String</span></span>|<span data-ttu-id="41dce-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="41dce-134">Key of the entity.</span></span> <span data-ttu-id="41dce-135">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="41dce-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="41dce-136">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="41dce-136">userEmailAddress</span></span>|<span data-ttu-id="41dce-137">String.</span><span class="sxs-lookup"><span data-stu-id="41dce-137">String</span></span>|<span data-ttu-id="41dce-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="41dce-138">The user email address.</span></span> <span data-ttu-id="41dce-139">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="41dce-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="41dce-140">userId</span><span class="sxs-lookup"><span data-stu-id="41dce-140">userId</span></span>|<span data-ttu-id="41dce-141">String</span><span class="sxs-lookup"><span data-stu-id="41dce-141">String</span></span>|<span data-ttu-id="41dce-142">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="41dce-142">The user ID.</span></span> <span data-ttu-id="41dce-143">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="41dce-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="41dce-144">userName</span><span class="sxs-lookup"><span data-stu-id="41dce-144">userName</span></span>|<span data-ttu-id="41dce-145">String</span><span class="sxs-lookup"><span data-stu-id="41dce-145">String</span></span>|<span data-ttu-id="41dce-146">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="41dce-146">The user name.</span></span> <span data-ttu-id="41dce-147">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="41dce-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="41dce-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="41dce-148">userPrincipalName</span></span>|<span data-ttu-id="41dce-149">Строка</span><span class="sxs-lookup"><span data-stu-id="41dce-149">String</span></span>|<span data-ttu-id="41dce-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="41dce-150">The user principal name.</span></span> <span data-ttu-id="41dce-151">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="41dce-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="41dce-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="41dce-152">Response</span></span>
<span data-ttu-id="41dce-153">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="41dce-153">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41dce-154">Пример</span><span class="sxs-lookup"><span data-stu-id="41dce-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="41dce-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="41dce-155">Request</span></span>
<span data-ttu-id="41dce-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41dce-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="41dce-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="41dce-157">Response</span></span>
<span data-ttu-id="41dce-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="41dce-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




