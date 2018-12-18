---
title: Удаление объекта sharedPCConfiguration
description: Удаляет объект sharedPCConfiguration.
author: tfitzmac
ms.openlocfilehash: aca06e7a2d0d3ce6aaa28a7b86274c8c4f44acc3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304398"
---
# <a name="delete-sharedpcconfiguration"></a><span data-ttu-id="edadd-103">Удаление объекта sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="edadd-103">Delete sharedPCConfiguration</span></span>

> <span data-ttu-id="edadd-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="edadd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="edadd-105">Удаляет объект [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="edadd-105">Deletes a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="edadd-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="edadd-106">Prerequisites</span></span>
<span data-ttu-id="edadd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edadd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="edadd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="edadd-109">Permission type</span></span>|<span data-ttu-id="edadd-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="edadd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="edadd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="edadd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="edadd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edadd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="edadd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="edadd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="edadd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edadd-114">Not supported.</span></span>|
|<span data-ttu-id="edadd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="edadd-115">Application</span></span>|<span data-ttu-id="edadd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="edadd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="edadd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="edadd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="edadd-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="edadd-118">Request headers</span></span>
|<span data-ttu-id="edadd-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="edadd-119">Header</span></span>|<span data-ttu-id="edadd-120">Значение</span><span class="sxs-lookup"><span data-stu-id="edadd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="edadd-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="edadd-121">Authorization</span></span>|<span data-ttu-id="edadd-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="edadd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="edadd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="edadd-123">Accept</span></span>|<span data-ttu-id="edadd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="edadd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="edadd-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="edadd-125">Request body</span></span>
<span data-ttu-id="edadd-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="edadd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="edadd-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="edadd-127">Response</span></span>
<span data-ttu-id="edadd-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="edadd-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="edadd-129">Пример</span><span class="sxs-lookup"><span data-stu-id="edadd-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="edadd-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="edadd-130">Request</span></span>
<span data-ttu-id="edadd-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="edadd-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="edadd-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="edadd-132">Response</span></span>
<span data-ttu-id="edadd-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="edadd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



