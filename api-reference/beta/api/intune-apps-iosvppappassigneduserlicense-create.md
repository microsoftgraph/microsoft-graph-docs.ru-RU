---
title: Создание Иосвппаппассигнедусерлиценсе
description: Создание нового объекта Иосвппаппассигнедусерлиценсе.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1adad9b8251069fcc6e14ef15f756337d38f502f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761848"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="9103e-103">Создание Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="9103e-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="9103e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9103e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9103e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9103e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9103e-106">Создание нового объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="9103e-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9103e-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="9103e-107">Prerequisites</span></span>
<span data-ttu-id="9103e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9103e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9103e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9103e-110">Permission type</span></span>|<span data-ttu-id="9103e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9103e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9103e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9103e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9103e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9103e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9103e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9103e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9103e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9103e-115">Not supported.</span></span>|
|<span data-ttu-id="9103e-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9103e-116">Application</span></span>|<span data-ttu-id="9103e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9103e-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9103e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9103e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="9103e-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="9103e-119">Request headers</span></span>
|<span data-ttu-id="9103e-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9103e-120">Header</span></span>|<span data-ttu-id="9103e-121">Значение</span><span class="sxs-lookup"><span data-stu-id="9103e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9103e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9103e-122">Authorization</span></span>|<span data-ttu-id="9103e-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9103e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9103e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9103e-124">Accept</span></span>|<span data-ttu-id="9103e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9103e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9103e-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9103e-126">Request body</span></span>
<span data-ttu-id="9103e-127">В тексте запроса добавьте представление объекта Иосвппаппассигнедусерлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9103e-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="9103e-128">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнедусерлиценсе.</span><span class="sxs-lookup"><span data-stu-id="9103e-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="9103e-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="9103e-129">Property</span></span>|<span data-ttu-id="9103e-130">Тип</span><span class="sxs-lookup"><span data-stu-id="9103e-130">Type</span></span>|<span data-ttu-id="9103e-131">Описание</span><span class="sxs-lookup"><span data-stu-id="9103e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9103e-132">id</span><span class="sxs-lookup"><span data-stu-id="9103e-132">id</span></span>|<span data-ttu-id="9103e-133">Строка</span><span class="sxs-lookup"><span data-stu-id="9103e-133">String</span></span>|<span data-ttu-id="9103e-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="9103e-134">Key of the entity.</span></span> <span data-ttu-id="9103e-135">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="9103e-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="9103e-136">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="9103e-136">userEmailAddress</span></span>|<span data-ttu-id="9103e-137">String</span><span class="sxs-lookup"><span data-stu-id="9103e-137">String</span></span>|<span data-ttu-id="9103e-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="9103e-138">The user email address.</span></span> <span data-ttu-id="9103e-139">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="9103e-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="9103e-140">userId</span><span class="sxs-lookup"><span data-stu-id="9103e-140">userId</span></span>|<span data-ttu-id="9103e-141">String</span><span class="sxs-lookup"><span data-stu-id="9103e-141">String</span></span>|<span data-ttu-id="9103e-142">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="9103e-142">The user ID.</span></span> <span data-ttu-id="9103e-143">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="9103e-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="9103e-144">userName</span><span class="sxs-lookup"><span data-stu-id="9103e-144">userName</span></span>|<span data-ttu-id="9103e-145">String</span><span class="sxs-lookup"><span data-stu-id="9103e-145">String</span></span>|<span data-ttu-id="9103e-146">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="9103e-146">The user name.</span></span> <span data-ttu-id="9103e-147">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="9103e-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="9103e-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="9103e-148">userPrincipalName</span></span>|<span data-ttu-id="9103e-149">Строка</span><span class="sxs-lookup"><span data-stu-id="9103e-149">String</span></span>|<span data-ttu-id="9103e-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="9103e-150">The user principal name.</span></span> <span data-ttu-id="9103e-151">Наследуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="9103e-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9103e-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="9103e-152">Response</span></span>
<span data-ttu-id="9103e-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9103e-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9103e-154">Пример</span><span class="sxs-lookup"><span data-stu-id="9103e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="9103e-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="9103e-155">Request</span></span>
<span data-ttu-id="9103e-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9103e-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9103e-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="9103e-157">Response</span></span>
<span data-ttu-id="9103e-p107">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9103e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




