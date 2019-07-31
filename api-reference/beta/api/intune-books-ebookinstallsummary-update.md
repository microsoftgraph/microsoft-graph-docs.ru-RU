---
title: Update eBookInstallSummary
description: Обновление свойств объекта eBookInstallSummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fb5e5c0b14b41f4f3ea5c489f87f130d46b49bcd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959385"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="c4fdf-103">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="c4fdf-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="c4fdf-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4fdf-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4fdf-106">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c4fdf-106">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4fdf-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c4fdf-107">Prerequisites</span></span>
<span data-ttu-id="c4fdf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4fdf-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4fdf-110">Permission type</span></span>|<span data-ttu-id="c4fdf-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4fdf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4fdf-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4fdf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4fdf-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4fdf-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c4fdf-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4fdf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4fdf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-115">Not supported.</span></span>|
|<span data-ttu-id="c4fdf-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4fdf-116">Application</span></span>|<span data-ttu-id="c4fdf-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4fdf-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4fdf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="c4fdf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4fdf-119">Request headers</span></span>
|<span data-ttu-id="c4fdf-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4fdf-120">Header</span></span>|<span data-ttu-id="c4fdf-121">Значение</span><span class="sxs-lookup"><span data-stu-id="c4fdf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4fdf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4fdf-122">Authorization</span></span>|<span data-ttu-id="c4fdf-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4fdf-124">Accept</span><span class="sxs-lookup"><span data-stu-id="c4fdf-124">Accept</span></span>|<span data-ttu-id="c4fdf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c4fdf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4fdf-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c4fdf-126">Request body</span></span>
<span data-ttu-id="c4fdf-127">В теле запроса добавьте представление объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-127">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="c4fdf-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="c4fdf-128">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="c4fdf-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4fdf-129">Property</span></span>|<span data-ttu-id="c4fdf-130">Тип</span><span class="sxs-lookup"><span data-stu-id="c4fdf-130">Type</span></span>|<span data-ttu-id="c4fdf-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c4fdf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4fdf-132">id</span><span class="sxs-lookup"><span data-stu-id="c4fdf-132">id</span></span>|<span data-ttu-id="c4fdf-133">String</span><span class="sxs-lookup"><span data-stu-id="c4fdf-133">String</span></span>|<span data-ttu-id="c4fdf-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-134">Key of the entity.</span></span>|
|<span data-ttu-id="c4fdf-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4fdf-135">installedDeviceCount</span></span>|<span data-ttu-id="c4fdf-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c4fdf-136">Int32</span></span>|<span data-ttu-id="c4fdf-137">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-137">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="c4fdf-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4fdf-138">failedDeviceCount</span></span>|<span data-ttu-id="c4fdf-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c4fdf-139">Int32</span></span>|<span data-ttu-id="c4fdf-140">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-140">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="c4fdf-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="c4fdf-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="c4fdf-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c4fdf-142">Int32</span></span>|<span data-ttu-id="c4fdf-143">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-143">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="c4fdf-144">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="c4fdf-144">installedUserCount</span></span>|<span data-ttu-id="c4fdf-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c4fdf-145">Int32</span></span>|<span data-ttu-id="c4fdf-146">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-146">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="c4fdf-147">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="c4fdf-147">failedUserCount</span></span>|<span data-ttu-id="c4fdf-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c4fdf-148">Int32</span></span>|<span data-ttu-id="c4fdf-149">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-149">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="c4fdf-150">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="c4fdf-150">notInstalledUserCount</span></span>|<span data-ttu-id="c4fdf-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c4fdf-151">Int32</span></span>|<span data-ttu-id="c4fdf-152">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-152">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="c4fdf-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4fdf-153">Response</span></span>
<span data-ttu-id="c4fdf-154">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-154">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4fdf-155">Пример</span><span class="sxs-lookup"><span data-stu-id="c4fdf-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4fdf-156">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4fdf-156">Request</span></span>
<span data-ttu-id="c4fdf-157">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c4fdf-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4fdf-158">Response</span></span>
<span data-ttu-id="c4fdf-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c4fdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





