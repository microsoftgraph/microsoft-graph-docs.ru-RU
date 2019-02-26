---
title: Создание пользователя
description: Создание объекта user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 95b01b4b00328c230d55b530cbdef2cb32dfe607
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250231"
---
# <a name="create-user"></a><span data-ttu-id="64e06-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="64e06-103">Create user</span></span>

> <span data-ttu-id="64e06-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="64e06-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64e06-105">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="64e06-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64e06-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="64e06-106">Prerequisites</span></span>
<span data-ttu-id="64e06-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="64e06-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="64e06-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64e06-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="64e06-109">Конкретное требуемое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="64e06-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="64e06-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64e06-110">Permission type</span></span>|<span data-ttu-id="64e06-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="64e06-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64e06-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64e06-112">Delegated (work or school account)</span></span>| <span data-ttu-id="64e06-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="64e06-113">_varies by context_</span></span> |
| <span data-ttu-id="64e06-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="64e06-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="64e06-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e06-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="64e06-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="64e06-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="64e06-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e06-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="64e06-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="64e06-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="64e06-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e06-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="64e06-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="64e06-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="64e06-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e06-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="64e06-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64e06-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64e06-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64e06-123">Not supported.</span></span>|
|<span data-ttu-id="64e06-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64e06-124">Application</span></span>|<span data-ttu-id="64e06-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64e06-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64e06-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64e06-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="64e06-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64e06-127">Request headers</span></span>
|<span data-ttu-id="64e06-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="64e06-128">Header</span></span>|<span data-ttu-id="64e06-129">Значение</span><span class="sxs-lookup"><span data-stu-id="64e06-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64e06-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="64e06-130">Authorization</span></span>|<span data-ttu-id="64e06-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="64e06-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64e06-132">Accept</span><span class="sxs-lookup"><span data-stu-id="64e06-132">Accept</span></span>|<span data-ttu-id="64e06-133">application/json</span><span class="sxs-lookup"><span data-stu-id="64e06-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64e06-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="64e06-134">Request body</span></span>
<span data-ttu-id="64e06-135">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64e06-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="64e06-136">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="64e06-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="64e06-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="64e06-137">Property</span></span>|<span data-ttu-id="64e06-138">Тип</span><span class="sxs-lookup"><span data-stu-id="64e06-138">Type</span></span>|<span data-ttu-id="64e06-139">Описание</span><span class="sxs-lookup"><span data-stu-id="64e06-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e06-140">id</span><span class="sxs-lookup"><span data-stu-id="64e06-140">id</span></span>|<span data-ttu-id="64e06-141">String</span><span class="sxs-lookup"><span data-stu-id="64e06-141">String</span></span>|<span data-ttu-id="64e06-142">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="64e06-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="64e06-143">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="64e06-143">**Onboarding**</span></span>|
|<span data-ttu-id="64e06-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="64e06-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="64e06-145">Int32</span><span class="sxs-lookup"><span data-stu-id="64e06-145">Int32</span></span>|<span data-ttu-id="64e06-146">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="64e06-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="64e06-147">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="64e06-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="64e06-148">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="64e06-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="64e06-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="64e06-149">Response</span></span>
<span data-ttu-id="64e06-150">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="64e06-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64e06-151">Пример</span><span class="sxs-lookup"><span data-stu-id="64e06-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="64e06-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="64e06-152">Request</span></span>
<span data-ttu-id="64e06-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64e06-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="64e06-154">Ответ</span><span class="sxs-lookup"><span data-stu-id="64e06-154">Response</span></span>
<span data-ttu-id="64e06-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="64e06-155">Here is an example of the response.</span></span> <span data-ttu-id="64e06-156">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="64e06-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="64e06-157">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="64e06-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



