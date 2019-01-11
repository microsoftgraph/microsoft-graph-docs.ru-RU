---
title: Удаление пользователя
description: Удаляет объект user.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cc1979284cada76f76a98acc8956271b7224aa53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837837"
---
# <a name="delete-user"></a><span data-ttu-id="427d1-103">Удаление пользователя</span><span class="sxs-lookup"><span data-stu-id="427d1-103">Delete user</span></span>

> <span data-ttu-id="427d1-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="427d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="427d1-105">Удаляет объект [user](../resources/intune-shared-user.md).</span><span class="sxs-lookup"><span data-stu-id="427d1-105">Deletes a [user](../resources/intune-shared-user.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="427d1-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="427d1-106">Prerequisites</span></span>
<span data-ttu-id="427d1-107">Чтобы вызвать этот интерфейс API необходимо одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="427d1-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="427d1-108">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="427d1-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>  <span data-ttu-id="427d1-109">Необходимые разрешения определенного зависит от контекста.</span><span class="sxs-lookup"><span data-stu-id="427d1-109">The specific permission required depends on context.</span></span>

|<span data-ttu-id="427d1-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="427d1-110">Permission type</span></span>|<span data-ttu-id="427d1-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="427d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="427d1-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="427d1-112">Delegated (work or school account)</span></span>| <span data-ttu-id="427d1-113">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="427d1-113">_varies by context_</span></span>|
| <span data-ttu-id="427d1-114">&nbsp;&nbsp; Устройств</span><span class="sxs-lookup"><span data-stu-id="427d1-114">&nbsp; &nbsp; Devices</span></span> | <span data-ttu-id="427d1-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427d1-115">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="427d1-116">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="427d1-116">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="427d1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427d1-117">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="427d1-118">&nbsp;&nbsp; Адаптация новых сотрудников</span><span class="sxs-lookup"><span data-stu-id="427d1-118">&nbsp; &nbsp; Onboarding</span></span> | <span data-ttu-id="427d1-119">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427d1-119">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="427d1-120">&nbsp;&nbsp; Устранение неполадок</span><span class="sxs-lookup"><span data-stu-id="427d1-120">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="427d1-121">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="427d1-121">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
|<span data-ttu-id="427d1-122">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="427d1-122">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="427d1-123">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="427d1-123">Not supported.</span></span>|
|<span data-ttu-id="427d1-124">Для приложений</span><span class="sxs-lookup"><span data-stu-id="427d1-124">Application</span></span>|<span data-ttu-id="427d1-125">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="427d1-125">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="427d1-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="427d1-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="427d1-127">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="427d1-127">Request headers</span></span>
|<span data-ttu-id="427d1-128">Заголовок</span><span class="sxs-lookup"><span data-stu-id="427d1-128">Header</span></span>|<span data-ttu-id="427d1-129">Значение</span><span class="sxs-lookup"><span data-stu-id="427d1-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="427d1-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="427d1-130">Authorization</span></span>|<span data-ttu-id="427d1-131">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="427d1-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="427d1-132">Accept</span><span class="sxs-lookup"><span data-stu-id="427d1-132">Accept</span></span>|<span data-ttu-id="427d1-133">application/json</span><span class="sxs-lookup"><span data-stu-id="427d1-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="427d1-134">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="427d1-134">Request body</span></span>
<span data-ttu-id="427d1-135">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="427d1-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="427d1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="427d1-136">Response</span></span>
<span data-ttu-id="427d1-137">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="427d1-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="427d1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="427d1-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="427d1-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="427d1-139">Request</span></span>
<span data-ttu-id="427d1-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="427d1-140">Here is an example of the request.</span></span>

``` http
DELETE https://graph.microsoft.com/v1.0/users/{usersId}
```

### <a name="response"></a><span data-ttu-id="427d1-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="427d1-141">Response</span></span>
<span data-ttu-id="427d1-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="427d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 204 No Content
```



