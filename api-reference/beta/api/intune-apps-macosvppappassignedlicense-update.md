---
title: Обновление macOsVppAppAssignedLicense
description: Обновление свойства объекта macOsVppAppAssignedLicense.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0e3a8a2c54035a29225be547c9971d70fb70f92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431732"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="54329-103">Обновление macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="54329-103">Update macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="54329-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54329-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54329-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54329-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54329-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="54329-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54329-107">Обновление свойства объекта [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="54329-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54329-108">Предварительные требования</span><span class="sxs-lookup"><span data-stu-id="54329-108">Prerequisites</span></span>
<span data-ttu-id="54329-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="54329-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54329-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54329-111">Permission type</span></span>|<span data-ttu-id="54329-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="54329-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54329-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54329-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54329-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54329-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54329-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54329-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54329-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54329-116">Not supported.</span></span>|
|<span data-ttu-id="54329-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="54329-117">Application</span></span>|<span data-ttu-id="54329-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54329-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54329-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54329-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="54329-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54329-120">Request headers</span></span>
|<span data-ttu-id="54329-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54329-121">Header</span></span>|<span data-ttu-id="54329-122">Значение</span><span class="sxs-lookup"><span data-stu-id="54329-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54329-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54329-123">Authorization</span></span>|<span data-ttu-id="54329-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="54329-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54329-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54329-125">Accept</span></span>|<span data-ttu-id="54329-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54329-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54329-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54329-127">Request body</span></span>
<span data-ttu-id="54329-128">В тексте запроса укажите представление JSON для объекта [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="54329-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="54329-129">В следующей таблице показаны свойства, которые необходимы для создания [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span><span class="sxs-lookup"><span data-stu-id="54329-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="54329-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="54329-130">Property</span></span>|<span data-ttu-id="54329-131">Тип</span><span class="sxs-lookup"><span data-stu-id="54329-131">Type</span></span>|<span data-ttu-id="54329-132">Описание</span><span class="sxs-lookup"><span data-stu-id="54329-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54329-133">id</span><span class="sxs-lookup"><span data-stu-id="54329-133">id</span></span>|<span data-ttu-id="54329-134">String</span><span class="sxs-lookup"><span data-stu-id="54329-134">String</span></span>|<span data-ttu-id="54329-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="54329-135">Key of the entity.</span></span>|
|<span data-ttu-id="54329-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="54329-136">userEmailAddress</span></span>|<span data-ttu-id="54329-137">String</span><span class="sxs-lookup"><span data-stu-id="54329-137">String</span></span>|<span data-ttu-id="54329-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="54329-138">The user email address.</span></span>|
|<span data-ttu-id="54329-139">userId</span><span class="sxs-lookup"><span data-stu-id="54329-139">userId</span></span>|<span data-ttu-id="54329-140">String</span><span class="sxs-lookup"><span data-stu-id="54329-140">String</span></span>|<span data-ttu-id="54329-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="54329-141">The user ID.</span></span>|
|<span data-ttu-id="54329-142">userName</span><span class="sxs-lookup"><span data-stu-id="54329-142">userName</span></span>|<span data-ttu-id="54329-143">String</span><span class="sxs-lookup"><span data-stu-id="54329-143">String</span></span>|<span data-ttu-id="54329-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="54329-144">The user name.</span></span>|
|<span data-ttu-id="54329-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="54329-145">userPrincipalName</span></span>|<span data-ttu-id="54329-146">String</span><span class="sxs-lookup"><span data-stu-id="54329-146">String</span></span>|<span data-ttu-id="54329-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="54329-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="54329-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="54329-148">Response</span></span>
<span data-ttu-id="54329-149">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="54329-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54329-150">Пример</span><span class="sxs-lookup"><span data-stu-id="54329-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="54329-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="54329-151">Request</span></span>
<span data-ttu-id="54329-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54329-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="54329-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="54329-153">Response</span></span>
<span data-ttu-id="54329-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="54329-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




