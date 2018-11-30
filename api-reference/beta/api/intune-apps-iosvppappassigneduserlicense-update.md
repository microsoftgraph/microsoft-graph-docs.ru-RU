---
title: Обновление iosVppAppAssignedUserLicense
description: Обновление свойства объекта iosVppAppAssignedUserLicense.
ms.openlocfilehash: 4374a2288c633da47773c827fc47a6e3ef0ee1d1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082660"
---
# <a name="update-iosvppappassigneduserlicense"></a><span data-ttu-id="22326-103">Обновление iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="22326-103">Update iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="22326-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22326-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22326-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22326-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22326-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="22326-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22326-107">Обновление свойства объекта [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="22326-107">Update the properties of a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22326-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="22326-108">Prerequisites</span></span>
<span data-ttu-id="22326-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22326-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22326-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="22326-111">Permission type</span></span>|<span data-ttu-id="22326-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="22326-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22326-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="22326-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22326-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22326-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22326-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="22326-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22326-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22326-116">Not supported.</span></span>|
|<span data-ttu-id="22326-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="22326-117">Application</span></span>|<span data-ttu-id="22326-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22326-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22326-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="22326-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="22326-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="22326-120">Request headers</span></span>
|<span data-ttu-id="22326-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="22326-121">Header</span></span>|<span data-ttu-id="22326-122">Значение</span><span class="sxs-lookup"><span data-stu-id="22326-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22326-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22326-123">Authorization</span></span>|<span data-ttu-id="22326-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="22326-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22326-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22326-125">Accept</span></span>|<span data-ttu-id="22326-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22326-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22326-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="22326-127">Request body</span></span>
<span data-ttu-id="22326-128">В тексте запроса укажите представление JSON для объекта [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="22326-128">In the request body, supply a JSON representation for the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

<span data-ttu-id="22326-129">В следующей таблице показаны свойства, которые необходимы для создания [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span><span class="sxs-lookup"><span data-stu-id="22326-129">The following table shows the properties that are required when you create the [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).</span></span>

|<span data-ttu-id="22326-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="22326-130">Property</span></span>|<span data-ttu-id="22326-131">Тип</span><span class="sxs-lookup"><span data-stu-id="22326-131">Type</span></span>|<span data-ttu-id="22326-132">Описание</span><span class="sxs-lookup"><span data-stu-id="22326-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22326-133">id</span><span class="sxs-lookup"><span data-stu-id="22326-133">id</span></span>|<span data-ttu-id="22326-134">String</span><span class="sxs-lookup"><span data-stu-id="22326-134">String</span></span>|<span data-ttu-id="22326-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="22326-135">Key of the entity.</span></span> <span data-ttu-id="22326-136">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="22326-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="22326-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="22326-137">userEmailAddress</span></span>|<span data-ttu-id="22326-138">String</span><span class="sxs-lookup"><span data-stu-id="22326-138">String</span></span>|<span data-ttu-id="22326-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="22326-139">The user email address.</span></span> <span data-ttu-id="22326-140">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="22326-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="22326-141">userId</span><span class="sxs-lookup"><span data-stu-id="22326-141">userId</span></span>|<span data-ttu-id="22326-142">String</span><span class="sxs-lookup"><span data-stu-id="22326-142">String</span></span>|<span data-ttu-id="22326-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="22326-143">The user ID.</span></span> <span data-ttu-id="22326-144">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="22326-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="22326-145">userName</span><span class="sxs-lookup"><span data-stu-id="22326-145">userName</span></span>|<span data-ttu-id="22326-146">String</span><span class="sxs-lookup"><span data-stu-id="22326-146">String</span></span>|<span data-ttu-id="22326-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="22326-147">The user name.</span></span> <span data-ttu-id="22326-148">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="22326-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="22326-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="22326-149">userPrincipalName</span></span>|<span data-ttu-id="22326-150">String</span><span class="sxs-lookup"><span data-stu-id="22326-150">String</span></span>|<span data-ttu-id="22326-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="22326-151">The user principal name.</span></span> <span data-ttu-id="22326-152">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="22326-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="22326-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="22326-153">Response</span></span>
<span data-ttu-id="22326-154">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="22326-154">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22326-155">Пример</span><span class="sxs-lookup"><span data-stu-id="22326-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="22326-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="22326-156">Request</span></span>
<span data-ttu-id="22326-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="22326-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
Content-type: application/json
Content-length: 171

{
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="22326-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="22326-158">Response</span></span>
<span data-ttu-id="22326-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="22326-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





