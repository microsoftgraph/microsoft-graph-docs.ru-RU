---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3401ae8c2a33e56e69121b5704cc2e45905429be
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422700"
---
# <a name="update-user"></a><span data-ttu-id="20612-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="20612-103">Update user</span></span>

> <span data-ttu-id="20612-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="20612-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="20612-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20612-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20612-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="20612-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20612-107">Обновление свойств объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="20612-107">Update the properties of a [user](../resources/intune-shared-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20612-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="20612-108">Prerequisites</span></span>

<span data-ttu-id="20612-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20612-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20612-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="20612-111">Permission type</span></span>|<span data-ttu-id="20612-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="20612-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20612-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="20612-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="20612-114">&nbsp; &nbsp; **Управление устройствами**</span><span class="sxs-lookup"><span data-stu-id="20612-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="20612-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20612-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
| <span data-ttu-id="20612-116">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="20612-116">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="20612-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20612-117">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="20612-118">&nbsp;&nbsp; **Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="20612-118">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="20612-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20612-119">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
| <span data-ttu-id="20612-120">&nbsp; &nbsp; **Устранение неполадок**</span><span class="sxs-lookup"><span data-stu-id="20612-120">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="20612-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20612-121">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="20612-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="20612-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20612-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20612-123">Not supported.</span></span>|
|<span data-ttu-id="20612-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="20612-124">Application</span></span>|<span data-ttu-id="20612-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="20612-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20612-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="20612-126">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="20612-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="20612-127">Request headers</span></span>

|<span data-ttu-id="20612-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="20612-128">Header</span></span>|<span data-ttu-id="20612-129">Значение</span><span class="sxs-lookup"><span data-stu-id="20612-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20612-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="20612-130">Authorization</span></span>|<span data-ttu-id="20612-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="20612-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20612-132">Accept</span><span class="sxs-lookup"><span data-stu-id="20612-132">Accept</span></span>|<span data-ttu-id="20612-133">application/json</span><span class="sxs-lookup"><span data-stu-id="20612-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20612-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="20612-134">Request body</span></span>

<span data-ttu-id="20612-135">В теле запроса добавьте представление объекта [user](../resources/intune-shared-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="20612-135">In the request body, supply a JSON representation for the [user](../resources/intune-shared-user.md) object.</span></span>

<span data-ttu-id="20612-136">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="20612-136">The following table shows the properties that are required when you create the [user](../resources/intune-shared-user.md).</span></span>

|<span data-ttu-id="20612-137">Свойство</span><span class="sxs-lookup"><span data-stu-id="20612-137">Property</span></span>|<span data-ttu-id="20612-138">Тип</span><span class="sxs-lookup"><span data-stu-id="20612-138">Type</span></span>|<span data-ttu-id="20612-139">Описание</span><span class="sxs-lookup"><span data-stu-id="20612-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20612-140">id</span><span class="sxs-lookup"><span data-stu-id="20612-140">id</span></span>|<span data-ttu-id="20612-141">String</span><span class="sxs-lookup"><span data-stu-id="20612-141">String</span></span>|<span data-ttu-id="20612-142">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="20612-142">Unique identifier of the user.</span></span>|
|<span data-ttu-id="20612-143">**Адаптация новых сотрудников**</span><span class="sxs-lookup"><span data-stu-id="20612-143">**Onboarding**</span></span>|
|<span data-ttu-id="20612-144">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="20612-144">deviceEnrollmentLimit</span></span>|<span data-ttu-id="20612-145">Int32</span><span class="sxs-lookup"><span data-stu-id="20612-145">Int32</span></span>|<span data-ttu-id="20612-146">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="20612-146">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="20612-147">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="20612-147">Allowed values are 5 or 1000.</span></span>|

## <a name="response"></a><span data-ttu-id="20612-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="20612-148">Response</span></span>

<span data-ttu-id="20612-149">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-shared-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="20612-149">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-shared-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20612-150">Пример</span><span class="sxs-lookup"><span data-stu-id="20612-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="20612-151">Запрос</span><span class="sxs-lookup"><span data-stu-id="20612-151">Request</span></span>

<span data-ttu-id="20612-152">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="20612-152">Here is an example of the request.</span></span>

``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="20612-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="20612-153">Response</span></span>

<span data-ttu-id="20612-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="20612-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



