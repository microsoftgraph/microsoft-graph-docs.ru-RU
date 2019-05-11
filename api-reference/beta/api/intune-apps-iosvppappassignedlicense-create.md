---
title: Создание Иосвппаппассигнедлиценсе
description: Создание нового объекта Иосвппаппассигнедлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b42149e547c363f6677a9ecf7cd7ae7492405ec
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33936191"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="8b1de-103">Создание Иосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="8b1de-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="8b1de-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b1de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b1de-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b1de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b1de-106">Создание нового объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="8b1de-106">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b1de-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="8b1de-107">Prerequisites</span></span>
<span data-ttu-id="8b1de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b1de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b1de-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8b1de-110">Permission type</span></span>|<span data-ttu-id="8b1de-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="8b1de-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b1de-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8b1de-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b1de-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b1de-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8b1de-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8b1de-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b1de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b1de-115">Not supported.</span></span>|
|<span data-ttu-id="8b1de-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8b1de-116">Application</span></span>|<span data-ttu-id="8b1de-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b1de-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b1de-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8b1de-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="8b1de-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8b1de-119">Request headers</span></span>
|<span data-ttu-id="8b1de-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8b1de-120">Header</span></span>|<span data-ttu-id="8b1de-121">Значение</span><span class="sxs-lookup"><span data-stu-id="8b1de-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b1de-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8b1de-122">Authorization</span></span>|<span data-ttu-id="8b1de-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8b1de-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b1de-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8b1de-124">Accept</span></span>|<span data-ttu-id="8b1de-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b1de-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b1de-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8b1de-126">Request body</span></span>
<span data-ttu-id="8b1de-127">В тексте запроса добавьте представление объекта Иосвппаппассигнедлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b1de-127">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="8b1de-128">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнедлиценсе.</span><span class="sxs-lookup"><span data-stu-id="8b1de-128">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="8b1de-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b1de-129">Property</span></span>|<span data-ttu-id="8b1de-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8b1de-130">Type</span></span>|<span data-ttu-id="8b1de-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8b1de-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b1de-132">id</span><span class="sxs-lookup"><span data-stu-id="8b1de-132">id</span></span>|<span data-ttu-id="8b1de-133">Строка</span><span class="sxs-lookup"><span data-stu-id="8b1de-133">String</span></span>|<span data-ttu-id="8b1de-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="8b1de-134">Key of the entity.</span></span>|
|<span data-ttu-id="8b1de-135">Усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="8b1de-135">userEmailAddress</span></span>|<span data-ttu-id="8b1de-136">Строка</span><span class="sxs-lookup"><span data-stu-id="8b1de-136">String</span></span>|<span data-ttu-id="8b1de-137">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b1de-137">The user email address.</span></span>|
|<span data-ttu-id="8b1de-138">userId</span><span class="sxs-lookup"><span data-stu-id="8b1de-138">userId</span></span>|<span data-ttu-id="8b1de-139">String</span><span class="sxs-lookup"><span data-stu-id="8b1de-139">String</span></span>|<span data-ttu-id="8b1de-140">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b1de-140">The user ID.</span></span>|
|<span data-ttu-id="8b1de-141">userName</span><span class="sxs-lookup"><span data-stu-id="8b1de-141">userName</span></span>|<span data-ttu-id="8b1de-142">String</span><span class="sxs-lookup"><span data-stu-id="8b1de-142">String</span></span>|<span data-ttu-id="8b1de-143">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b1de-143">The user name.</span></span>|
|<span data-ttu-id="8b1de-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b1de-144">userPrincipalName</span></span>|<span data-ttu-id="8b1de-145">Строка</span><span class="sxs-lookup"><span data-stu-id="8b1de-145">String</span></span>|<span data-ttu-id="8b1de-146">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b1de-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="8b1de-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b1de-147">Response</span></span>
<span data-ttu-id="8b1de-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8b1de-148">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b1de-149">Пример</span><span class="sxs-lookup"><span data-stu-id="8b1de-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b1de-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="8b1de-150">Request</span></span>
<span data-ttu-id="8b1de-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8b1de-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8b1de-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8b1de-152">Response</span></span>
<span data-ttu-id="8b1de-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8b1de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




