---
title: Создание пользователя
description: Создание объекта user.
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85487883069c7456da3404dce7e013c166bbe790
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195785"
---
# <a name="create-user"></a><span data-ttu-id="af17d-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="af17d-103">Create user</span></span>

> <span data-ttu-id="af17d-104">**Важно!** API в версии/Beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="af17d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="af17d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af17d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af17d-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af17d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af17d-107">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="af17d-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="af17d-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="af17d-108">Prerequisites</span></span>

<span data-ttu-id="af17d-109">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="af17d-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="af17d-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="af17d-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="af17d-111">Конкретное требуемое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="af17d-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="af17d-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="af17d-112">Permission type</span></span>|<span data-ttu-id="af17d-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="af17d-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af17d-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="af17d-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="af17d-115">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="af17d-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="af17d-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af17d-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="af17d-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="af17d-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="af17d-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af17d-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="af17d-119">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="af17d-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="af17d-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af17d-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="af17d-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="af17d-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="af17d-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af17d-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af17d-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="af17d-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af17d-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af17d-124">Not supported.</span></span>|
|<span data-ttu-id="af17d-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="af17d-125">Application</span></span>||
| <span data-ttu-id="af17d-126">&nbsp;&nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="af17d-126">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="af17d-127">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af17d-127">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="af17d-128">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="af17d-128">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="af17d-129">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af17d-129">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="af17d-130">&nbsp; &nbsp; **Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="af17d-130">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="af17d-131">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af17d-131">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="af17d-132">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="af17d-132">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="af17d-133">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af17d-133">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="af17d-134">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="af17d-134">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="af17d-135">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="af17d-135">Request headers</span></span>

|<span data-ttu-id="af17d-136">Заголовок</span><span class="sxs-lookup"><span data-stu-id="af17d-136">Header</span></span>|<span data-ttu-id="af17d-137">Значение</span><span class="sxs-lookup"><span data-stu-id="af17d-137">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af17d-138">Авторизация</span><span class="sxs-lookup"><span data-stu-id="af17d-138">Authorization</span></span>|<span data-ttu-id="af17d-139">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="af17d-139">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af17d-140">Accept</span><span class="sxs-lookup"><span data-stu-id="af17d-140">Accept</span></span>|<span data-ttu-id="af17d-141">application/json</span><span class="sxs-lookup"><span data-stu-id="af17d-141">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af17d-142">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="af17d-142">Request body</span></span>

<span data-ttu-id="af17d-143">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af17d-143">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="af17d-144">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="af17d-144">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="af17d-145">Свойство</span><span class="sxs-lookup"><span data-stu-id="af17d-145">Property</span></span>|<span data-ttu-id="af17d-146">Тип</span><span class="sxs-lookup"><span data-stu-id="af17d-146">Type</span></span>|<span data-ttu-id="af17d-147">Описание</span><span class="sxs-lookup"><span data-stu-id="af17d-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af17d-148">id</span><span class="sxs-lookup"><span data-stu-id="af17d-148">id</span></span>|<span data-ttu-id="af17d-149">String</span><span class="sxs-lookup"><span data-stu-id="af17d-149">String</span></span>|<span data-ttu-id="af17d-150">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="af17d-150">Unique identifier of the user.</span></span>|
|<span data-ttu-id="af17d-151">**Встроенное подключение**</span><span class="sxs-lookup"><span data-stu-id="af17d-151">**On-boarding**</span></span>||
|<span data-ttu-id="af17d-152">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="af17d-152">deviceEnrollmentLimit</span></span>|<span data-ttu-id="af17d-153">Int32</span><span class="sxs-lookup"><span data-stu-id="af17d-153">Int32</span></span>|<span data-ttu-id="af17d-154">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="af17d-154">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="af17d-155">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="af17d-155">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="af17d-156">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="af17d-156">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="af17d-157">Отклик</span><span class="sxs-lookup"><span data-stu-id="af17d-157">Response</span></span>

<span data-ttu-id="af17d-158">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="af17d-158">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af17d-159">Пример</span><span class="sxs-lookup"><span data-stu-id="af17d-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="af17d-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="af17d-160">Request</span></span>

<span data-ttu-id="af17d-161">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="af17d-161">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="af17d-162">Отклик</span><span class="sxs-lookup"><span data-stu-id="af17d-162">Response</span></span>

<span data-ttu-id="af17d-163">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="af17d-163">Here is an example of the response.</span></span> <span data-ttu-id="af17d-164">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="af17d-164">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="af17d-165">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="af17d-165">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```







