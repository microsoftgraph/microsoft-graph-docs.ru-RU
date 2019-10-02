---
title: Создание пользователя
description: Создание объекта user.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8cbdb53286d427223d80bf8b55cef63cbf0416a4
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361331"
---
# <a name="create-user"></a><span data-ttu-id="5e74e-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="5e74e-103">Create user</span></span>

> <span data-ttu-id="5e74e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5e74e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5e74e-105">Создание объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="5e74e-105">Create a new [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5e74e-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="5e74e-106">Prerequisites</span></span>
<span data-ttu-id="5e74e-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="5e74e-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5e74e-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5e74e-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="5e74e-109">Конкретное требуемое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="5e74e-109">The specific permission required depends on the context.</span></span>

|<span data-ttu-id="5e74e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5e74e-110">Permission type</span></span>|<span data-ttu-id="5e74e-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="5e74e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e74e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5e74e-112">Delegated (work or school account)</span></span>| <span data-ttu-id="5e74e-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="5e74e-113">_varies by context_</span></span> |
| <span data-ttu-id="5e74e-114">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="5e74e-114">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="5e74e-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e74e-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="5e74e-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="5e74e-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="5e74e-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e74e-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="5e74e-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="5e74e-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="5e74e-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e74e-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="5e74e-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="5e74e-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="5e74e-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e74e-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="5e74e-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5e74e-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e74e-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e74e-123">Not supported.</span></span>|
|<span data-ttu-id="5e74e-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5e74e-124">Application</span></span>|<span data-ttu-id="5e74e-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5e74e-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e74e-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5e74e-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="5e74e-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5e74e-127">Request headers</span></span>
|<span data-ttu-id="5e74e-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="5e74e-128">Header</span></span>|<span data-ttu-id="5e74e-129">Значение</span><span class="sxs-lookup"><span data-stu-id="5e74e-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e74e-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5e74e-130">Authorization</span></span>|<span data-ttu-id="5e74e-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5e74e-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e74e-132">Accept</span><span class="sxs-lookup"><span data-stu-id="5e74e-132">Accept</span></span>|<span data-ttu-id="5e74e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="5e74e-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e74e-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5e74e-134">Request body</span></span>
<span data-ttu-id="5e74e-135">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e74e-135">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="5e74e-136">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="5e74e-136">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="5e74e-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e74e-137">Property</span></span>|<span data-ttu-id="5e74e-138">Тип</span><span class="sxs-lookup"><span data-stu-id="5e74e-138">Type</span></span>|<span data-ttu-id="5e74e-139">Описание</span><span class="sxs-lookup"><span data-stu-id="5e74e-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e74e-140">id</span><span class="sxs-lookup"><span data-stu-id="5e74e-140">id</span></span>|<span data-ttu-id="5e74e-141">String</span><span class="sxs-lookup"><span data-stu-id="5e74e-141">String</span></span>|<span data-ttu-id="5e74e-142">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e74e-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="5e74e-143">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="5e74e-143">**Onboarding**</span></span>|
|<span data-ttu-id="5e74e-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="5e74e-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="5e74e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5e74e-145">Int32</span></span>|<span data-ttu-id="5e74e-146">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="5e74e-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="5e74e-147">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="5e74e-147">Allowed values are 5 or 1000.</span></span>|

<span data-ttu-id="5e74e-148">Поддержка свойств текста запроса зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="5e74e-148">Request body property support varies according to context.</span></span>

## <a name="response"></a><span data-ttu-id="5e74e-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e74e-149">Response</span></span>
<span data-ttu-id="5e74e-150">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="5e74e-150">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e74e-151">Пример</span><span class="sxs-lookup"><span data-stu-id="5e74e-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="5e74e-152">Запрос</span><span class="sxs-lookup"><span data-stu-id="5e74e-152">Request</span></span>
<span data-ttu-id="5e74e-153">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5e74e-153">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="5e74e-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="5e74e-154">Response</span></span>
<span data-ttu-id="5e74e-155">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5e74e-155">Here is an example of the response.</span></span> <span data-ttu-id="5e74e-156">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="5e74e-156">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="5e74e-157">Свойства, возвращаемые при фактическом вызове, меняются в зависимости от контекста.</span><span class="sxs-lookup"><span data-stu-id="5e74e-157">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




