---
title: Удаление пользователя
description: Удаляет объект user.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3bb78ef11b67ba2a4d0c5f8ab9b15c65ad2ec26f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961528"
---
# <a name="delete-user"></a><span data-ttu-id="f4a01-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="f4a01-103">Delete user</span></span>

> <span data-ttu-id="f4a01-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f4a01-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4a01-105">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="f4a01-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4a01-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="f4a01-106">Prerequisites</span></span>
<span data-ttu-id="f4a01-107">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="f4a01-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f4a01-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4a01-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="f4a01-109">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="f4a01-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="f4a01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4a01-110">Permission type</span></span>|<span data-ttu-id="f4a01-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4a01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4a01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4a01-112">Delegated (work or school account)</span></span>| <span data-ttu-id="f4a01-113">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="f4a01-113">_varies by context_</span></span>|
| <span data-ttu-id="f4a01-114">&nbsp;&nbsp; Устройств</span><span class="sxs-lookup"><span data-stu-id="f4a01-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="f4a01-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a01-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="f4a01-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="f4a01-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="f4a01-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a01-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="f4a01-118">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="f4a01-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="f4a01-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a01-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="f4a01-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="f4a01-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="f4a01-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4a01-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="f4a01-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4a01-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4a01-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4a01-123">Not supported.</span></span>|
|<span data-ttu-id="f4a01-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4a01-124">Application</span></span>|<span data-ttu-id="f4a01-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4a01-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4a01-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4a01-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="f4a01-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4a01-127">Request headers</span></span>
|<span data-ttu-id="f4a01-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f4a01-128">Header</span></span>|<span data-ttu-id="f4a01-129">Значение</span><span class="sxs-lookup"><span data-stu-id="f4a01-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4a01-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4a01-130">Authorization</span></span>|<span data-ttu-id="f4a01-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f4a01-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4a01-132">Accept</span><span class="sxs-lookup"><span data-stu-id="f4a01-132">Accept</span></span>|<span data-ttu-id="f4a01-133">application/json</span><span class="sxs-lookup"><span data-stu-id="f4a01-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4a01-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f4a01-134">Request body</span></span>
<span data-ttu-id="f4a01-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f4a01-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4a01-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4a01-136">Response</span></span>
<span data-ttu-id="f4a01-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f4a01-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f4a01-138">Пример</span><span class="sxs-lookup"><span data-stu-id="f4a01-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4a01-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4a01-139">Request</span></span>
<span data-ttu-id="f4a01-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4a01-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="f4a01-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="f4a01-141">Response</span></span>
<span data-ttu-id="f4a01-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f4a01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



