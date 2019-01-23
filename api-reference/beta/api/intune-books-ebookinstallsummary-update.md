---
title: Update eBookInstallSummary
description: Обновление свойств объекта eBookInstallSummary.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85e94a16799b9ee56c28041549b1d21692013599
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421167"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="0b8ba-103">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0b8ba-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="0b8ba-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b8ba-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b8ba-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b8ba-107">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b8ba-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b8ba-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0b8ba-108">Prerequisites</span></span>
<span data-ttu-id="0b8ba-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="0b8ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b8ba-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0b8ba-111">Permission type</span></span>|<span data-ttu-id="0b8ba-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0b8ba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b8ba-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0b8ba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b8ba-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b8ba-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b8ba-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0b8ba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b8ba-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-116">Not supported.</span></span>|
|<span data-ttu-id="0b8ba-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0b8ba-117">Application</span></span>|<span data-ttu-id="0b8ba-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b8ba-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0b8ba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="0b8ba-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0b8ba-120">Request headers</span></span>
|<span data-ttu-id="0b8ba-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0b8ba-121">Header</span></span>|<span data-ttu-id="0b8ba-122">Значение</span><span class="sxs-lookup"><span data-stu-id="0b8ba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b8ba-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0b8ba-123">Authorization</span></span>|<span data-ttu-id="0b8ba-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="0b8ba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b8ba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b8ba-125">Accept</span></span>|<span data-ttu-id="0b8ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b8ba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b8ba-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0b8ba-127">Request body</span></span>
<span data-ttu-id="0b8ba-128">В теле запроса добавьте представление объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="0b8ba-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="0b8ba-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="0b8ba-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="0b8ba-130">Property</span></span>|<span data-ttu-id="0b8ba-131">Тип</span><span class="sxs-lookup"><span data-stu-id="0b8ba-131">Type</span></span>|<span data-ttu-id="0b8ba-132">Описание</span><span class="sxs-lookup"><span data-stu-id="0b8ba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b8ba-133">id</span><span class="sxs-lookup"><span data-stu-id="0b8ba-133">id</span></span>|<span data-ttu-id="0b8ba-134">String</span><span class="sxs-lookup"><span data-stu-id="0b8ba-134">String</span></span>|<span data-ttu-id="0b8ba-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-135">Key of the entity.</span></span>|
|<span data-ttu-id="0b8ba-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b8ba-136">installedDeviceCount</span></span>|<span data-ttu-id="0b8ba-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0b8ba-137">Int32</span></span>|<span data-ttu-id="0b8ba-138">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="0b8ba-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b8ba-139">failedDeviceCount</span></span>|<span data-ttu-id="0b8ba-140">Int32</span><span class="sxs-lookup"><span data-stu-id="0b8ba-140">Int32</span></span>|<span data-ttu-id="0b8ba-141">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="0b8ba-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="0b8ba-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="0b8ba-143">Int32</span><span class="sxs-lookup"><span data-stu-id="0b8ba-143">Int32</span></span>|<span data-ttu-id="0b8ba-144">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="0b8ba-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="0b8ba-145">installedUserCount</span></span>|<span data-ttu-id="0b8ba-146">Int32</span><span class="sxs-lookup"><span data-stu-id="0b8ba-146">Int32</span></span>|<span data-ttu-id="0b8ba-147">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="0b8ba-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="0b8ba-148">failedUserCount</span></span>|<span data-ttu-id="0b8ba-149">Int32</span><span class="sxs-lookup"><span data-stu-id="0b8ba-149">Int32</span></span>|<span data-ttu-id="0b8ba-150">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="0b8ba-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="0b8ba-151">notInstalledUserCount</span></span>|<span data-ttu-id="0b8ba-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0b8ba-152">Int32</span></span>|<span data-ttu-id="0b8ba-153">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="0b8ba-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="0b8ba-154">Response</span></span>
<span data-ttu-id="0b8ba-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b8ba-156">Пример</span><span class="sxs-lookup"><span data-stu-id="0b8ba-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b8ba-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="0b8ba-157">Request</span></span>
<span data-ttu-id="0b8ba-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b8ba-159">Отклик</span><span class="sxs-lookup"><span data-stu-id="0b8ba-159">Response</span></span>
<span data-ttu-id="0b8ba-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="0b8ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




