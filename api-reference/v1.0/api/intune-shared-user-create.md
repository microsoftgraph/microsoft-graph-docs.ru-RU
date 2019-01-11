---
title: Создание пользователя
description: Создание объекта user.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3d654f287478b140f64f14a4814850a4c9d19ff7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866670"
---
# <a name="create-user"></a><span data-ttu-id="6bf5a-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="6bf5a-103">Create user</span></span>

> <span data-ttu-id="6bf5a-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bf5a-105">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="6bf5a-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6bf5a-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="6bf5a-106">Prerequisites</span></span>
<span data-ttu-id="6bf5a-107">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6bf5a-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6bf5a-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="6bf5a-109">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="6bf5a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6bf5a-110">Permission type</span></span>|<span data-ttu-id="6bf5a-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6bf5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6bf5a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6bf5a-112">Delegated (work or school account)</span></span>| <span data-ttu-id="6bf5a-113">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="6bf5a-113">_varies by context_</span></span> |
| <span data-ttu-id="6bf5a-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="6bf5a-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="6bf5a-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf5a-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="6bf5a-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="6bf5a-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="6bf5a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf5a-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="6bf5a-118">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="6bf5a-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="6bf5a-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf5a-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="6bf5a-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="6bf5a-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="6bf5a-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6bf5a-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="6bf5a-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6bf5a-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6bf5a-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-123">Not supported.</span></span>|
|<span data-ttu-id="6bf5a-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6bf5a-124">Application</span></span>|<span data-ttu-id="6bf5a-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6bf5a-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6bf5a-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="6bf5a-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6bf5a-127">Request headers</span></span>
|<span data-ttu-id="6bf5a-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6bf5a-128">Header</span></span>|<span data-ttu-id="6bf5a-129">Значение</span><span class="sxs-lookup"><span data-stu-id="6bf5a-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6bf5a-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6bf5a-130">Authorization</span></span>|<span data-ttu-id="6bf5a-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6bf5a-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6bf5a-132">Accept</span><span class="sxs-lookup"><span data-stu-id="6bf5a-132">Accept</span></span>|<span data-ttu-id="6bf5a-133">application/json</span><span class="sxs-lookup"><span data-stu-id="6bf5a-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6bf5a-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6bf5a-134">Request body</span></span>
<span data-ttu-id="6bf5a-135">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="6bf5a-136">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="6bf5a-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bf5a-137">Property</span></span>|<span data-ttu-id="6bf5a-138">Тип</span><span class="sxs-lookup"><span data-stu-id="6bf5a-138">Type</span></span>|<span data-ttu-id="6bf5a-139">Описание</span><span class="sxs-lookup"><span data-stu-id="6bf5a-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6bf5a-140">id</span><span class="sxs-lookup"><span data-stu-id="6bf5a-140">id</span></span>|<span data-ttu-id="6bf5a-141">String</span><span class="sxs-lookup"><span data-stu-id="6bf5a-141">String</span></span>|<span data-ttu-id="6bf5a-142">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="6bf5a-143">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="6bf5a-143">**Onboarding**</span></span>|
|<span data-ttu-id="6bf5a-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="6bf5a-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="6bf5a-145">Int32</span><span class="sxs-lookup"><span data-stu-id="6bf5a-145">Int32</span></span>|<span data-ttu-id="6bf5a-146">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="6bf5a-147">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="6bf5a-148">Поддержка свойств текст запроса изменяется в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="6bf5a-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="6bf5a-149">Response</span></span>
<span data-ttu-id="6bf5a-150">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6bf5a-151">Пример</span><span class="sxs-lookup"><span data-stu-id="6bf5a-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="6bf5a-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="6bf5a-152">Request</span></span>
<span data-ttu-id="6bf5a-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="6bf5a-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="6bf5a-154">Response</span></span>
<span data-ttu-id="6bf5a-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-155">Here is an example of the response.</span></span> <span data-ttu-id="6bf5a-156">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6bf5a-157">Свойства, возвращенные фактический вызов различаться в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="6bf5a-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



