---
title: Создание iosVppAppAssignedLicense
description: Создайте новый объект iosVppAppAssignedLicense.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6ae534c4edc24683221c204b4e6de48b2b17c69f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51144034"
---
# <a name="create-iosvppappassignedlicense"></a><span data-ttu-id="98cd3-103">Создание iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="98cd3-103">Create iosVppAppAssignedLicense</span></span>

<span data-ttu-id="98cd3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98cd3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98cd3-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98cd3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98cd3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="98cd3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98cd3-107">Создайте новый [объект iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="98cd3-107">Create a new [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98cd3-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="98cd3-108">Prerequisites</span></span>
<span data-ttu-id="98cd3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98cd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98cd3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98cd3-111">Permission type</span></span>|<span data-ttu-id="98cd3-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98cd3-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98cd3-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98cd3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98cd3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98cd3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="98cd3-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98cd3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98cd3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98cd3-116">Not supported.</span></span>|
|<span data-ttu-id="98cd3-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="98cd3-117">Application</span></span>|<span data-ttu-id="98cd3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98cd3-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98cd3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98cd3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="98cd3-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="98cd3-120">Request headers</span></span>
|<span data-ttu-id="98cd3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98cd3-121">Header</span></span>|<span data-ttu-id="98cd3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="98cd3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98cd3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98cd3-123">Authorization</span></span>|<span data-ttu-id="98cd3-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98cd3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98cd3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98cd3-125">Accept</span></span>|<span data-ttu-id="98cd3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98cd3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98cd3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="98cd3-127">Request body</span></span>
<span data-ttu-id="98cd3-128">В теле запроса поставляем представление JSON для объекта iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="98cd3-128">In the request body, supply a JSON representation for the iosVppAppAssignedLicense object.</span></span>

<span data-ttu-id="98cd3-129">В следующей таблице показаны свойства, необходимые при создании iosVppAppAssignedLicense.</span><span class="sxs-lookup"><span data-stu-id="98cd3-129">The following table shows the properties that are required when you create the iosVppAppAssignedLicense.</span></span>

|<span data-ttu-id="98cd3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="98cd3-130">Property</span></span>|<span data-ttu-id="98cd3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="98cd3-131">Type</span></span>|<span data-ttu-id="98cd3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="98cd3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98cd3-133">id</span><span class="sxs-lookup"><span data-stu-id="98cd3-133">id</span></span>|<span data-ttu-id="98cd3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="98cd3-134">String</span></span>|<span data-ttu-id="98cd3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="98cd3-135">Key of the entity.</span></span>|
|<span data-ttu-id="98cd3-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="98cd3-136">userEmailAddress</span></span>|<span data-ttu-id="98cd3-137">Строка</span><span class="sxs-lookup"><span data-stu-id="98cd3-137">String</span></span>|<span data-ttu-id="98cd3-138">Адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="98cd3-138">The user email address.</span></span>|
|<span data-ttu-id="98cd3-139">userId</span><span class="sxs-lookup"><span data-stu-id="98cd3-139">userId</span></span>|<span data-ttu-id="98cd3-140">String</span><span class="sxs-lookup"><span data-stu-id="98cd3-140">String</span></span>|<span data-ttu-id="98cd3-141">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="98cd3-141">The user ID.</span></span>|
|<span data-ttu-id="98cd3-142">userName</span><span class="sxs-lookup"><span data-stu-id="98cd3-142">userName</span></span>|<span data-ttu-id="98cd3-143">String</span><span class="sxs-lookup"><span data-stu-id="98cd3-143">String</span></span>|<span data-ttu-id="98cd3-144">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="98cd3-144">The user name.</span></span>|
|<span data-ttu-id="98cd3-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="98cd3-145">userPrincipalName</span></span>|<span data-ttu-id="98cd3-146">String</span><span class="sxs-lookup"><span data-stu-id="98cd3-146">String</span></span>|<span data-ttu-id="98cd3-147">Имя участника-пользователя.</span><span class="sxs-lookup"><span data-stu-id="98cd3-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="98cd3-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="98cd3-148">Response</span></span>
<span data-ttu-id="98cd3-149">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="98cd3-149">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98cd3-150">Пример</span><span class="sxs-lookup"><span data-stu-id="98cd3-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="98cd3-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="98cd3-151">Request</span></span>
<span data-ttu-id="98cd3-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98cd3-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98cd3-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="98cd3-153">Response</span></span>
<span data-ttu-id="98cd3-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="98cd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




