---
title: Update eBookInstallSummary
description: Обновление свойств объекта eBookInstallSummary.
author: tfitzmac
ms.openlocfilehash: 200a84609523ed81ea7e5b9b3c50bd95913ddd80
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318027"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="bacd2-103">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="bacd2-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="bacd2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bacd2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bacd2-105">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bacd2-105">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bacd2-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="bacd2-106">Prerequisites</span></span>
<span data-ttu-id="bacd2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bacd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bacd2-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bacd2-109">Permission type</span></span>|<span data-ttu-id="bacd2-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bacd2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bacd2-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bacd2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bacd2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bacd2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bacd2-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bacd2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bacd2-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacd2-114">Not supported.</span></span>|
|<span data-ttu-id="bacd2-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bacd2-115">Application</span></span>|<span data-ttu-id="bacd2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bacd2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bacd2-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bacd2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="bacd2-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bacd2-118">Request headers</span></span>
|<span data-ttu-id="bacd2-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bacd2-119">Header</span></span>|<span data-ttu-id="bacd2-120">Значение</span><span class="sxs-lookup"><span data-stu-id="bacd2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bacd2-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bacd2-121">Authorization</span></span>|<span data-ttu-id="bacd2-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="bacd2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bacd2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bacd2-123">Accept</span></span>|<span data-ttu-id="bacd2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bacd2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bacd2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bacd2-125">Request body</span></span>
<span data-ttu-id="bacd2-126">В теле запроса добавьте представление объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bacd2-126">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="bacd2-127">Ниже показаны свойства, которые необходимо указывать при создании объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="bacd2-127">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="bacd2-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="bacd2-128">Property</span></span>|<span data-ttu-id="bacd2-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bacd2-129">Type</span></span>|<span data-ttu-id="bacd2-130">Описание</span><span class="sxs-lookup"><span data-stu-id="bacd2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bacd2-131">id</span><span class="sxs-lookup"><span data-stu-id="bacd2-131">id</span></span>|<span data-ttu-id="bacd2-132">Строка</span><span class="sxs-lookup"><span data-stu-id="bacd2-132">String</span></span>|<span data-ttu-id="bacd2-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="bacd2-133">Key of the entity.</span></span>|
|<span data-ttu-id="bacd2-134">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bacd2-134">installedDeviceCount</span></span>|<span data-ttu-id="bacd2-135">Int32</span><span class="sxs-lookup"><span data-stu-id="bacd2-135">Int32</span></span>|<span data-ttu-id="bacd2-136">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="bacd2-136">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="bacd2-137">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bacd2-137">failedDeviceCount</span></span>|<span data-ttu-id="bacd2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="bacd2-138">Int32</span></span>|<span data-ttu-id="bacd2-139">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="bacd2-139">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="bacd2-140">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="bacd2-140">notInstalledDeviceCount</span></span>|<span data-ttu-id="bacd2-141">Int32</span><span class="sxs-lookup"><span data-stu-id="bacd2-141">Int32</span></span>|<span data-ttu-id="bacd2-142">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="bacd2-142">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="bacd2-143">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="bacd2-143">installedUserCount</span></span>|<span data-ttu-id="bacd2-144">Int32</span><span class="sxs-lookup"><span data-stu-id="bacd2-144">Int32</span></span>|<span data-ttu-id="bacd2-145">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="bacd2-145">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="bacd2-146">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="bacd2-146">failedUserCount</span></span>|<span data-ttu-id="bacd2-147">Int32</span><span class="sxs-lookup"><span data-stu-id="bacd2-147">Int32</span></span>|<span data-ttu-id="bacd2-148">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="bacd2-148">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="bacd2-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="bacd2-149">notInstalledUserCount</span></span>|<span data-ttu-id="bacd2-150">Int32</span><span class="sxs-lookup"><span data-stu-id="bacd2-150">Int32</span></span>|<span data-ttu-id="bacd2-151">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="bacd2-151">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="bacd2-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="bacd2-152">Response</span></span>
<span data-ttu-id="bacd2-153">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bacd2-153">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bacd2-154">Пример</span><span class="sxs-lookup"><span data-stu-id="bacd2-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="bacd2-155">Запрос</span><span class="sxs-lookup"><span data-stu-id="bacd2-155">Request</span></span>
<span data-ttu-id="bacd2-156">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bacd2-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
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

### <a name="response"></a><span data-ttu-id="bacd2-157">Ответ</span><span class="sxs-lookup"><span data-stu-id="bacd2-157">Response</span></span>
<span data-ttu-id="bacd2-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="bacd2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



