---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
ms.openlocfilehash: cfb8a7d46d8383cdaae4f012cff4ed0a0ad93594
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026883"
---
# <a name="update-user"></a><span data-ttu-id="02e8e-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="02e8e-103">Update user</span></span>

> <span data-ttu-id="02e8e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="02e8e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02e8e-105">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="02e8e-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02e8e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="02e8e-106">Prerequisites</span></span>
<span data-ttu-id="02e8e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02e8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02e8e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="02e8e-109">Permission type</span></span>|<span data-ttu-id="02e8e-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="02e8e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02e8e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="02e8e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="02e8e-112">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="02e8e-112">_varies by context_</span></span>|
| <span data-ttu-id="02e8e-113">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="02e8e-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="02e8e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e8e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="02e8e-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="02e8e-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="02e8e-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e8e-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="02e8e-117">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="02e8e-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="02e8e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e8e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="02e8e-119">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="02e8e-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="02e8e-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02e8e-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="02e8e-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="02e8e-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02e8e-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02e8e-122">Not supported.</span></span>|
|<span data-ttu-id="02e8e-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="02e8e-123">Application</span></span>|<span data-ttu-id="02e8e-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02e8e-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02e8e-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="02e8e-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="02e8e-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="02e8e-126">Request headers</span></span>
|<span data-ttu-id="02e8e-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="02e8e-127">Header</span></span>|<span data-ttu-id="02e8e-128">Значение</span><span class="sxs-lookup"><span data-stu-id="02e8e-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02e8e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="02e8e-129">Authorization</span></span>|<span data-ttu-id="02e8e-130">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="02e8e-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02e8e-131">Accept</span><span class="sxs-lookup"><span data-stu-id="02e8e-131">Accept</span></span>|<span data-ttu-id="02e8e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="02e8e-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02e8e-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="02e8e-133">Request body</span></span>
<span data-ttu-id="02e8e-134">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02e8e-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="02e8e-135">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="02e8e-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="02e8e-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="02e8e-136">Property</span></span>|<span data-ttu-id="02e8e-137">Тип</span><span class="sxs-lookup"><span data-stu-id="02e8e-137">Type</span></span>|<span data-ttu-id="02e8e-138">Описание</span><span class="sxs-lookup"><span data-stu-id="02e8e-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02e8e-139">id</span><span class="sxs-lookup"><span data-stu-id="02e8e-139">id</span></span>|<span data-ttu-id="02e8e-140">String</span><span class="sxs-lookup"><span data-stu-id="02e8e-140">String</span></span>|<span data-ttu-id="02e8e-141">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="02e8e-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="02e8e-142">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="02e8e-142">**Onboarding**</span></span>|
|<span data-ttu-id="02e8e-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="02e8e-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="02e8e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="02e8e-144">Int32</span></span>|<span data-ttu-id="02e8e-145">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="02e8e-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="02e8e-146">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="02e8e-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="02e8e-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="02e8e-147">Response</span></span>
<span data-ttu-id="02e8e-148">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="02e8e-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02e8e-149">Пример</span><span class="sxs-lookup"><span data-stu-id="02e8e-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="02e8e-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="02e8e-150">Request</span></span>
<span data-ttu-id="02e8e-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="02e8e-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="02e8e-152">Ответ</span><span class="sxs-lookup"><span data-stu-id="02e8e-152">Response</span></span>
<span data-ttu-id="02e8e-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="02e8e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



