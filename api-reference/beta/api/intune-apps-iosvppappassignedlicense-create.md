---
title: Создание iosVppAppAssignedLicense
description: Создание нового объекта iosVppAppAssignedLicense.
author: tfitzmac
ms.openlocfilehash: a77ac7d98df2dc99555603e83adb5d09e5e14a3f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304643"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="40500-103">Создание iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="40500-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="40500-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="40500-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40500-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40500-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40500-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="40500-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="40500-107">Создание нового объекта [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="40500-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="40500-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="40500-108">Prerequisites</span></span>
<span data-ttu-id="40500-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40500-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40500-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="40500-111">Permission type</span></span>|<span data-ttu-id="40500-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="40500-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40500-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="40500-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40500-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40500-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40500-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="40500-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40500-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40500-116">Not supported.</span></span>|
|<span data-ttu-id="40500-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="40500-117">Application</span></span>|<span data-ttu-id="40500-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40500-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40500-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="40500-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="40500-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="40500-120">Request headers</span></span>
|<span data-ttu-id="40500-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="40500-121">Header</span></span>|<span data-ttu-id="40500-122">Значение</span><span class="sxs-lookup"><span data-stu-id="40500-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40500-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="40500-123">Authorization</span></span>|<span data-ttu-id="40500-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="40500-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40500-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40500-125">Accept</span></span>|<span data-ttu-id="40500-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40500-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40500-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="40500-127">Request body</span></span>
<span data-ttu-id="40500-128">В тексте запроса укажите представление JSON для объекта iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="40500-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="40500-129">В следующей таблице показаны свойства, которые необходимы для создания iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="40500-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="40500-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="40500-130">Property</span></span>|<span data-ttu-id="40500-131">Тип</span><span class="sxs-lookup"><span data-stu-id="40500-131">Type</span></span>|<span data-ttu-id="40500-132">Описание</span><span class="sxs-lookup"><span data-stu-id="40500-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40500-133">id</span><span class="sxs-lookup"><span data-stu-id="40500-133">id</span></span>|<span data-ttu-id="40500-134">Строка</span><span class="sxs-lookup"><span data-stu-id="40500-134">String</span></span>|<span data-ttu-id="40500-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="40500-135">Key of the entity.</span></span>|
|<span data-ttu-id="40500-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="40500-136">userEmailAddress</span></span>|<span data-ttu-id="40500-137">String.</span><span class="sxs-lookup"><span data-stu-id="40500-137">String</span></span>|<span data-ttu-id="40500-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="40500-138">The user email address.</span></span>|
|<span data-ttu-id="40500-139">userId</span><span class="sxs-lookup"><span data-stu-id="40500-139">userId</span></span>|<span data-ttu-id="40500-140">String</span><span class="sxs-lookup"><span data-stu-id="40500-140">String</span></span>|<span data-ttu-id="40500-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="40500-141">The user ID.</span></span>|
|<span data-ttu-id="40500-142">userName</span><span class="sxs-lookup"><span data-stu-id="40500-142">userName</span></span>|<span data-ttu-id="40500-143">String</span><span class="sxs-lookup"><span data-stu-id="40500-143">String</span></span>|<span data-ttu-id="40500-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="40500-144">The user name.</span></span>|
|<span data-ttu-id="40500-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="40500-145">userPrincipalName</span></span>|<span data-ttu-id="40500-146">Строка</span><span class="sxs-lookup"><span data-stu-id="40500-146">String</span></span>|<span data-ttu-id="40500-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="40500-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="40500-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="40500-148">Response</span></span>
<span data-ttu-id="40500-149">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="40500-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40500-150">Пример</span><span class="sxs-lookup"><span data-stu-id="40500-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="40500-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="40500-151">Request</span></span>
<span data-ttu-id="40500-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="40500-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
Content-type: application/json
Content-length: 234

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="40500-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="40500-153">Response</span></span>
<span data-ttu-id="40500-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="40500-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





