---
title: Обновление объекта userInstallStateSummary
description: Обновление свойств объекта userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae856b6d544c99b32f785c24aaa922a6fe9fdb62
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132949"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="f0a52-103">Обновление объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="f0a52-103">Update userInstallStateSummary</span></span>

<span data-ttu-id="f0a52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0a52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0a52-105">**Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0a52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0a52-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f0a52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0a52-107">Обновление свойств объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f0a52-107">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0a52-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="f0a52-108">Prerequisites</span></span>
<span data-ttu-id="f0a52-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0a52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0a52-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f0a52-111">Permission type</span></span>|<span data-ttu-id="f0a52-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f0a52-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0a52-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f0a52-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0a52-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0a52-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0a52-115">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f0a52-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0a52-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f0a52-116">Not supported.</span></span>|
|<span data-ttu-id="f0a52-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="f0a52-117">Application</span></span>|<span data-ttu-id="f0a52-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0a52-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0a52-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f0a52-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="f0a52-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="f0a52-120">Request headers</span></span>
|<span data-ttu-id="f0a52-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f0a52-121">Header</span></span>|<span data-ttu-id="f0a52-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f0a52-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0a52-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0a52-123">Authorization</span></span>|<span data-ttu-id="f0a52-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0a52-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0a52-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0a52-125">Accept</span></span>|<span data-ttu-id="f0a52-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0a52-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0a52-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f0a52-127">Request body</span></span>
<span data-ttu-id="f0a52-128">В тексте запроса добавьте представление объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f0a52-128">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="f0a52-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="f0a52-129">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="f0a52-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f0a52-130">Property</span></span>|<span data-ttu-id="f0a52-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f0a52-131">Type</span></span>|<span data-ttu-id="f0a52-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f0a52-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0a52-133">id</span><span class="sxs-lookup"><span data-stu-id="f0a52-133">id</span></span>|<span data-ttu-id="f0a52-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f0a52-134">String</span></span>|<span data-ttu-id="f0a52-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f0a52-135">Key of the entity.</span></span>|
|<span data-ttu-id="f0a52-136">userName</span><span class="sxs-lookup"><span data-stu-id="f0a52-136">userName</span></span>|<span data-ttu-id="f0a52-137">String</span><span class="sxs-lookup"><span data-stu-id="f0a52-137">String</span></span>|<span data-ttu-id="f0a52-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="f0a52-138">User name.</span></span>|
|<span data-ttu-id="f0a52-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0a52-139">installedDeviceCount</span></span>|<span data-ttu-id="f0a52-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a52-140">Int32</span></span>|<span data-ttu-id="f0a52-141">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f0a52-141">Installed Device Count.</span></span>|
|<span data-ttu-id="f0a52-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0a52-142">failedDeviceCount</span></span>|<span data-ttu-id="f0a52-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a52-143">Int32</span></span>|<span data-ttu-id="f0a52-144">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="f0a52-144">Failed Device Count.</span></span>|
|<span data-ttu-id="f0a52-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f0a52-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="f0a52-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f0a52-146">Int32</span></span>|<span data-ttu-id="f0a52-147">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="f0a52-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="f0a52-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0a52-148">Response</span></span>
<span data-ttu-id="f0a52-149">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f0a52-149">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0a52-150">Пример</span><span class="sxs-lookup"><span data-stu-id="f0a52-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0a52-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="f0a52-151">Request</span></span>
<span data-ttu-id="f0a52-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f0a52-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="f0a52-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="f0a52-153">Response</span></span>
<span data-ttu-id="f0a52-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f0a52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




