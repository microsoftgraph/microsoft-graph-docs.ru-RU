---
title: Создание Иосвппаппассигнедлиценсе
description: Создание нового объекта Иосвппаппассигнедлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 73a25e6f217f287811be7ce7b3a459c36727f1dc
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173488"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="39ce8-103">Создание Иосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="39ce8-103">Create iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="39ce8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39ce8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39ce8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="39ce8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39ce8-106">Создание нового объекта [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="39ce8-106">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="39ce8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="39ce8-107">Prerequisites</span></span>
<span data-ttu-id="39ce8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39ce8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39ce8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39ce8-110">Permission type</span></span>|<span data-ttu-id="39ce8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="39ce8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39ce8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39ce8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="39ce8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39ce8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39ce8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39ce8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39ce8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39ce8-115">Not supported.</span></span>|
|<span data-ttu-id="39ce8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39ce8-116">Application</span></span>|<span data-ttu-id="39ce8-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39ce8-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="39ce8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39ce8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="39ce8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39ce8-119">Request headers</span></span>
|<span data-ttu-id="39ce8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="39ce8-120">Header</span></span>|<span data-ttu-id="39ce8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="39ce8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39ce8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39ce8-122">Authorization</span></span>|<span data-ttu-id="39ce8-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39ce8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39ce8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="39ce8-124">Accept</span></span>|<span data-ttu-id="39ce8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="39ce8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39ce8-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39ce8-126">Request body</span></span>
<span data-ttu-id="39ce8-127">В тексте запроса добавьте представление объекта Иосвппаппассигнедлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="39ce8-127">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="39ce8-128">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнедлиценсе.</span><span class="sxs-lookup"><span data-stu-id="39ce8-128">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="39ce8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="39ce8-129">Property</span></span>|<span data-ttu-id="39ce8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="39ce8-130">Type</span></span>|<span data-ttu-id="39ce8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="39ce8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ce8-132">id</span><span class="sxs-lookup"><span data-stu-id="39ce8-132">id</span></span>|<span data-ttu-id="39ce8-133">Строка</span><span class="sxs-lookup"><span data-stu-id="39ce8-133">String</span></span>|<span data-ttu-id="39ce8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="39ce8-134">Key of the entity.</span></span>|
|<span data-ttu-id="39ce8-135">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="39ce8-135">userEmailAddress</span></span>|<span data-ttu-id="39ce8-136">String.</span><span class="sxs-lookup"><span data-stu-id="39ce8-136">String</span></span>|<span data-ttu-id="39ce8-137">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="39ce8-137">The user email address.</span></span>|
|<span data-ttu-id="39ce8-138">userId</span><span class="sxs-lookup"><span data-stu-id="39ce8-138">userId</span></span>|<span data-ttu-id="39ce8-139">String</span><span class="sxs-lookup"><span data-stu-id="39ce8-139">String</span></span>|<span data-ttu-id="39ce8-140">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="39ce8-140">The user ID.</span></span>|
|<span data-ttu-id="39ce8-141">userName</span><span class="sxs-lookup"><span data-stu-id="39ce8-141">userName</span></span>|<span data-ttu-id="39ce8-142">String</span><span class="sxs-lookup"><span data-stu-id="39ce8-142">String</span></span>|<span data-ttu-id="39ce8-143">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="39ce8-143">The user name.</span></span>|
|<span data-ttu-id="39ce8-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="39ce8-144">userPrincipalName</span></span>|<span data-ttu-id="39ce8-145">Строка</span><span class="sxs-lookup"><span data-stu-id="39ce8-145">String</span></span>|<span data-ttu-id="39ce8-146">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="39ce8-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="39ce8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="39ce8-147">Response</span></span>
<span data-ttu-id="39ce8-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39ce8-148">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39ce8-149">Пример</span><span class="sxs-lookup"><span data-stu-id="39ce8-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="39ce8-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="39ce8-150">Request</span></span>
<span data-ttu-id="39ce8-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39ce8-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="39ce8-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="39ce8-152">Response</span></span>
<span data-ttu-id="39ce8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39ce8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




