---
title: Создание объекта userInstallStateSummary
description: Создание объекта userInstallStateSummary.
ms.openlocfilehash: d524801d8ee1b44ea955afdeb2a7c78364d89360
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028122"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="bb2b1-103">Создание объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="bb2b1-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="bb2b1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb2b1-105">Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="bb2b1-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bb2b1-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="bb2b1-106">Prerequisites</span></span>
<span data-ttu-id="bb2b1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb2b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb2b1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bb2b1-109">Permission type</span></span>|<span data-ttu-id="bb2b1-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bb2b1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb2b1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bb2b1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb2b1-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb2b1-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bb2b1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bb2b1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb2b1-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-114">Not supported.</span></span>|
|<span data-ttu-id="bb2b1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bb2b1-115">Application</span></span>|<span data-ttu-id="bb2b1-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb2b1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bb2b1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="bb2b1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bb2b1-118">Request headers</span></span>
|<span data-ttu-id="bb2b1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bb2b1-119">Header</span></span>|<span data-ttu-id="bb2b1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bb2b1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb2b1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb2b1-121">Authorization</span></span>|<span data-ttu-id="bb2b1-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bb2b1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb2b1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bb2b1-123">Accept</span></span>|<span data-ttu-id="bb2b1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb2b1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb2b1-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bb2b1-125">Request body</span></span>
<span data-ttu-id="bb2b1-126">В тексте запроса добавьте представление объекта userInstallStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="bb2b1-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="bb2b1-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb2b1-128">Property</span></span>|<span data-ttu-id="bb2b1-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bb2b1-129">Type</span></span>|<span data-ttu-id="bb2b1-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bb2b1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb2b1-131">id</span><span class="sxs-lookup"><span data-stu-id="bb2b1-131">id</span></span>|<span data-ttu-id="bb2b1-132">String</span><span class="sxs-lookup"><span data-stu-id="bb2b1-132">String</span></span>|<span data-ttu-id="bb2b1-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-133">Key of the entity.</span></span>|
|<span data-ttu-id="bb2b1-134">userName</span><span class="sxs-lookup"><span data-stu-id="bb2b1-134">userName</span></span>|<span data-ttu-id="bb2b1-135">String</span><span class="sxs-lookup"><span data-stu-id="bb2b1-135">String</span></span>|<span data-ttu-id="bb2b1-136">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-136">User name.</span></span>|
|<span data-ttu-id="bb2b1-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb2b1-137">installedDeviceCount</span></span>|<span data-ttu-id="bb2b1-138">Int32</span><span class="sxs-lookup"><span data-stu-id="bb2b1-138">Int32</span></span>|<span data-ttu-id="bb2b1-139">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-139">Installed Device Count.</span></span>|
|<span data-ttu-id="bb2b1-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb2b1-140">failedDeviceCount</span></span>|<span data-ttu-id="bb2b1-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bb2b1-141">Int32</span></span>|<span data-ttu-id="bb2b1-142">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-142">Failed Device Count.</span></span>|
|<span data-ttu-id="bb2b1-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bb2b1-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="bb2b1-144">Int32</span><span class="sxs-lookup"><span data-stu-id="bb2b1-144">Int32</span></span>|<span data-ttu-id="bb2b1-145">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="bb2b1-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="bb2b1-146">Response</span></span>
<span data-ttu-id="bb2b1-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb2b1-148">Пример</span><span class="sxs-lookup"><span data-stu-id="bb2b1-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb2b1-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="bb2b1-149">Request</span></span>
<span data-ttu-id="bb2b1-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bb2b1-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="bb2b1-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="bb2b1-151">Response</span></span>
<span data-ttu-id="bb2b1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="bb2b1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```



