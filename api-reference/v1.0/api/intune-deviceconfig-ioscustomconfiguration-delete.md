---
title: Delete iosCustomConfiguration
description: Удаляет объект iosCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 45b7193deb7fd52ddeeeb78274b41be7f9dc0160
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332125"
---
# <a name="delete-ioscustomconfiguration"></a><span data-ttu-id="6f6ad-103">Delete iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="6f6ad-103">Delete iosCustomConfiguration</span></span>

> <span data-ttu-id="6f6ad-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f6ad-105">Удаляет объект [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="6f6ad-105">Deletes a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f6ad-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6ad-106">Prerequisites</span></span>
<span data-ttu-id="6f6ad-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f6ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6ad-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6f6ad-109">Permission type</span></span>|<span data-ttu-id="6f6ad-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6f6ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f6ad-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6f6ad-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6f6ad-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6ad-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6f6ad-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6f6ad-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f6ad-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-114">Not supported.</span></span>|
|<span data-ttu-id="6f6ad-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6f6ad-115">Application</span></span>|<span data-ttu-id="6f6ad-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f6ad-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6f6ad-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6f6ad-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6f6ad-118">Request headers</span></span>
|<span data-ttu-id="6f6ad-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6f6ad-119">Header</span></span>|<span data-ttu-id="6f6ad-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6f6ad-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f6ad-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6f6ad-121">Authorization</span></span>|<span data-ttu-id="6f6ad-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6f6ad-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f6ad-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6f6ad-123">Accept</span></span>|<span data-ttu-id="6f6ad-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6f6ad-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6ad-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6f6ad-125">Request body</span></span>
<span data-ttu-id="6f6ad-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f6ad-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f6ad-127">Response</span></span>
<span data-ttu-id="6f6ad-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6f6ad-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6f6ad-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f6ad-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6f6ad-130">Request</span></span>
<span data-ttu-id="6f6ad-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6f6ad-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="6f6ad-132">Response</span></span>
<span data-ttu-id="6f6ad-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="6f6ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



