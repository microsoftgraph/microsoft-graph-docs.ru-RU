---
title: Создание Иосвппаппассигнедлиценсе
description: Создание нового объекта Иосвппаппассигнедлиценсе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3142f583f9ec87ba0aa176453c990e73458ca007
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48700068"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="dfbbd-103">Создание Иосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="dfbbd-103">Create iosVppAppAssignedLicense</span></span>

<span data-ttu-id="dfbbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfbbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfbbd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfbbd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfbbd-107">Создание нового объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="dfbbd-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfbbd-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="dfbbd-108">Prerequisites</span></span>
<span data-ttu-id="dfbbd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfbbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfbbd-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dfbbd-111">Permission type</span></span>|<span data-ttu-id="dfbbd-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="dfbbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfbbd-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dfbbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dfbbd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfbbd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dfbbd-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dfbbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfbbd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-116">Not supported.</span></span>|
|<span data-ttu-id="dfbbd-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dfbbd-117">Application</span></span>|<span data-ttu-id="dfbbd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfbbd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfbbd-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dfbbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="dfbbd-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="dfbbd-120">Request headers</span></span>
|<span data-ttu-id="dfbbd-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dfbbd-121">Header</span></span>|<span data-ttu-id="dfbbd-122">Значение</span><span class="sxs-lookup"><span data-stu-id="dfbbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfbbd-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dfbbd-123">Authorization</span></span>|<span data-ttu-id="dfbbd-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfbbd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dfbbd-125">Accept</span></span>|<span data-ttu-id="dfbbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dfbbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfbbd-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="dfbbd-127">Request body</span></span>
<span data-ttu-id="dfbbd-128">В тексте запроса добавьте представление объекта Иосвппаппассигнедлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="dfbbd-129">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнедлиценсе.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="dfbbd-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfbbd-130">Property</span></span>|<span data-ttu-id="dfbbd-131">Тип</span><span class="sxs-lookup"><span data-stu-id="dfbbd-131">Type</span></span>|<span data-ttu-id="dfbbd-132">Описание</span><span class="sxs-lookup"><span data-stu-id="dfbbd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfbbd-133">id</span><span class="sxs-lookup"><span data-stu-id="dfbbd-133">id</span></span>|<span data-ttu-id="dfbbd-134">Строка</span><span class="sxs-lookup"><span data-stu-id="dfbbd-134">String</span></span>|<span data-ttu-id="dfbbd-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-135">Key of the entity.</span></span>|
|<span data-ttu-id="dfbbd-136">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="dfbbd-136">userEmailAddress</span></span>|<span data-ttu-id="dfbbd-137">Строка</span><span class="sxs-lookup"><span data-stu-id="dfbbd-137">String</span></span>|<span data-ttu-id="dfbbd-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-138">The user email address.</span></span>|
|<span data-ttu-id="dfbbd-139">userId</span><span class="sxs-lookup"><span data-stu-id="dfbbd-139">userId</span></span>|<span data-ttu-id="dfbbd-140">String</span><span class="sxs-lookup"><span data-stu-id="dfbbd-140">String</span></span>|<span data-ttu-id="dfbbd-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-141">The user ID.</span></span>|
|<span data-ttu-id="dfbbd-142">userName</span><span class="sxs-lookup"><span data-stu-id="dfbbd-142">userName</span></span>|<span data-ttu-id="dfbbd-143">String</span><span class="sxs-lookup"><span data-stu-id="dfbbd-143">String</span></span>|<span data-ttu-id="dfbbd-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-144">The user name.</span></span>|
|<span data-ttu-id="dfbbd-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dfbbd-145">userPrincipalName</span></span>|<span data-ttu-id="dfbbd-146">String</span><span class="sxs-lookup"><span data-stu-id="dfbbd-146">String</span></span>|<span data-ttu-id="dfbbd-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="dfbbd-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="dfbbd-148">Response</span></span>
<span data-ttu-id="dfbbd-149">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfbbd-150">Пример</span><span class="sxs-lookup"><span data-stu-id="dfbbd-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfbbd-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="dfbbd-151">Request</span></span>
<span data-ttu-id="dfbbd-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dfbbd-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="dfbbd-153">Response</span></span>
<span data-ttu-id="dfbbd-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dfbbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





