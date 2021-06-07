---
title: Создание пользователя
description: Создание объекта user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce928fd6f7de939a0edc708ddf5f6cab9dc60355
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756516"
---
# <a name="create-user"></a><span data-ttu-id="16e58-103">Создание пользователя</span><span class="sxs-lookup"><span data-stu-id="16e58-103">Create user</span></span>

<span data-ttu-id="16e58-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16e58-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16e58-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16e58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16e58-106">Создание объекта [user](../resources/intune-mam-user.md).</span><span class="sxs-lookup"><span data-stu-id="16e58-106">Create a new [user](../resources/intune-mam-user.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16e58-107">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="16e58-107">Prerequisites</span></span>
<span data-ttu-id="16e58-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="16e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16e58-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="16e58-110">Permission type</span></span>|<span data-ttu-id="16e58-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="16e58-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16e58-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="16e58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16e58-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e58-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="16e58-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="16e58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16e58-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="16e58-115">Not supported.</span></span>|
|<span data-ttu-id="16e58-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="16e58-116">Application</span></span>|<span data-ttu-id="16e58-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e58-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="16e58-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="16e58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users
```

## <a name="request-headers"></a><span data-ttu-id="16e58-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="16e58-119">Request headers</span></span>
|<span data-ttu-id="16e58-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="16e58-120">Header</span></span>|<span data-ttu-id="16e58-121">Значение</span><span class="sxs-lookup"><span data-stu-id="16e58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16e58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16e58-122">Authorization</span></span>|<span data-ttu-id="16e58-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="16e58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16e58-124">Accept</span><span class="sxs-lookup"><span data-stu-id="16e58-124">Accept</span></span>|<span data-ttu-id="16e58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16e58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16e58-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="16e58-126">Request body</span></span>
<span data-ttu-id="16e58-127">В теле запроса добавьте представление объекта user в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16e58-127">In the request body, supply a JSON representation for the user object.</span></span>

<span data-ttu-id="16e58-128">В приведенной ниже таблице указаны свойства, необходимые при создании объекта user.</span><span class="sxs-lookup"><span data-stu-id="16e58-128">The following table shows the properties that are required when you create the user.</span></span>

|<span data-ttu-id="16e58-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="16e58-129">Property</span></span>|<span data-ttu-id="16e58-130">Тип</span><span class="sxs-lookup"><span data-stu-id="16e58-130">Type</span></span>|<span data-ttu-id="16e58-131">Описание</span><span class="sxs-lookup"><span data-stu-id="16e58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e58-132">id</span><span class="sxs-lookup"><span data-stu-id="16e58-132">id</span></span>|<span data-ttu-id="16e58-133">String</span><span class="sxs-lookup"><span data-stu-id="16e58-133">String</span></span>|<span data-ttu-id="16e58-134">Идентификатор пользователя.</span><span class="sxs-lookup"><span data-stu-id="16e58-134">The user identifier.</span></span>|



## <a name="response"></a><span data-ttu-id="16e58-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="16e58-135">Response</span></span>
<span data-ttu-id="16e58-136">При успешном выполнении этот метод возвращает код отклика `201 Created` и объект [user](../resources/intune-mam-user.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="16e58-136">If successful, this method returns a `201 Created` response code and a [user](../resources/intune-mam-user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e58-137">Пример</span><span class="sxs-lookup"><span data-stu-id="16e58-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="16e58-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="16e58-138">Request</span></span>
<span data-ttu-id="16e58-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="16e58-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json
Content-length: 46

{
  "@odata.type": "#microsoft.graph.user"
}
```

### <a name="response"></a><span data-ttu-id="16e58-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="16e58-140">Response</span></span>
<span data-ttu-id="16e58-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="16e58-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```




