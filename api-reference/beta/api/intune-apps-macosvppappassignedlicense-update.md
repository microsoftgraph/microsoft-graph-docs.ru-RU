---
title: Обновление Макосвппаппассигнедлиценсе
description: Обновление свойств объекта Макосвппаппассигнедлиценсе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0f0ccb27bb9bedcbd9d83333c60c864dc99e5b4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160426"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="cbdb8-103">Обновление Макосвппаппассигнедлиценсе</span><span class="sxs-lookup"><span data-stu-id="cbdb8-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="cbdb8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbdb8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbdb8-106">Обновление свойств объекта [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="cbdb8-106">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbdb8-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="cbdb8-107">Prerequisites</span></span>
<span data-ttu-id="cbdb8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="cbdb8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cbdb8-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbdb8-110">Permission type</span></span>|<span data-ttu-id="cbdb8-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbdb8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbdb8-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbdb8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbdb8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cbdb8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cbdb8-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbdb8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbdb8-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-115">Not supported.</span></span>|
|<span data-ttu-id="cbdb8-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbdb8-116">Application</span></span>|<span data-ttu-id="cbdb8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbdb8-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbdb8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="cbdb8-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbdb8-119">Request headers</span></span>
|<span data-ttu-id="cbdb8-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="cbdb8-120">Header</span></span>|<span data-ttu-id="cbdb8-121">Значение</span><span class="sxs-lookup"><span data-stu-id="cbdb8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbdb8-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cbdb8-122">Authorization</span></span>|<span data-ttu-id="cbdb8-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="cbdb8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbdb8-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cbdb8-124">Accept</span></span>|<span data-ttu-id="cbdb8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbdb8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbdb8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbdb8-126">Request body</span></span>
<span data-ttu-id="cbdb8-127">В тексте запроса добавьте представление объекта [Макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-127">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="cbdb8-128">В следующей таблице приведены свойства, необходимые при создании [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="cbdb8-128">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="cbdb8-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="cbdb8-129">Property</span></span>|<span data-ttu-id="cbdb8-130">Тип</span><span class="sxs-lookup"><span data-stu-id="cbdb8-130">Type</span></span>|<span data-ttu-id="cbdb8-131">Описание</span><span class="sxs-lookup"><span data-stu-id="cbdb8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbdb8-132">id</span><span class="sxs-lookup"><span data-stu-id="cbdb8-132">id</span></span>|<span data-ttu-id="cbdb8-133">String</span><span class="sxs-lookup"><span data-stu-id="cbdb8-133">String</span></span>|<span data-ttu-id="cbdb8-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-134">Key of the entity.</span></span>|
|<span data-ttu-id="cbdb8-135">Усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="cbdb8-135">userEmailAddress</span></span>|<span data-ttu-id="cbdb8-136">String</span><span class="sxs-lookup"><span data-stu-id="cbdb8-136">String</span></span>|<span data-ttu-id="cbdb8-137">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-137">The user email address.</span></span>|
|<span data-ttu-id="cbdb8-138">userId</span><span class="sxs-lookup"><span data-stu-id="cbdb8-138">userId</span></span>|<span data-ttu-id="cbdb8-139">String</span><span class="sxs-lookup"><span data-stu-id="cbdb8-139">String</span></span>|<span data-ttu-id="cbdb8-140">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-140">The user ID.</span></span>|
|<span data-ttu-id="cbdb8-141">userName</span><span class="sxs-lookup"><span data-stu-id="cbdb8-141">userName</span></span>|<span data-ttu-id="cbdb8-142">String</span><span class="sxs-lookup"><span data-stu-id="cbdb8-142">String</span></span>|<span data-ttu-id="cbdb8-143">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-143">The user name.</span></span>|
|<span data-ttu-id="cbdb8-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cbdb8-144">userPrincipalName</span></span>|<span data-ttu-id="cbdb8-145">Строка</span><span class="sxs-lookup"><span data-stu-id="cbdb8-145">String</span></span>|<span data-ttu-id="cbdb8-146">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="cbdb8-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbdb8-147">Response</span></span>
<span data-ttu-id="cbdb8-148">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [макосвппаппассигнедлиценсе](../resources/intune-apps-macosvppappassignedlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-148">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbdb8-149">Пример</span><span class="sxs-lookup"><span data-stu-id="cbdb8-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbdb8-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="cbdb8-150">Request</span></span>
<span data-ttu-id="cbdb8-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="cbdb8-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbdb8-152">Response</span></span>
<span data-ttu-id="cbdb8-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbdb8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




