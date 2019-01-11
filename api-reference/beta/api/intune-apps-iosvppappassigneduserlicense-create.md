---
title: Создание iosVppAppAssignedUserLicense
description: Создание нового объекта iosVppAppAssignedUserLicense.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2e6178570da6e89ef50c933d027daa2a9d7e1adf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864654"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="e91fc-103">Создание iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="e91fc-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="e91fc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e91fc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e91fc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e91fc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e91fc-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e91fc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e91fc-107">Создание нового объекта [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="e91fc-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e91fc-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="e91fc-108">Prerequisites</span></span>
<span data-ttu-id="e91fc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e91fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e91fc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e91fc-111">Permission type</span></span>|<span data-ttu-id="e91fc-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="e91fc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e91fc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e91fc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e91fc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e91fc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e91fc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e91fc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e91fc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e91fc-116">Not supported.</span></span>|
|<span data-ttu-id="e91fc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e91fc-117">Application</span></span>|<span data-ttu-id="e91fc-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e91fc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e91fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e91fc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="e91fc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e91fc-120">Request headers</span></span>
|<span data-ttu-id="e91fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e91fc-121">Header</span></span>|<span data-ttu-id="e91fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="e91fc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e91fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e91fc-123">Authorization</span></span>|<span data-ttu-id="e91fc-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="e91fc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e91fc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e91fc-125">Accept</span></span>|<span data-ttu-id="e91fc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e91fc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e91fc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e91fc-127">Request body</span></span>
<span data-ttu-id="e91fc-128">В тексте запроса укажите представление JSON для объекта iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="e91fc-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="e91fc-129">В следующей таблице показаны свойства, которые необходимы для создания iosVppAppAssignedUserLicense.</span><span class="sxs-lookup"><span data-stu-id="e91fc-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="e91fc-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e91fc-130">Property</span></span>|<span data-ttu-id="e91fc-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e91fc-131">Type</span></span>|<span data-ttu-id="e91fc-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e91fc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e91fc-133">id</span><span class="sxs-lookup"><span data-stu-id="e91fc-133">id</span></span>|<span data-ttu-id="e91fc-134">Строка</span><span class="sxs-lookup"><span data-stu-id="e91fc-134">String</span></span>|<span data-ttu-id="e91fc-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e91fc-135">Key of the entity.</span></span> <span data-ttu-id="e91fc-136">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e91fc-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e91fc-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e91fc-137">userEmailAddress</span></span>|<span data-ttu-id="e91fc-138">Строка</span><span class="sxs-lookup"><span data-stu-id="e91fc-138">String</span></span>|<span data-ttu-id="e91fc-139">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="e91fc-139">The user email address.</span></span> <span data-ttu-id="e91fc-140">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e91fc-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e91fc-141">userId</span><span class="sxs-lookup"><span data-stu-id="e91fc-141">userId</span></span>|<span data-ttu-id="e91fc-142">String</span><span class="sxs-lookup"><span data-stu-id="e91fc-142">String</span></span>|<span data-ttu-id="e91fc-143">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="e91fc-143">The user ID.</span></span> <span data-ttu-id="e91fc-144">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e91fc-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e91fc-145">userName</span><span class="sxs-lookup"><span data-stu-id="e91fc-145">userName</span></span>|<span data-ttu-id="e91fc-146">String</span><span class="sxs-lookup"><span data-stu-id="e91fc-146">String</span></span>|<span data-ttu-id="e91fc-147">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="e91fc-147">The user name.</span></span> <span data-ttu-id="e91fc-148">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e91fc-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="e91fc-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e91fc-149">userPrincipalName</span></span>|<span data-ttu-id="e91fc-150">Строка</span><span class="sxs-lookup"><span data-stu-id="e91fc-150">String</span></span>|<span data-ttu-id="e91fc-151">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="e91fc-151">The user principal name.</span></span> <span data-ttu-id="e91fc-152">Наследуется от [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="e91fc-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="e91fc-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="e91fc-153">Response</span></span>
<span data-ttu-id="e91fc-154">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e91fc-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e91fc-155">Пример</span><span class="sxs-lookup"><span data-stu-id="e91fc-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="e91fc-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="e91fc-156">Request</span></span>
<span data-ttu-id="e91fc-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e91fc-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e91fc-158">Ответ</span><span class="sxs-lookup"><span data-stu-id="e91fc-158">Response</span></span>
<span data-ttu-id="e91fc-p108">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="e91fc-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





