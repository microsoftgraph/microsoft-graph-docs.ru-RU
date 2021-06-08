---
title: Обновление объекта userInstallStateSummary
description: Обновление свойств объекта userInstallStateSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2c7a87b15e70d902b5001af2bcdf48f76107bde7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758479"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="7f321-103">Обновление объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="7f321-103">Update userInstallStateSummary</span></span>

<span data-ttu-id="7f321-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f321-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f321-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7f321-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f321-106">Обновление свойств объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7f321-106">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f321-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="7f321-107">Prerequisites</span></span>
<span data-ttu-id="7f321-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f321-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f321-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f321-110">Permission type</span></span>|<span data-ttu-id="7f321-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f321-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f321-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f321-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f321-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f321-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f321-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f321-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f321-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f321-115">Not supported.</span></span>|
|<span data-ttu-id="7f321-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7f321-116">Application</span></span>|<span data-ttu-id="7f321-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f321-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f321-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f321-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7f321-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="7f321-119">Request headers</span></span>
|<span data-ttu-id="7f321-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f321-120">Header</span></span>|<span data-ttu-id="7f321-121">Значение</span><span class="sxs-lookup"><span data-stu-id="7f321-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f321-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f321-122">Authorization</span></span>|<span data-ttu-id="7f321-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f321-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f321-124">Accept</span><span class="sxs-lookup"><span data-stu-id="7f321-124">Accept</span></span>|<span data-ttu-id="7f321-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f321-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f321-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7f321-126">Request body</span></span>
<span data-ttu-id="7f321-127">В тексте запроса добавьте представление объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f321-127">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="7f321-128">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="7f321-128">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="7f321-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="7f321-129">Property</span></span>|<span data-ttu-id="7f321-130">Тип</span><span class="sxs-lookup"><span data-stu-id="7f321-130">Type</span></span>|<span data-ttu-id="7f321-131">Описание</span><span class="sxs-lookup"><span data-stu-id="7f321-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f321-132">id</span><span class="sxs-lookup"><span data-stu-id="7f321-132">id</span></span>|<span data-ttu-id="7f321-133">String</span><span class="sxs-lookup"><span data-stu-id="7f321-133">String</span></span>|<span data-ttu-id="7f321-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="7f321-134">Key of the entity.</span></span>|
|<span data-ttu-id="7f321-135">userName</span><span class="sxs-lookup"><span data-stu-id="7f321-135">userName</span></span>|<span data-ttu-id="7f321-136">String</span><span class="sxs-lookup"><span data-stu-id="7f321-136">String</span></span>|<span data-ttu-id="7f321-137">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="7f321-137">User name.</span></span>|
|<span data-ttu-id="7f321-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7f321-138">installedDeviceCount</span></span>|<span data-ttu-id="7f321-139">Int32</span><span class="sxs-lookup"><span data-stu-id="7f321-139">Int32</span></span>|<span data-ttu-id="7f321-140">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="7f321-140">Installed Device Count.</span></span>|
|<span data-ttu-id="7f321-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7f321-141">failedDeviceCount</span></span>|<span data-ttu-id="7f321-142">Int32</span><span class="sxs-lookup"><span data-stu-id="7f321-142">Int32</span></span>|<span data-ttu-id="7f321-143">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="7f321-143">Failed Device Count.</span></span>|
|<span data-ttu-id="7f321-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7f321-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="7f321-145">Int32</span><span class="sxs-lookup"><span data-stu-id="7f321-145">Int32</span></span>|<span data-ttu-id="7f321-146">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="7f321-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="7f321-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f321-147">Response</span></span>
<span data-ttu-id="7f321-148">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и обновленный объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7f321-148">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f321-149">Пример</span><span class="sxs-lookup"><span data-stu-id="7f321-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f321-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f321-150">Request</span></span>
<span data-ttu-id="7f321-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f321-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="7f321-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f321-152">Response</span></span>
<span data-ttu-id="7f321-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7f321-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




