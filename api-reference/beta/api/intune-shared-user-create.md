---
title: Создание пользователя
description: Создание объекта user.
ms.openlocfilehash: 827f8ea7fd9261dbf8dab87f6fc01c608bf900cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079066"
---
# <a name="create-user"></a><span data-ttu-id="27a4a-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="27a4a-103">Create user</span></span>

> <span data-ttu-id="27a4a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="27a4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27a4a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27a4a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="27a4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27a4a-107">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="27a4a-107">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27a4a-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="27a4a-108">Prerequisites</span></span>

<span data-ttu-id="27a4a-109">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="27a4a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="27a4a-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27a4a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="27a4a-111">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="27a4a-111">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="27a4a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27a4a-112">Permission type</span></span>|<span data-ttu-id="27a4a-113">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="27a4a-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27a4a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27a4a-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="27a4a-115">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="27a4a-115">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="27a4a-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a4a-116">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="27a4a-117">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="27a4a-117">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="27a4a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a4a-118">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="27a4a-119">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="27a4a-119">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="27a4a-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a4a-120">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="27a4a-121">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="27a4a-121">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="27a4a-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27a4a-122">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="27a4a-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27a4a-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27a4a-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a4a-124">Not supported.</span></span>|
|<span data-ttu-id="27a4a-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27a4a-125">Application</span></span>|<span data-ttu-id="27a4a-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27a4a-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27a4a-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27a4a-127">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="27a4a-128">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27a4a-128">Request headers</span></span>

|<span data-ttu-id="27a4a-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="27a4a-129">Header</span></span>|<span data-ttu-id="27a4a-130">Значение</span><span class="sxs-lookup"><span data-stu-id="27a4a-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27a4a-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="27a4a-131">Authorization</span></span>|<span data-ttu-id="27a4a-132">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="27a4a-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27a4a-133">Accept</span><span class="sxs-lookup"><span data-stu-id="27a4a-133">Accept</span></span>|<span data-ttu-id="27a4a-134">application/json</span><span class="sxs-lookup"><span data-stu-id="27a4a-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27a4a-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="27a4a-135">Request body</span></span>

<span data-ttu-id="27a4a-136">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27a4a-136">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="27a4a-137">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="27a4a-137">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="27a4a-138">Свойство</span><span class="sxs-lookup"><span data-stu-id="27a4a-138">Property</span></span>|<span data-ttu-id="27a4a-139">Тип</span><span class="sxs-lookup"><span data-stu-id="27a4a-139">Type</span></span>|<span data-ttu-id="27a4a-140">Описание</span><span class="sxs-lookup"><span data-stu-id="27a4a-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27a4a-141">id</span><span class="sxs-lookup"><span data-stu-id="27a4a-141">id</span></span>|<span data-ttu-id="27a4a-142">String</span><span class="sxs-lookup"><span data-stu-id="27a4a-142">String</span></span>|<span data-ttu-id="27a4a-143">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="27a4a-143">Unique identifier of the user.</span></span>|
|<span data-ttu-id="27a4a-144">**На использование доски**</span><span class="sxs-lookup"><span data-stu-id="27a4a-144">**On-boarding**</span></span>||
|<span data-ttu-id="27a4a-145">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="27a4a-145">deviceEnrollmentLimit</span></span>|<span data-ttu-id="27a4a-146">Int32</span><span class="sxs-lookup"><span data-stu-id="27a4a-146">Int32</span></span>|<span data-ttu-id="27a4a-147">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="27a4a-147">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="27a4a-148">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="27a4a-148">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="27a4a-149">Поддержка свойств текст запроса изменяется в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="27a4a-149">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="27a4a-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="27a4a-150">Response</span></span>

<span data-ttu-id="27a4a-151">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="27a4a-151">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27a4a-152">Пример</span><span class="sxs-lookup"><span data-stu-id="27a4a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="27a4a-153">Запрос</span><span class="sxs-lookup"><span data-stu-id="27a4a-153">Request</span></span>

<span data-ttu-id="27a4a-154">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27a4a-154">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="27a4a-155">Ответ</span><span class="sxs-lookup"><span data-stu-id="27a4a-155">Response</span></span>

<span data-ttu-id="27a4a-156">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27a4a-156">Here is an example of the response.</span></span> <span data-ttu-id="27a4a-157">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="27a4a-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="27a4a-158">Свойства, возвращенные фактический вызов различаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="27a4a-158">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



