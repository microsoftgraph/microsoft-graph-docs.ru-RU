---
title: Удаление пользователя
description: Удаляет объект user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f516c1386d828412e71fa35668b4c86a496f6af
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028807"
---
# <a name="delete-user"></a><span data-ttu-id="d5a28-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="d5a28-103">Delete user</span></span>

<span data-ttu-id="d5a28-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5a28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5a28-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d5a28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5a28-106">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="d5a28-106">Deletes a [user](../resources/intune-shared-user.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5a28-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="d5a28-107">Prerequisites</span></span>
<span data-ttu-id="d5a28-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="d5a28-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d5a28-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5a28-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="d5a28-110">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="d5a28-110">The specific permission required depends on context.</span></span>

|<span data-ttu-id="d5a28-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d5a28-111">Permission type</span></span>|<span data-ttu-id="d5a28-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d5a28-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5a28-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d5a28-113">Delegated (work or school account)</span></span>| <span data-ttu-id="d5a28-114">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="d5a28-114">_varies by context_</span></span>|
| <span data-ttu-id="d5a28-115">&nbsp;&nbsp;Devices (устройства)</span><span class="sxs-lookup"><span data-stu-id="d5a28-115">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="d5a28-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a28-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="d5a28-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="d5a28-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="d5a28-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a28-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="d5a28-119">&nbsp;Входящая миграция &nbsp;</span><span class="sxs-lookup"><span data-stu-id="d5a28-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="d5a28-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a28-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="d5a28-121">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="d5a28-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="d5a28-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d5a28-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="d5a28-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d5a28-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5a28-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a28-124">Not supported.</span></span>|
|<span data-ttu-id="d5a28-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d5a28-125">Application</span></span>|<span data-ttu-id="d5a28-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d5a28-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5a28-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d5a28-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="d5a28-128">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d5a28-128">Request headers</span></span>
|<span data-ttu-id="d5a28-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d5a28-129">Header</span></span>|<span data-ttu-id="d5a28-130">Значение</span><span class="sxs-lookup"><span data-stu-id="d5a28-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5a28-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5a28-131">Authorization</span></span>|<span data-ttu-id="d5a28-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d5a28-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5a28-133">Accept</span><span class="sxs-lookup"><span data-stu-id="d5a28-133">Accept</span></span>|<span data-ttu-id="d5a28-134">application/json</span><span class="sxs-lookup"><span data-stu-id="d5a28-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5a28-135">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d5a28-135">Request body</span></span>
<span data-ttu-id="d5a28-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d5a28-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5a28-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a28-137">Response</span></span>
<span data-ttu-id="d5a28-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d5a28-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d5a28-139">Пример</span><span class="sxs-lookup"><span data-stu-id="d5a28-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5a28-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="d5a28-140">Request</span></span>
<span data-ttu-id="d5a28-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d5a28-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="d5a28-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d5a28-142">Response</span></span>
<span data-ttu-id="d5a28-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d5a28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









