---
title: Создание Иосвппаппассигнедусерлиценсе
description: Создание нового объекта Иосвппаппассигнедусерлиценсе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c59a79c158bfa9c14d3e489765d8f6b6e1c5e538
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32495507"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="c15ad-103">Создание Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="c15ad-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="c15ad-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c15ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c15ad-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c15ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c15ad-106">Создание нового объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="c15ad-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c15ad-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c15ad-107">Prerequisites</span></span>
<span data-ttu-id="c15ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c15ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c15ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c15ad-110">Permission type</span></span>|<span data-ttu-id="c15ad-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c15ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c15ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c15ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c15ad-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c15ad-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c15ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c15ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c15ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c15ad-115">Not supported.</span></span>|
|<span data-ttu-id="c15ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c15ad-116">Application</span></span>|<span data-ttu-id="c15ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c15ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c15ad-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c15ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="c15ad-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c15ad-119">Request headers</span></span>
|<span data-ttu-id="c15ad-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c15ad-120">Header</span></span>|<span data-ttu-id="c15ad-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c15ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c15ad-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c15ad-122">Authorization</span></span>|<span data-ttu-id="c15ad-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c15ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c15ad-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c15ad-124">Accept</span></span>|<span data-ttu-id="c15ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c15ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c15ad-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c15ad-126">Request body</span></span>
<span data-ttu-id="c15ad-127">В тексте запроса добавьте представление объекта Иосвппаппассигнедусерлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c15ad-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="c15ad-128">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнедусерлиценсе.</span><span class="sxs-lookup"><span data-stu-id="c15ad-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="c15ad-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c15ad-129">Property</span></span>|<span data-ttu-id="c15ad-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c15ad-130">Type</span></span>|<span data-ttu-id="c15ad-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c15ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c15ad-132">id</span><span class="sxs-lookup"><span data-stu-id="c15ad-132">id</span></span>|<span data-ttu-id="c15ad-133">Строка</span><span class="sxs-lookup"><span data-stu-id="c15ad-133">String</span></span>|<span data-ttu-id="c15ad-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c15ad-134">Key of the entity.</span></span> <span data-ttu-id="c15ad-135">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c15ad-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c15ad-136">Усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="c15ad-136">userEmailAddress</span></span>|<span data-ttu-id="c15ad-137">String</span><span class="sxs-lookup"><span data-stu-id="c15ad-137">String</span></span>|<span data-ttu-id="c15ad-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="c15ad-138">The user email address.</span></span> <span data-ttu-id="c15ad-139">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c15ad-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c15ad-140">userId</span><span class="sxs-lookup"><span data-stu-id="c15ad-140">userId</span></span>|<span data-ttu-id="c15ad-141">String</span><span class="sxs-lookup"><span data-stu-id="c15ad-141">String</span></span>|<span data-ttu-id="c15ad-142">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="c15ad-142">The user ID.</span></span> <span data-ttu-id="c15ad-143">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c15ad-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c15ad-144">userName</span><span class="sxs-lookup"><span data-stu-id="c15ad-144">userName</span></span>|<span data-ttu-id="c15ad-145">String</span><span class="sxs-lookup"><span data-stu-id="c15ad-145">String</span></span>|<span data-ttu-id="c15ad-146">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="c15ad-146">The user name.</span></span> <span data-ttu-id="c15ad-147">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c15ad-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="c15ad-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c15ad-148">userPrincipalName</span></span>|<span data-ttu-id="c15ad-149">String</span><span class="sxs-lookup"><span data-stu-id="c15ad-149">String</span></span>|<span data-ttu-id="c15ad-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="c15ad-150">The user principal name.</span></span> <span data-ttu-id="c15ad-151">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="c15ad-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="c15ad-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="c15ad-152">Response</span></span>
<span data-ttu-id="c15ad-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c15ad-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c15ad-154">Пример</span><span class="sxs-lookup"><span data-stu-id="c15ad-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="c15ad-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="c15ad-155">Request</span></span>
<span data-ttu-id="c15ad-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c15ad-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c15ad-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="c15ad-157">Response</span></span>
<span data-ttu-id="c15ad-p107">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c15ad-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





