---
title: Создание iosVppAppAssignedUserLicense
description: Создание нового объекта iosVppAppAssignedUserLicense.
author: tfitzmac
ms.openlocfilehash: 93b92d28a73e253eb598d03d3171318d95d3fd8a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308983"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="429a2-103">Создание iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="429a2-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="429a2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="429a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="429a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="429a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="429a2-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="429a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="429a2-107">Создание нового объекта [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="429a2-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="429a2-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="429a2-108">Prerequisites</span></span>
<span data-ttu-id="429a2-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="429a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="429a2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="429a2-111">Permission type</span></span>|<span data-ttu-id="429a2-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="429a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="429a2-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="429a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="429a2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="429a2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="429a2-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="429a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="429a2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="429a2-116">Not supported.</span></span>|
|<span data-ttu-id="429a2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="429a2-117">Application</span></span>|<span data-ttu-id="429a2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="429a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="429a2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="429a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="429a2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="429a2-120">Request headers</span></span>
|<span data-ttu-id="429a2-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="429a2-121">Header</span></span>|<span data-ttu-id="429a2-122">Значение</span><span class="sxs-lookup"><span data-stu-id="429a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="429a2-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="429a2-123">Authorization</span></span>|<span data-ttu-id="429a2-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="429a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="429a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="429a2-125">Accept</span></span>|<span data-ttu-id="429a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="429a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="429a2-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="429a2-127">Request body</span></span>
<span data-ttu-id="429a2-128">В тексте запроса укажите представление JSON для объекта iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="429a2-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="429a2-129">В следующей таблице показаны свойства, которые необходимы для создания iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="429a2-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="429a2-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="429a2-130">Property</span></span>|<span data-ttu-id="429a2-131">Тип</span><span class="sxs-lookup"><span data-stu-id="429a2-131">Type</span></span>|<span data-ttu-id="429a2-132">Описание</span><span class="sxs-lookup"><span data-stu-id="429a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="429a2-133">id</span><span class="sxs-lookup"><span data-stu-id="429a2-133">id</span></span>|<span data-ttu-id="429a2-134">Строка</span><span class="sxs-lookup"><span data-stu-id="429a2-134">String</span></span>|<span data-ttu-id="429a2-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="429a2-135">Key of the entity.</span></span> <span data-ttu-id="429a2-136">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="429a2-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="429a2-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="429a2-137">userEmailAddress</span></span>|<span data-ttu-id="429a2-138">String.</span><span class="sxs-lookup"><span data-stu-id="429a2-138">String</span></span>|<span data-ttu-id="429a2-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="429a2-139">The user email address.</span></span> <span data-ttu-id="429a2-140">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="429a2-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="429a2-141">userId</span><span class="sxs-lookup"><span data-stu-id="429a2-141">userId</span></span>|<span data-ttu-id="429a2-142">String</span><span class="sxs-lookup"><span data-stu-id="429a2-142">String</span></span>|<span data-ttu-id="429a2-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="429a2-143">The user ID.</span></span> <span data-ttu-id="429a2-144">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="429a2-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="429a2-145">userName</span><span class="sxs-lookup"><span data-stu-id="429a2-145">userName</span></span>|<span data-ttu-id="429a2-146">String</span><span class="sxs-lookup"><span data-stu-id="429a2-146">String</span></span>|<span data-ttu-id="429a2-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="429a2-147">The user name.</span></span> <span data-ttu-id="429a2-148">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="429a2-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="429a2-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="429a2-149">userPrincipalName</span></span>|<span data-ttu-id="429a2-150">Строка</span><span class="sxs-lookup"><span data-stu-id="429a2-150">String</span></span>|<span data-ttu-id="429a2-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="429a2-151">The user principal name.</span></span> <span data-ttu-id="429a2-152">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="429a2-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="429a2-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="429a2-153">Response</span></span>
<span data-ttu-id="429a2-154">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="429a2-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="429a2-155">Пример</span><span class="sxs-lookup"><span data-stu-id="429a2-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="429a2-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="429a2-156">Request</span></span>
<span data-ttu-id="429a2-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="429a2-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="429a2-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="429a2-158">Response</span></span>
<span data-ttu-id="429a2-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="429a2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





