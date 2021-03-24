---
title: Обновление iosVppAppAssignedLicense
description: Обновление свойств объекта iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d8fc793f48d718af7a3cbc1ffa4dada36766df97
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144020"
---
# <a name="update-iosvppappassignedlicense"></a><span data-ttu-id="51f9d-103">Обновление iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="51f9d-103">Update iosVppAppAssignedLicense</span></span>

<span data-ttu-id="51f9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51f9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51f9d-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51f9d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51f9d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51f9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51f9d-107">Обновление свойств объекта [iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="51f9d-107">Update the properties of a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51f9d-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51f9d-108">Prerequisites</span></span>
<span data-ttu-id="51f9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51f9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51f9d-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51f9d-111">Permission type</span></span>|<span data-ttu-id="51f9d-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="51f9d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51f9d-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51f9d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51f9d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51f9d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51f9d-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51f9d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51f9d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51f9d-116">Not supported.</span></span>|
|<span data-ttu-id="51f9d-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="51f9d-117">Application</span></span>|<span data-ttu-id="51f9d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51f9d-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51f9d-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51f9d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="51f9d-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51f9d-120">Request headers</span></span>
|<span data-ttu-id="51f9d-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51f9d-121">Header</span></span>|<span data-ttu-id="51f9d-122">Значение</span><span class="sxs-lookup"><span data-stu-id="51f9d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51f9d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51f9d-123">Authorization</span></span>|<span data-ttu-id="51f9d-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51f9d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51f9d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51f9d-125">Accept</span></span>|<span data-ttu-id="51f9d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51f9d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51f9d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51f9d-127">Request body</span></span>
<span data-ttu-id="51f9d-128">В теле запроса поставляем представление JSON для [объекта iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="51f9d-128">In the request body, supply a JSON representation for the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="51f9d-129">В следующей таблице показаны свойства, необходимые при создании [iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="51f9d-129">The following table shows the properties that are required when you create the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="51f9d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="51f9d-130">Property</span></span>|<span data-ttu-id="51f9d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="51f9d-131">Type</span></span>|<span data-ttu-id="51f9d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="51f9d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51f9d-133">id</span><span class="sxs-lookup"><span data-stu-id="51f9d-133">id</span></span>|<span data-ttu-id="51f9d-134">Строка</span><span class="sxs-lookup"><span data-stu-id="51f9d-134">String</span></span>|<span data-ttu-id="51f9d-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="51f9d-135">Key of the entity.</span></span>|
|<span data-ttu-id="51f9d-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="51f9d-136">userEmailAddress</span></span>|<span data-ttu-id="51f9d-137">Строка</span><span class="sxs-lookup"><span data-stu-id="51f9d-137">String</span></span>|<span data-ttu-id="51f9d-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="51f9d-138">The user email address.</span></span>|
|<span data-ttu-id="51f9d-139">userId</span><span class="sxs-lookup"><span data-stu-id="51f9d-139">userId</span></span>|<span data-ttu-id="51f9d-140">String</span><span class="sxs-lookup"><span data-stu-id="51f9d-140">String</span></span>|<span data-ttu-id="51f9d-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="51f9d-141">The user ID.</span></span>|
|<span data-ttu-id="51f9d-142">userName</span><span class="sxs-lookup"><span data-stu-id="51f9d-142">userName</span></span>|<span data-ttu-id="51f9d-143">String</span><span class="sxs-lookup"><span data-stu-id="51f9d-143">String</span></span>|<span data-ttu-id="51f9d-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="51f9d-144">The user name.</span></span>|
|<span data-ttu-id="51f9d-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="51f9d-145">userPrincipalName</span></span>|<span data-ttu-id="51f9d-146">String</span><span class="sxs-lookup"><span data-stu-id="51f9d-146">String</span></span>|<span data-ttu-id="51f9d-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="51f9d-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="51f9d-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="51f9d-148">Response</span></span>
<span data-ttu-id="51f9d-149">В случае успеха этот метод возвращает код отклика и обновленный `200 OK` [объект iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="51f9d-149">If successful, this method returns a `200 OK` response code and an updated [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51f9d-150">Пример</span><span class="sxs-lookup"><span data-stu-id="51f9d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="51f9d-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="51f9d-151">Request</span></span>
<span data-ttu-id="51f9d-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51f9d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51f9d-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="51f9d-153">Response</span></span>
<span data-ttu-id="51f9d-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51f9d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




