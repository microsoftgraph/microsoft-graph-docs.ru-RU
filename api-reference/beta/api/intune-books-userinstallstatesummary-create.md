---
title: Создание объекта userInstallStateSummary
description: Создание объекта userInstallStateSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 33ce8deba11363f27971a3c5bc2ac1fef5c05a45
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335909"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="82729-103">Создание объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="82729-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="82729-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82729-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82729-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="82729-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82729-106">Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="82729-106">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82729-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="82729-107">Prerequisites</span></span>
<span data-ttu-id="82729-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="82729-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82729-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="82729-110">Permission type</span></span>|<span data-ttu-id="82729-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="82729-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82729-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="82729-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82729-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82729-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="82729-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="82729-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82729-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="82729-115">Not supported.</span></span>|
|<span data-ttu-id="82729-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="82729-116">Application</span></span>|<span data-ttu-id="82729-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82729-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="82729-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="82729-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="82729-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="82729-119">Request headers</span></span>
|<span data-ttu-id="82729-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="82729-120">Header</span></span>|<span data-ttu-id="82729-121">Значение</span><span class="sxs-lookup"><span data-stu-id="82729-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82729-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="82729-122">Authorization</span></span>|<span data-ttu-id="82729-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="82729-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82729-124">Accept</span><span class="sxs-lookup"><span data-stu-id="82729-124">Accept</span></span>|<span data-ttu-id="82729-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82729-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82729-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="82729-126">Request body</span></span>
<span data-ttu-id="82729-127">В тексте запроса добавьте представление объекта userInstallStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82729-127">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="82729-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="82729-128">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="82729-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="82729-129">Property</span></span>|<span data-ttu-id="82729-130">Тип</span><span class="sxs-lookup"><span data-stu-id="82729-130">Type</span></span>|<span data-ttu-id="82729-131">Описание</span><span class="sxs-lookup"><span data-stu-id="82729-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82729-132">id</span><span class="sxs-lookup"><span data-stu-id="82729-132">id</span></span>|<span data-ttu-id="82729-133">String</span><span class="sxs-lookup"><span data-stu-id="82729-133">String</span></span>|<span data-ttu-id="82729-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="82729-134">Key of the entity.</span></span>|
|<span data-ttu-id="82729-135">userName</span><span class="sxs-lookup"><span data-stu-id="82729-135">userName</span></span>|<span data-ttu-id="82729-136">String</span><span class="sxs-lookup"><span data-stu-id="82729-136">String</span></span>|<span data-ttu-id="82729-137">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="82729-137">User name.</span></span>|
|<span data-ttu-id="82729-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82729-138">installedDeviceCount</span></span>|<span data-ttu-id="82729-139">Int32</span><span class="sxs-lookup"><span data-stu-id="82729-139">Int32</span></span>|<span data-ttu-id="82729-140">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="82729-140">Installed Device Count.</span></span>|
|<span data-ttu-id="82729-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82729-141">failedDeviceCount</span></span>|<span data-ttu-id="82729-142">Int32</span><span class="sxs-lookup"><span data-stu-id="82729-142">Int32</span></span>|<span data-ttu-id="82729-143">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="82729-143">Failed Device Count.</span></span>|
|<span data-ttu-id="82729-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="82729-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="82729-145">Int32</span><span class="sxs-lookup"><span data-stu-id="82729-145">Int32</span></span>|<span data-ttu-id="82729-146">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="82729-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="82729-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="82729-147">Response</span></span>
<span data-ttu-id="82729-148">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="82729-148">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82729-149">Пример</span><span class="sxs-lookup"><span data-stu-id="82729-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="82729-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="82729-150">Request</span></span>
<span data-ttu-id="82729-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="82729-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
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

### <a name="response"></a><span data-ttu-id="82729-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="82729-152">Response</span></span>
<span data-ttu-id="82729-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="82729-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






