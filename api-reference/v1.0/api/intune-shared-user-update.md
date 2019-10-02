---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 944930fcb5eb046908fe157713a486845322e2cc
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361233"
---
# <a name="update-user"></a><span data-ttu-id="733ab-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="733ab-103">Update user</span></span>

> <span data-ttu-id="733ab-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="733ab-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="733ab-105">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="733ab-105">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="733ab-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="733ab-106">Prerequisites</span></span>
<span data-ttu-id="733ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="733ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="733ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="733ab-109">Permission type</span></span>|<span data-ttu-id="733ab-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="733ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="733ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="733ab-111">Delegated (work or school account)</span></span>| <span data-ttu-id="733ab-112">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="733ab-112">_varies by context_</span></span>|
| <span data-ttu-id="733ab-113">&nbsp;&nbsp; Управление устройствами</span><span class="sxs-lookup"><span data-stu-id="733ab-113">&nbsp; &nbsp; Device management</span></span> | <span data-ttu-id="733ab-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="733ab-114">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="733ab-115">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="733ab-115">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="733ab-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="733ab-116">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="733ab-117">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="733ab-117">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="733ab-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="733ab-118">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="733ab-119">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="733ab-119">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="733ab-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="733ab-120">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="733ab-121">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="733ab-121">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="733ab-122">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="733ab-122">Not supported.</span></span>|
|<span data-ttu-id="733ab-123">Для приложений</span><span class="sxs-lookup"><span data-stu-id="733ab-123">Application</span></span>|<span data-ttu-id="733ab-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="733ab-124">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="733ab-125">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="733ab-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="733ab-126">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="733ab-126">Request headers</span></span>
|<span data-ttu-id="733ab-127">Заголовок</span><span class="sxs-lookup"><span data-stu-id="733ab-127">Header</span></span>|<span data-ttu-id="733ab-128">Значение</span><span class="sxs-lookup"><span data-stu-id="733ab-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="733ab-129">Авторизация</span><span class="sxs-lookup"><span data-stu-id="733ab-129">Authorization</span></span>|<span data-ttu-id="733ab-130">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="733ab-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="733ab-131">Accept</span><span class="sxs-lookup"><span data-stu-id="733ab-131">Accept</span></span>|<span data-ttu-id="733ab-132">application/json</span><span class="sxs-lookup"><span data-stu-id="733ab-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="733ab-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="733ab-133">Request body</span></span>
<span data-ttu-id="733ab-134">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="733ab-134">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="733ab-135">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="733ab-135">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="733ab-136">Свойство</span><span class="sxs-lookup"><span data-stu-id="733ab-136">Property</span></span>|<span data-ttu-id="733ab-137">Тип</span><span class="sxs-lookup"><span data-stu-id="733ab-137">Type</span></span>|<span data-ttu-id="733ab-138">Описание</span><span class="sxs-lookup"><span data-stu-id="733ab-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="733ab-139">id</span><span class="sxs-lookup"><span data-stu-id="733ab-139">id</span></span>|<span data-ttu-id="733ab-140">String</span><span class="sxs-lookup"><span data-stu-id="733ab-140">String</span></span>|<span data-ttu-id="733ab-141">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="733ab-141">Unique identifier of the user.</span></span>|
|<span data-ttu-id="733ab-142">**Входящая миграция**</span><span class="sxs-lookup"><span data-stu-id="733ab-142">**Onboarding**</span></span>|
|<span data-ttu-id="733ab-143">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="733ab-143">deviceEnrollmentLimit</span></span>|<span data-ttu-id="733ab-144">Int32</span><span class="sxs-lookup"><span data-stu-id="733ab-144">Int32</span></span>|<span data-ttu-id="733ab-145">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="733ab-145">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="733ab-146">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="733ab-146">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="733ab-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="733ab-147">Response</span></span>
<span data-ttu-id="733ab-148">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="733ab-148">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="733ab-149">Пример</span><span class="sxs-lookup"><span data-stu-id="733ab-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="733ab-150">Запрос</span><span class="sxs-lookup"><span data-stu-id="733ab-150">Request</span></span>
<span data-ttu-id="733ab-151">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="733ab-151">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="733ab-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="733ab-152">Response</span></span>
<span data-ttu-id="733ab-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="733ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




