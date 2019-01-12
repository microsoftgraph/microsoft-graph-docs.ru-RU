---
title: Создание объекта userInstallStateSummary
description: Создание объекта userInstallStateSummary.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b738e79c832fbfde23bfa48a84573c6d5c8f3e98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950258"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="4c516-103">Создание объекта userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="4c516-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="4c516-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4c516-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c516-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c516-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c516-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4c516-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c516-107">Создание объекта [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span><span class="sxs-lookup"><span data-stu-id="4c516-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c516-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="4c516-108">Prerequisites</span></span>
<span data-ttu-id="4c516-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4c516-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c516-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4c516-111">Permission type</span></span>|<span data-ttu-id="4c516-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="4c516-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c516-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4c516-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c516-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c516-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c516-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4c516-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c516-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c516-116">Not supported.</span></span>|
|<span data-ttu-id="4c516-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4c516-117">Application</span></span>|<span data-ttu-id="4c516-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c516-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c516-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4c516-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="4c516-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4c516-120">Request headers</span></span>
|<span data-ttu-id="4c516-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="4c516-121">Header</span></span>|<span data-ttu-id="4c516-122">Значение</span><span class="sxs-lookup"><span data-stu-id="4c516-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c516-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c516-123">Authorization</span></span>|<span data-ttu-id="4c516-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="4c516-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c516-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c516-125">Accept</span></span>|<span data-ttu-id="4c516-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c516-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c516-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4c516-127">Request body</span></span>
<span data-ttu-id="4c516-128">В тексте запроса добавьте представление объекта userInstallStateSummary в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c516-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="4c516-129">В таблице ниже приведены свойства, которые необходимо указывать при создании объекта userInstallStateSummary.</span><span class="sxs-lookup"><span data-stu-id="4c516-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="4c516-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c516-130">Property</span></span>|<span data-ttu-id="4c516-131">Тип</span><span class="sxs-lookup"><span data-stu-id="4c516-131">Type</span></span>|<span data-ttu-id="4c516-132">Описание</span><span class="sxs-lookup"><span data-stu-id="4c516-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c516-133">id</span><span class="sxs-lookup"><span data-stu-id="4c516-133">id</span></span>|<span data-ttu-id="4c516-134">String</span><span class="sxs-lookup"><span data-stu-id="4c516-134">String</span></span>|<span data-ttu-id="4c516-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="4c516-135">Key of the entity.</span></span>|
|<span data-ttu-id="4c516-136">userName</span><span class="sxs-lookup"><span data-stu-id="4c516-136">userName</span></span>|<span data-ttu-id="4c516-137">String</span><span class="sxs-lookup"><span data-stu-id="4c516-137">String</span></span>|<span data-ttu-id="4c516-138">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="4c516-138">User name.</span></span>|
|<span data-ttu-id="4c516-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c516-139">installedDeviceCount</span></span>|<span data-ttu-id="4c516-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4c516-140">Int32</span></span>|<span data-ttu-id="4c516-141">Количество установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="4c516-141">Installed Device Count.</span></span>|
|<span data-ttu-id="4c516-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c516-142">failedDeviceCount</span></span>|<span data-ttu-id="4c516-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4c516-143">Int32</span></span>|<span data-ttu-id="4c516-144">Количество устройств со сбоями.</span><span class="sxs-lookup"><span data-stu-id="4c516-144">Failed Device Count.</span></span>|
|<span data-ttu-id="4c516-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c516-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="4c516-146">Int32</span><span class="sxs-lookup"><span data-stu-id="4c516-146">Int32</span></span>|<span data-ttu-id="4c516-147">Количество не установленных устройств.</span><span class="sxs-lookup"><span data-stu-id="4c516-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="4c516-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c516-148">Response</span></span>
<span data-ttu-id="4c516-149">В случае успешного выполнения этот метод возвращает код отклика `201 Created` и объект [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4c516-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c516-150">Пример</span><span class="sxs-lookup"><span data-stu-id="4c516-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c516-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="4c516-151">Request</span></span>
<span data-ttu-id="4c516-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4c516-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c516-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="4c516-153">Response</span></span>
<span data-ttu-id="4c516-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4c516-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





