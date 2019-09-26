---
title: Создание Макосвппаппассигнедлиценсе
description: Создание нового объекта Макосвппаппассигнедлиценсе.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2f4620465b30cca525faf0fb3e58b4205befad23
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37173278"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="ede36-103">Создание Макосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="ede36-103">Create macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="ede36-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ede36-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ede36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ede36-106">Создание нового объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="ede36-106">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ede36-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="ede36-107">Prerequisites</span></span>
<span data-ttu-id="ede36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ede36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ede36-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ede36-110">Permission type</span></span>|<span data-ttu-id="ede36-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ede36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ede36-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ede36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ede36-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ede36-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ede36-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ede36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ede36-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede36-115">Not supported.</span></span>|
|<span data-ttu-id="ede36-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ede36-116">Application</span></span>|<span data-ttu-id="ede36-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ede36-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ede36-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ede36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="ede36-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ede36-119">Request headers</span></span>
|<span data-ttu-id="ede36-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ede36-120">Header</span></span>|<span data-ttu-id="ede36-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ede36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ede36-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ede36-122">Authorization</span></span>|<span data-ttu-id="ede36-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ede36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ede36-124">Accept</span><span class="sxs-lookup"><span data-stu-id="ede36-124">Accept</span></span>|<span data-ttu-id="ede36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ede36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ede36-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ede36-126">Request body</span></span>
<span data-ttu-id="ede36-127">В тексте запроса добавьте представление объекта Макосвппаппассигнедлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ede36-127">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="ede36-128">В следующей таблице приведены свойства, необходимые при создании Макосвппаппассигнедлиценсе.</span><span class="sxs-lookup"><span data-stu-id="ede36-128">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="ede36-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="ede36-129">Property</span></span>|<span data-ttu-id="ede36-130">Тип</span><span class="sxs-lookup"><span data-stu-id="ede36-130">Type</span></span>|<span data-ttu-id="ede36-131">Описание</span><span class="sxs-lookup"><span data-stu-id="ede36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ede36-132">id</span><span class="sxs-lookup"><span data-stu-id="ede36-132">id</span></span>|<span data-ttu-id="ede36-133">Строка</span><span class="sxs-lookup"><span data-stu-id="ede36-133">String</span></span>|<span data-ttu-id="ede36-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="ede36-134">Key of the entity.</span></span>|
|<span data-ttu-id="ede36-135">усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="ede36-135">userEmailAddress</span></span>|<span data-ttu-id="ede36-136">String.</span><span class="sxs-lookup"><span data-stu-id="ede36-136">String</span></span>|<span data-ttu-id="ede36-137">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="ede36-137">The user email address.</span></span>|
|<span data-ttu-id="ede36-138">userId</span><span class="sxs-lookup"><span data-stu-id="ede36-138">userId</span></span>|<span data-ttu-id="ede36-139">String</span><span class="sxs-lookup"><span data-stu-id="ede36-139">String</span></span>|<span data-ttu-id="ede36-140">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="ede36-140">The user ID.</span></span>|
|<span data-ttu-id="ede36-141">userName</span><span class="sxs-lookup"><span data-stu-id="ede36-141">userName</span></span>|<span data-ttu-id="ede36-142">String</span><span class="sxs-lookup"><span data-stu-id="ede36-142">String</span></span>|<span data-ttu-id="ede36-143">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="ede36-143">The user name.</span></span>|
|<span data-ttu-id="ede36-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ede36-144">userPrincipalName</span></span>|<span data-ttu-id="ede36-145">Строка</span><span class="sxs-lookup"><span data-stu-id="ede36-145">String</span></span>|<span data-ttu-id="ede36-146">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="ede36-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="ede36-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="ede36-147">Response</span></span>
<span data-ttu-id="ede36-148">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ede36-148">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ede36-149">Пример</span><span class="sxs-lookup"><span data-stu-id="ede36-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="ede36-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="ede36-150">Request</span></span>
<span data-ttu-id="ede36-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ede36-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ede36-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="ede36-152">Response</span></span>
<span data-ttu-id="ede36-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ede36-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




