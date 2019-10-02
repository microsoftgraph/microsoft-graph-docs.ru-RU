---
title: Создание объекта userInstallStateSummary
description: Создание объекта userInstallStateSummary.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 23060cad3191e2df69614c3f9238bd9fbdf56ca2
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37354653"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="3ced4-103">Создание объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="3ced4-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="3ced4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3ced4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ced4-105">Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="3ced4-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3ced4-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="3ced4-106">Prerequisites</span></span>
<span data-ttu-id="3ced4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ced4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ced4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3ced4-109">Permission type</span></span>|<span data-ttu-id="3ced4-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3ced4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3ced4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3ced4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3ced4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ced4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3ced4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3ced4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3ced4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ced4-114">Not supported.</span></span>|
|<span data-ttu-id="3ced4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3ced4-115">Application</span></span>|<span data-ttu-id="3ced4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3ced4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3ced4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3ced4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="3ced4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3ced4-118">Request headers</span></span>
|<span data-ttu-id="3ced4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3ced4-119">Header</span></span>|<span data-ttu-id="3ced4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3ced4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3ced4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3ced4-121">Authorization</span></span>|<span data-ttu-id="3ced4-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3ced4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3ced4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3ced4-123">Accept</span></span>|<span data-ttu-id="3ced4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3ced4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3ced4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3ced4-125">Request body</span></span>
<span data-ttu-id="3ced4-126">В тексте запроса добавьте представление объекта userInstallStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3ced4-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="3ced4-127">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="3ced4-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="3ced4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="3ced4-128">Property</span></span>|<span data-ttu-id="3ced4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="3ced4-129">Type</span></span>|<span data-ttu-id="3ced4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="3ced4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ced4-131">id</span><span class="sxs-lookup"><span data-stu-id="3ced4-131">id</span></span>|<span data-ttu-id="3ced4-132">String</span><span class="sxs-lookup"><span data-stu-id="3ced4-132">String</span></span>|<span data-ttu-id="3ced4-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3ced4-133">Key of the entity.</span></span>|
|<span data-ttu-id="3ced4-134">userName</span><span class="sxs-lookup"><span data-stu-id="3ced4-134">userName</span></span>|<span data-ttu-id="3ced4-135">String</span><span class="sxs-lookup"><span data-stu-id="3ced4-135">String</span></span>|<span data-ttu-id="3ced4-136">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="3ced4-136">User name.</span></span>|
|<span data-ttu-id="3ced4-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ced4-137">installedDeviceCount</span></span>|<span data-ttu-id="3ced4-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3ced4-138">Int32</span></span>|<span data-ttu-id="3ced4-139">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="3ced4-139">Installed Device Count.</span></span>|
|<span data-ttu-id="3ced4-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ced4-140">failedDeviceCount</span></span>|<span data-ttu-id="3ced4-141">Int32</span><span class="sxs-lookup"><span data-stu-id="3ced4-141">Int32</span></span>|<span data-ttu-id="3ced4-142">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="3ced4-142">Failed Device Count.</span></span>|
|<span data-ttu-id="3ced4-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3ced4-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="3ced4-144">Int32</span><span class="sxs-lookup"><span data-stu-id="3ced4-144">Int32</span></span>|<span data-ttu-id="3ced4-145">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="3ced4-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="3ced4-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ced4-146">Response</span></span>
<span data-ttu-id="3ced4-147">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3ced4-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ced4-148">Пример</span><span class="sxs-lookup"><span data-stu-id="3ced4-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="3ced4-149">Запрос</span><span class="sxs-lookup"><span data-stu-id="3ced4-149">Request</span></span>
<span data-ttu-id="3ced4-150">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3ced4-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3ced4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="3ced4-151">Response</span></span>
<span data-ttu-id="3ced4-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3ced4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




