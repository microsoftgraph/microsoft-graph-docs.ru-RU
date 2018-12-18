---
title: Delete deviceConfigurationUserStatus
description: Удаляет объект deviceConfigurationUserStatus.
author: tfitzmac
ms.openlocfilehash: d248f1440053aeac9a53a534b22af61cfc396c03
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355080"
---
# <a name="delete-deviceconfigurationuserstatus"></a><span data-ttu-id="a9903-103">Delete deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="a9903-103">Delete deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="a9903-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a9903-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9903-105">Удаляет объект [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="a9903-105">Deletes a [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9903-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="a9903-106">Prerequisites</span></span>
<span data-ttu-id="a9903-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a9903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9903-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a9903-109">Permission type</span></span>|<span data-ttu-id="a9903-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a9903-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9903-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a9903-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9903-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9903-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9903-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a9903-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9903-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9903-114">Not supported.</span></span>|
|<span data-ttu-id="a9903-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a9903-115">Application</span></span>|<span data-ttu-id="a9903-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a9903-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9903-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a9903-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="a9903-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a9903-118">Request headers</span></span>
|<span data-ttu-id="a9903-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a9903-119">Header</span></span>|<span data-ttu-id="a9903-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a9903-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9903-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a9903-121">Authorization</span></span>|<span data-ttu-id="a9903-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a9903-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9903-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a9903-123">Accept</span></span>|<span data-ttu-id="a9903-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9903-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9903-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a9903-125">Request body</span></span>
<span data-ttu-id="a9903-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a9903-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9903-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9903-127">Response</span></span>
<span data-ttu-id="a9903-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a9903-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a9903-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a9903-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9903-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a9903-130">Request</span></span>
<span data-ttu-id="a9903-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a9903-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="a9903-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="a9903-132">Response</span></span>
<span data-ttu-id="a9903-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a9903-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



