---
title: Удаление пользователя
description: Удаляет объект user.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1f516c1386d828412e71fa35668b4c86a496f6af
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732802"
---
# <a name="delete-user"></a><span data-ttu-id="51162-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="51162-103">Delete user</span></span>

<span data-ttu-id="51162-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51162-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51162-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51162-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51162-106">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="51162-106">Deletes a [user](../resources/intune-shared-user.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51162-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="51162-107">Prerequisites</span></span>
<span data-ttu-id="51162-108">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="51162-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="51162-109">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51162-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="51162-110">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="51162-110">The specific permission required depends on context.</span></span>

|<span data-ttu-id="51162-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="51162-111">Permission type</span></span>|<span data-ttu-id="51162-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="51162-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51162-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="51162-113">Delegated (work or school account)</span></span>| <span data-ttu-id="51162-114">_изменяется в зависимости от контекста_</span><span class="sxs-lookup"><span data-stu-id="51162-114">_varies by context_</span></span>|
| <span data-ttu-id="51162-115">&nbsp;&nbsp;Устройства</span><span class="sxs-lookup"><span data-stu-id="51162-115">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="51162-116">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51162-116">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="51162-117">&nbsp;&nbsp;MAM</span><span class="sxs-lookup"><span data-stu-id="51162-117">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="51162-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51162-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="51162-119">&nbsp;&nbsp;Onboarding</span><span class="sxs-lookup"><span data-stu-id="51162-119">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="51162-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51162-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="51162-121">&nbsp;&nbsp;Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="51162-121">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="51162-122">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51162-122">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="51162-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="51162-123">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51162-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51162-124">Not supported.</span></span>|
|<span data-ttu-id="51162-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="51162-125">Application</span></span>|<span data-ttu-id="51162-126">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="51162-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51162-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="51162-127">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="51162-128">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="51162-128">Request headers</span></span>
|<span data-ttu-id="51162-129">Заголовок</span><span class="sxs-lookup"><span data-stu-id="51162-129">Header</span></span>|<span data-ttu-id="51162-130">Значение</span><span class="sxs-lookup"><span data-stu-id="51162-130">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51162-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="51162-131">Authorization</span></span>|<span data-ttu-id="51162-132">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="51162-132">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51162-133">Accept</span><span class="sxs-lookup"><span data-stu-id="51162-133">Accept</span></span>|<span data-ttu-id="51162-134">application/json</span><span class="sxs-lookup"><span data-stu-id="51162-134">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51162-135">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="51162-135">Request body</span></span>
<span data-ttu-id="51162-136">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="51162-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51162-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="51162-137">Response</span></span>
<span data-ttu-id="51162-138">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="51162-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="51162-139">Пример</span><span class="sxs-lookup"><span data-stu-id="51162-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="51162-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="51162-140">Request</span></span>
<span data-ttu-id="51162-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="51162-141">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="51162-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="51162-142">Response</span></span>
<span data-ttu-id="51162-p102">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="51162-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```









