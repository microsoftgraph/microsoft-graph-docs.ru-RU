---
title: Обновление пользователя
description: Обновление свойств объекта пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8c807a52cf27c53813f82b70c908575b06f94e4b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753134"
---
# <a name="update-user"></a><span data-ttu-id="89e5d-103">Обновление пользователя</span><span class="sxs-lookup"><span data-stu-id="89e5d-103">Update user</span></span>

<span data-ttu-id="89e5d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89e5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89e5d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89e5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89e5d-106">Обновление свойств объекта [user](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="89e5d-106">Update the properties of a [user](../resources/intune-onboarding-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89e5d-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="89e5d-107">Prerequisites</span></span>
<span data-ttu-id="89e5d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89e5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89e5d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="89e5d-110">Permission type</span></span>|<span data-ttu-id="89e5d-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="89e5d-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89e5d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="89e5d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89e5d-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e5d-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="89e5d-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="89e5d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89e5d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="89e5d-115">Not supported.</span></span>|
|<span data-ttu-id="89e5d-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="89e5d-116">Application</span></span>|<span data-ttu-id="89e5d-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89e5d-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="89e5d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="89e5d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="89e5d-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="89e5d-119">Request headers</span></span>
|<span data-ttu-id="89e5d-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="89e5d-120">Header</span></span>|<span data-ttu-id="89e5d-121">Значение</span><span class="sxs-lookup"><span data-stu-id="89e5d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89e5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89e5d-122">Authorization</span></span>|<span data-ttu-id="89e5d-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="89e5d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89e5d-124">Accept</span><span class="sxs-lookup"><span data-stu-id="89e5d-124">Accept</span></span>|<span data-ttu-id="89e5d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89e5d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89e5d-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="89e5d-126">Request body</span></span>
<span data-ttu-id="89e5d-127">В теле запроса добавьте представление объекта [user](../resources/intune-onboarding-user.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89e5d-127">In the request body, supply a JSON representation for the [user](../resources/intune-onboarding-user.md) object.</span></span>

<span data-ttu-id="89e5d-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта [user](../resources/intune-onboarding-user.md).</span><span class="sxs-lookup"><span data-stu-id="89e5d-128">The following table shows the properties that are required when you create the [user](../resources/intune-onboarding-user.md).</span></span>

|<span data-ttu-id="89e5d-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="89e5d-129">Property</span></span>|<span data-ttu-id="89e5d-130">Тип</span><span class="sxs-lookup"><span data-stu-id="89e5d-130">Type</span></span>|<span data-ttu-id="89e5d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="89e5d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89e5d-132">id</span><span class="sxs-lookup"><span data-stu-id="89e5d-132">id</span></span>|<span data-ttu-id="89e5d-133">String</span><span class="sxs-lookup"><span data-stu-id="89e5d-133">String</span></span>|<span data-ttu-id="89e5d-134">Уникальный идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="89e5d-134">Unique identifier of the user.</span></span>|
|<span data-ttu-id="89e5d-135">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="89e5d-135">deviceEnrollmentLimit</span></span>|<span data-ttu-id="89e5d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="89e5d-136">Int32</span></span>|<span data-ttu-id="89e5d-137">Максимальное количество устройств, которые разрешено зарегистрировать пользователю.</span><span class="sxs-lookup"><span data-stu-id="89e5d-137">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="89e5d-138">Допустимые значения: 5 или 1000.</span><span class="sxs-lookup"><span data-stu-id="89e5d-138">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="89e5d-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="89e5d-139">Response</span></span>
<span data-ttu-id="89e5d-140">При успешном выполнении этот метод возвращает код отклика `200 OK` и обновленный объект [user](../resources/intune-onboarding-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="89e5d-140">If successful, this method returns a `200 OK` response code and an updated [user](../resources/intune-onboarding-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89e5d-141">Пример</span><span class="sxs-lookup"><span data-stu-id="89e5d-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="89e5d-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="89e5d-142">Request</span></span>
<span data-ttu-id="89e5d-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="89e5d-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.user",
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="89e5d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="89e5d-144">Response</span></span>
<span data-ttu-id="89e5d-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="89e5d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```




