---
title: Обновление Иосвппаппассигнедлиценсе
description: Обновление свойств объекта Иосвппаппассигнедлиценсе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 205d529c361b42dc13b55345260a9e00e7e85cba
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49251803"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="46e02-103">Обновление Иосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="46e02-103">Update iosVppAppAssignedLicense</span></span>

<span data-ttu-id="46e02-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46e02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46e02-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46e02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46e02-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46e02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46e02-107">Обновление свойств объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="46e02-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46e02-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="46e02-108">Prerequisites</span></span>
<span data-ttu-id="46e02-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46e02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46e02-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46e02-111">Permission type</span></span>|<span data-ttu-id="46e02-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="46e02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46e02-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46e02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46e02-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e02-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="46e02-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46e02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46e02-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46e02-116">Not supported.</span></span>|
|<span data-ttu-id="46e02-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="46e02-117">Application</span></span>|<span data-ttu-id="46e02-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46e02-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46e02-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46e02-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="46e02-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="46e02-120">Request headers</span></span>
|<span data-ttu-id="46e02-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="46e02-121">Header</span></span>|<span data-ttu-id="46e02-122">Значение</span><span class="sxs-lookup"><span data-stu-id="46e02-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46e02-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46e02-123">Authorization</span></span>|<span data-ttu-id="46e02-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46e02-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46e02-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46e02-125">Accept</span></span>|<span data-ttu-id="46e02-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46e02-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46e02-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46e02-127">Request body</span></span>
<span data-ttu-id="46e02-128">В тексте запроса добавьте представление объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46e02-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="46e02-129">В следующей таблице приведены свойства, необходимые при создании [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="46e02-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="46e02-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="46e02-130">Property</span></span>|<span data-ttu-id="46e02-131">Тип</span><span class="sxs-lookup"><span data-stu-id="46e02-131">Type</span></span>|<span data-ttu-id="46e02-132">Описание</span><span class="sxs-lookup"><span data-stu-id="46e02-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46e02-133">id</span><span class="sxs-lookup"><span data-stu-id="46e02-133">id</span></span>|<span data-ttu-id="46e02-134">String</span><span class="sxs-lookup"><span data-stu-id="46e02-134">String</span></span>|<span data-ttu-id="46e02-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="46e02-135">Key of the entity.</span></span>|
|<span data-ttu-id="46e02-136">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="46e02-136">userEmailAddress</span></span>|<span data-ttu-id="46e02-137">String</span><span class="sxs-lookup"><span data-stu-id="46e02-137">String</span></span>|<span data-ttu-id="46e02-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="46e02-138">The user email address.</span></span>|
|<span data-ttu-id="46e02-139">userId</span><span class="sxs-lookup"><span data-stu-id="46e02-139">userId</span></span>|<span data-ttu-id="46e02-140">String</span><span class="sxs-lookup"><span data-stu-id="46e02-140">String</span></span>|<span data-ttu-id="46e02-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="46e02-141">The user ID.</span></span>|
|<span data-ttu-id="46e02-142">userName</span><span class="sxs-lookup"><span data-stu-id="46e02-142">userName</span></span>|<span data-ttu-id="46e02-143">String</span><span class="sxs-lookup"><span data-stu-id="46e02-143">String</span></span>|<span data-ttu-id="46e02-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="46e02-144">The user name.</span></span>|
|<span data-ttu-id="46e02-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46e02-145">userPrincipalName</span></span>|<span data-ttu-id="46e02-146">String</span><span class="sxs-lookup"><span data-stu-id="46e02-146">String</span></span>|<span data-ttu-id="46e02-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="46e02-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="46e02-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="46e02-148">Response</span></span>
<span data-ttu-id="46e02-149">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="46e02-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46e02-150">Пример</span><span class="sxs-lookup"><span data-stu-id="46e02-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="46e02-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="46e02-151">Request</span></span>
<span data-ttu-id="46e02-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46e02-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="46e02-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="46e02-153">Response</span></span>
<span data-ttu-id="46e02-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46e02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




