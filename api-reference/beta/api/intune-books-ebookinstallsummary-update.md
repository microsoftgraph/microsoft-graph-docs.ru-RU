---
title: Update eBookInstallSummary
description: Обновление свойств объекта eBookInstallSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9a16e670fdb68283539b14085200b761aae2462b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934382"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="3e7a7-103">Update eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="3e7a7-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="3e7a7-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e7a7-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e7a7-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e7a7-107">Обновление свойств объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3e7a7-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3e7a7-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7a7-108">Prerequisites</span></span>
<span data-ttu-id="3e7a7-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3e7a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3e7a7-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3e7a7-111">Permission type</span></span>|<span data-ttu-id="3e7a7-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3e7a7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3e7a7-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3e7a7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3e7a7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e7a7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3e7a7-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3e7a7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3e7a7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-116">Not supported.</span></span>|
|<span data-ttu-id="3e7a7-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3e7a7-117">Application</span></span>|<span data-ttu-id="3e7a7-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3e7a7-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3e7a7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="3e7a7-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3e7a7-120">Request headers</span></span>
|<span data-ttu-id="3e7a7-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3e7a7-121">Header</span></span>|<span data-ttu-id="3e7a7-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3e7a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3e7a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e7a7-123">Authorization</span></span>|<span data-ttu-id="3e7a7-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3e7a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3e7a7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3e7a7-125">Accept</span></span>|<span data-ttu-id="3e7a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3e7a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e7a7-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3e7a7-127">Request body</span></span>
<span data-ttu-id="3e7a7-128">В теле запроса добавьте представление объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="3e7a7-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span><span class="sxs-lookup"><span data-stu-id="3e7a7-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="3e7a7-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e7a7-130">Property</span></span>|<span data-ttu-id="3e7a7-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3e7a7-131">Type</span></span>|<span data-ttu-id="3e7a7-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3e7a7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e7a7-133">id</span><span class="sxs-lookup"><span data-stu-id="3e7a7-133">id</span></span>|<span data-ttu-id="3e7a7-134">Строка</span><span class="sxs-lookup"><span data-stu-id="3e7a7-134">String</span></span>|<span data-ttu-id="3e7a7-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-135">Key of the entity.</span></span>|
|<span data-ttu-id="3e7a7-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e7a7-136">installedDeviceCount</span></span>|<span data-ttu-id="3e7a7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3e7a7-137">Int32</span></span>|<span data-ttu-id="3e7a7-138">Количество устройств, на которых была успешно установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="3e7a7-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e7a7-139">failedDeviceCount</span></span>|<span data-ttu-id="3e7a7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3e7a7-140">Int32</span></span>|<span data-ttu-id="3e7a7-141">Количество устройств, на которых не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="3e7a7-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3e7a7-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="3e7a7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3e7a7-143">Int32</span></span>|<span data-ttu-id="3e7a7-144">Количество устройств, на которых не установлена эта книга.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="3e7a7-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="3e7a7-145">installedUserCount</span></span>|<span data-ttu-id="3e7a7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3e7a7-146">Int32</span></span>|<span data-ttu-id="3e7a7-147">Количество пользователей, которым удалось установить эту книгу на всех своих устройствах.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="3e7a7-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="3e7a7-148">failedUserCount</span></span>|<span data-ttu-id="3e7a7-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3e7a7-149">Int32</span></span>|<span data-ttu-id="3e7a7-150">Количество пользователей, у которых есть одно или несколько устройств, где не удалось установить эту книгу.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="3e7a7-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="3e7a7-151">notInstalledUserCount</span></span>|<span data-ttu-id="3e7a7-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3e7a7-152">Int32</span></span>|<span data-ttu-id="3e7a7-153">Количество пользователей, не установивших эту книгу.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="3e7a7-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e7a7-154">Response</span></span>
<span data-ttu-id="3e7a7-155">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e7a7-156">Пример</span><span class="sxs-lookup"><span data-stu-id="3e7a7-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="3e7a7-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="3e7a7-157">Request</span></span>
<span data-ttu-id="3e7a7-158">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="3e7a7-159">Ответ</span><span class="sxs-lookup"><span data-stu-id="3e7a7-159">Response</span></span>
<span data-ttu-id="3e7a7-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3e7a7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





