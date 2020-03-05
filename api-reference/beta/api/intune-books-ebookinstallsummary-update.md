---
title: Update eBookInstallSummary
description: Обновление свойств объекта eBookInstallSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d31bd389951a71c1fcca3cb26e5560b53a9195c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42444590"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="d3fee-103">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d3fee-103">Update eBookInstallSummary</span></span>

<span data-ttu-id="d3fee-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d3fee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3fee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3fee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3fee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d3fee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3fee-107">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d3fee-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3fee-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d3fee-108">Prerequisites</span></span>
<span data-ttu-id="d3fee-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3fee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3fee-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3fee-111">Permission type</span></span>|<span data-ttu-id="d3fee-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3fee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3fee-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3fee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d3fee-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3fee-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d3fee-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3fee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3fee-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3fee-116">Not supported.</span></span>|
|<span data-ttu-id="d3fee-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d3fee-117">Application</span></span>|<span data-ttu-id="d3fee-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3fee-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3fee-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3fee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="d3fee-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d3fee-120">Request headers</span></span>
|<span data-ttu-id="d3fee-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3fee-121">Header</span></span>|<span data-ttu-id="d3fee-122">Значение</span><span class="sxs-lookup"><span data-stu-id="d3fee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3fee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3fee-123">Authorization</span></span>|<span data-ttu-id="d3fee-124">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3fee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3fee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d3fee-125">Accept</span></span>|<span data-ttu-id="d3fee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3fee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3fee-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d3fee-127">Request body</span></span>
<span data-ttu-id="d3fee-128">В теле запроса добавьте представление объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3fee-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="d3fee-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="d3fee-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="d3fee-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3fee-130">Property</span></span>|<span data-ttu-id="d3fee-131">Тип</span><span class="sxs-lookup"><span data-stu-id="d3fee-131">Type</span></span>|<span data-ttu-id="d3fee-132">Описание</span><span class="sxs-lookup"><span data-stu-id="d3fee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3fee-133">id</span><span class="sxs-lookup"><span data-stu-id="d3fee-133">id</span></span>|<span data-ttu-id="d3fee-134">String</span><span class="sxs-lookup"><span data-stu-id="d3fee-134">String</span></span>|<span data-ttu-id="d3fee-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d3fee-135">Key of the entity.</span></span>|
|<span data-ttu-id="d3fee-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3fee-136">installedDeviceCount</span></span>|<span data-ttu-id="d3fee-137">Int32</span><span class="sxs-lookup"><span data-stu-id="d3fee-137">Int32</span></span>|<span data-ttu-id="d3fee-138">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="d3fee-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="d3fee-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3fee-139">failedDeviceCount</span></span>|<span data-ttu-id="d3fee-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d3fee-140">Int32</span></span>|<span data-ttu-id="d3fee-141">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="d3fee-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="d3fee-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d3fee-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="d3fee-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d3fee-143">Int32</span></span>|<span data-ttu-id="d3fee-144">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="d3fee-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="d3fee-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="d3fee-145">installedUserCount</span></span>|<span data-ttu-id="d3fee-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d3fee-146">Int32</span></span>|<span data-ttu-id="d3fee-147">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="d3fee-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="d3fee-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="d3fee-148">failedUserCount</span></span>|<span data-ttu-id="d3fee-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d3fee-149">Int32</span></span>|<span data-ttu-id="d3fee-150">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="d3fee-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="d3fee-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="d3fee-151">notInstalledUserCount</span></span>|<span data-ttu-id="d3fee-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d3fee-152">Int32</span></span>|<span data-ttu-id="d3fee-153">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="d3fee-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="d3fee-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3fee-154">Response</span></span>
<span data-ttu-id="d3fee-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d3fee-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3fee-156">Пример</span><span class="sxs-lookup"><span data-stu-id="d3fee-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3fee-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3fee-157">Request</span></span>
<span data-ttu-id="d3fee-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3fee-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="d3fee-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="d3fee-159">Response</span></span>
<span data-ttu-id="d3fee-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3fee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```





