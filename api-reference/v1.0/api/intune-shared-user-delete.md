---
title: Удаление пользователя
description: Удаляет объект user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e66d987c2e88f40dd5b104961e9203dcd636651a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576813"
---
# <a name="delete-user"></a><span data-ttu-id="189ae-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="189ae-103">Delete user</span></span>

> <span data-ttu-id="189ae-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="189ae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="189ae-105">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="189ae-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="189ae-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="189ae-106">Prerequisites</span></span>
<span data-ttu-id="189ae-107">Для вызова этого API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="189ae-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="189ae-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="189ae-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="189ae-109">Необходимое разрешение зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="189ae-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="189ae-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="189ae-110">Permission type</span></span>|<span data-ttu-id="189ae-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="189ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="189ae-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="189ae-112">Delegated (work or school account)</span></span>| <span data-ttu-id="189ae-113">_зависит от контекста_</span><span class="sxs-lookup"><span data-stu-id="189ae-113">_varies by context_</span></span>|
| <span data-ttu-id="189ae-114">&nbsp;&nbsp; Devices (устройства)</span><span class="sxs-lookup"><span data-stu-id="189ae-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="189ae-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189ae-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="189ae-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="189ae-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="189ae-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189ae-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="189ae-118">&nbsp;&nbsp; Входящая миграция</span><span class="sxs-lookup"><span data-stu-id="189ae-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="189ae-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189ae-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="189ae-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="189ae-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="189ae-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="189ae-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="189ae-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="189ae-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="189ae-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="189ae-123">Not supported.</span></span>|
|<span data-ttu-id="189ae-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="189ae-124">Application</span></span>|<span data-ttu-id="189ae-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="189ae-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="189ae-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="189ae-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="189ae-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="189ae-127">Request headers</span></span>
|<span data-ttu-id="189ae-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="189ae-128">Header</span></span>|<span data-ttu-id="189ae-129">Значение</span><span class="sxs-lookup"><span data-stu-id="189ae-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="189ae-130">Авторизация</span><span class="sxs-lookup"><span data-stu-id="189ae-130">Authorization</span></span>|<span data-ttu-id="189ae-131">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="189ae-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="189ae-132">Accept</span><span class="sxs-lookup"><span data-stu-id="189ae-132">Accept</span></span>|<span data-ttu-id="189ae-133">application/json</span><span class="sxs-lookup"><span data-stu-id="189ae-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="189ae-134">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="189ae-134">Request body</span></span>
<span data-ttu-id="189ae-135">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="189ae-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="189ae-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="189ae-136">Response</span></span>
<span data-ttu-id="189ae-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="189ae-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="189ae-138">Пример</span><span class="sxs-lookup"><span data-stu-id="189ae-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="189ae-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="189ae-139">Request</span></span>
<span data-ttu-id="189ae-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="189ae-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="189ae-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="189ae-141">Response</span></span>
<span data-ttu-id="189ae-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="189ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



