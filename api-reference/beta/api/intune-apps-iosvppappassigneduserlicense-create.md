---
title: Создание Иосвппаппассигнедусерлиценсе
description: Создание нового объекта Иосвппаппассигнедусерлиценсе.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f1efba3659190080c507ca3418bacd9bc7d6461
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157528"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="feb61-103">Создание Иосвппаппассигнедусерлиценсе</span><span class="sxs-lookup"><span data-stu-id="feb61-103">Create iosVppAppAssignedUserLicense</span></span>

> <span data-ttu-id="feb61-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feb61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="feb61-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="feb61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feb61-106">Создание нового объекта [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="feb61-106">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="feb61-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="feb61-107">Prerequisites</span></span>
<span data-ttu-id="feb61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="feb61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="feb61-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="feb61-110">Permission type</span></span>|<span data-ttu-id="feb61-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="feb61-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="feb61-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="feb61-112">Delegated (work or school account)</span></span>|<span data-ttu-id="feb61-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="feb61-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="feb61-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="feb61-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="feb61-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feb61-115">Not supported.</span></span>|
|<span data-ttu-id="feb61-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="feb61-116">Application</span></span>|<span data-ttu-id="feb61-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="feb61-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="feb61-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="feb61-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="feb61-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="feb61-119">Request headers</span></span>
|<span data-ttu-id="feb61-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="feb61-120">Header</span></span>|<span data-ttu-id="feb61-121">Значение</span><span class="sxs-lookup"><span data-stu-id="feb61-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="feb61-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="feb61-122">Authorization</span></span>|<span data-ttu-id="feb61-123">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="feb61-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="feb61-124">Accept</span><span class="sxs-lookup"><span data-stu-id="feb61-124">Accept</span></span>|<span data-ttu-id="feb61-125">application/json</span><span class="sxs-lookup"><span data-stu-id="feb61-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="feb61-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="feb61-126">Request body</span></span>
<span data-ttu-id="feb61-127">В тексте запроса добавьте представление объекта Иосвппаппассигнедусерлиценсе в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="feb61-127">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="feb61-128">В следующей таблице приведены свойства, необходимые при создании Иосвппаппассигнедусерлиценсе.</span><span class="sxs-lookup"><span data-stu-id="feb61-128">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="feb61-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="feb61-129">Property</span></span>|<span data-ttu-id="feb61-130">Тип</span><span class="sxs-lookup"><span data-stu-id="feb61-130">Type</span></span>|<span data-ttu-id="feb61-131">Описание</span><span class="sxs-lookup"><span data-stu-id="feb61-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb61-132">id</span><span class="sxs-lookup"><span data-stu-id="feb61-132">id</span></span>|<span data-ttu-id="feb61-133">String</span><span class="sxs-lookup"><span data-stu-id="feb61-133">String</span></span>|<span data-ttu-id="feb61-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="feb61-134">Key of the entity.</span></span> <span data-ttu-id="feb61-135">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="feb61-135">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="feb61-136">Усеремаиладдресс</span><span class="sxs-lookup"><span data-stu-id="feb61-136">userEmailAddress</span></span>|<span data-ttu-id="feb61-137">String</span><span class="sxs-lookup"><span data-stu-id="feb61-137">String</span></span>|<span data-ttu-id="feb61-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="feb61-138">The user email address.</span></span> <span data-ttu-id="feb61-139">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="feb61-139">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="feb61-140">userId</span><span class="sxs-lookup"><span data-stu-id="feb61-140">userId</span></span>|<span data-ttu-id="feb61-141">String</span><span class="sxs-lookup"><span data-stu-id="feb61-141">String</span></span>|<span data-ttu-id="feb61-142">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="feb61-142">The user ID.</span></span> <span data-ttu-id="feb61-143">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="feb61-143">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="feb61-144">userName</span><span class="sxs-lookup"><span data-stu-id="feb61-144">userName</span></span>|<span data-ttu-id="feb61-145">String</span><span class="sxs-lookup"><span data-stu-id="feb61-145">String</span></span>|<span data-ttu-id="feb61-146">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="feb61-146">The user name.</span></span> <span data-ttu-id="feb61-147">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="feb61-147">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="feb61-148">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="feb61-148">userPrincipalName</span></span>|<span data-ttu-id="feb61-149">Строка</span><span class="sxs-lookup"><span data-stu-id="feb61-149">String</span></span>|<span data-ttu-id="feb61-150">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="feb61-150">The user principal name.</span></span> <span data-ttu-id="feb61-151">НаСледуется от [иосвппаппассигнедлиценсе](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="feb61-151">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="feb61-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="feb61-152">Response</span></span>
<span data-ttu-id="feb61-153">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [иосвппаппассигнедусерлиценсе](../resources/intune-apps-iosvppappassigneduserlicense.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="feb61-153">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="feb61-154">Пример</span><span class="sxs-lookup"><span data-stu-id="feb61-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="feb61-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="feb61-155">Request</span></span>
<span data-ttu-id="feb61-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="feb61-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="feb61-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="feb61-157">Response</span></span>
<span data-ttu-id="feb61-p107">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="feb61-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




