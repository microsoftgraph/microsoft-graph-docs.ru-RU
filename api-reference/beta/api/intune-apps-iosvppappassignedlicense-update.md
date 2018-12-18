---
title: Обновление iosVppAppAssignedLicense
description: Обновление свойства объекта iosVppAppAssignedLicense.
author: tfitzmac
ms.openlocfilehash: e15aba6cf5ca5225210e946f04a6b1bff82cdd83
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322325"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="0e80b-103">Обновление iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="0e80b-103">Update iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="0e80b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0e80b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e80b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e80b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e80b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0e80b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e80b-107">Обновление свойства объекта [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="0e80b-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e80b-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="0e80b-108">Prerequisites</span></span>
<span data-ttu-id="0e80b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e80b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e80b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e80b-111">Permission type</span></span>|<span data-ttu-id="0e80b-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e80b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e80b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e80b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e80b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e80b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e80b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e80b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e80b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e80b-116">Not supported.</span></span>|
|<span data-ttu-id="0e80b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e80b-117">Application</span></span>|<span data-ttu-id="0e80b-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e80b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e80b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e80b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="0e80b-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e80b-120">Request headers</span></span>
|<span data-ttu-id="0e80b-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0e80b-121">Header</span></span>|<span data-ttu-id="0e80b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0e80b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e80b-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e80b-123">Authorization</span></span>|<span data-ttu-id="0e80b-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0e80b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e80b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e80b-125">Accept</span></span>|<span data-ttu-id="0e80b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e80b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e80b-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e80b-127">Request body</span></span>
<span data-ttu-id="0e80b-128">В тексте запроса укажите представление JSON для объекта [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="0e80b-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="0e80b-129">В следующей таблице показаны свойства, которые необходимы для создания [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="0e80b-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="0e80b-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0e80b-130">Property</span></span>|<span data-ttu-id="0e80b-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0e80b-131">Type</span></span>|<span data-ttu-id="0e80b-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0e80b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e80b-133">id</span><span class="sxs-lookup"><span data-stu-id="0e80b-133">id</span></span>|<span data-ttu-id="0e80b-134">Строка</span><span class="sxs-lookup"><span data-stu-id="0e80b-134">String</span></span>|<span data-ttu-id="0e80b-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0e80b-135">Key of the entity.</span></span>|
|<span data-ttu-id="0e80b-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="0e80b-136">userEmailAddress</span></span>|<span data-ttu-id="0e80b-137">String.</span><span class="sxs-lookup"><span data-stu-id="0e80b-137">String</span></span>|<span data-ttu-id="0e80b-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e80b-138">The user email address.</span></span>|
|<span data-ttu-id="0e80b-139">userId</span><span class="sxs-lookup"><span data-stu-id="0e80b-139">userId</span></span>|<span data-ttu-id="0e80b-140">String</span><span class="sxs-lookup"><span data-stu-id="0e80b-140">String</span></span>|<span data-ttu-id="0e80b-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e80b-141">The user ID.</span></span>|
|<span data-ttu-id="0e80b-142">userName</span><span class="sxs-lookup"><span data-stu-id="0e80b-142">userName</span></span>|<span data-ttu-id="0e80b-143">String</span><span class="sxs-lookup"><span data-stu-id="0e80b-143">String</span></span>|<span data-ttu-id="0e80b-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e80b-144">The user name.</span></span>|
|<span data-ttu-id="0e80b-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0e80b-145">userPrincipalName</span></span>|<span data-ttu-id="0e80b-146">Строка</span><span class="sxs-lookup"><span data-stu-id="0e80b-146">String</span></span>|<span data-ttu-id="0e80b-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="0e80b-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="0e80b-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e80b-148">Response</span></span>
<span data-ttu-id="0e80b-149">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0e80b-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e80b-150">Пример</span><span class="sxs-lookup"><span data-stu-id="0e80b-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e80b-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e80b-151">Request</span></span>
<span data-ttu-id="0e80b-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0e80b-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0e80b-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="0e80b-153">Response</span></span>
<span data-ttu-id="0e80b-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0e80b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 283

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```





