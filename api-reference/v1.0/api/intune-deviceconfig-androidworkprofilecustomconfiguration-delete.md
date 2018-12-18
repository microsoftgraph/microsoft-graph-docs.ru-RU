---
title: Удаление androidWorkProfileCustomConfiguration
description: Удаляет androidWorkProfileCustomConfiguration.
author: tfitzmac
ms.openlocfilehash: 91df3e95903621b603c30fc403f37e9e8c7b8ff3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303705"
---
# <a name="delete-androidworkprofilecustomconfiguration"></a><span data-ttu-id="7ef31-103">Удаление androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="7ef31-103">Delete androidWorkProfileCustomConfiguration</span></span>

> <span data-ttu-id="7ef31-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="7ef31-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7ef31-105">Удаляет [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7ef31-105">Deletes a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7ef31-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="7ef31-106">Prerequisites</span></span>
<span data-ttu-id="7ef31-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ef31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ef31-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ef31-109">Permission type</span></span>|<span data-ttu-id="7ef31-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ef31-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ef31-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ef31-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ef31-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ef31-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ef31-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ef31-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ef31-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef31-114">Not supported.</span></span>|
|<span data-ttu-id="7ef31-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ef31-115">Application</span></span>|<span data-ttu-id="7ef31-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ef31-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ef31-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ef31-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7ef31-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ef31-118">Request headers</span></span>
|<span data-ttu-id="7ef31-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ef31-119">Header</span></span>|<span data-ttu-id="7ef31-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7ef31-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ef31-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ef31-121">Authorization</span></span>|<span data-ttu-id="7ef31-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="7ef31-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ef31-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7ef31-123">Accept</span></span>|<span data-ttu-id="7ef31-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ef31-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ef31-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7ef31-125">Request body</span></span>
<span data-ttu-id="7ef31-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ef31-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ef31-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ef31-127">Response</span></span>
<span data-ttu-id="7ef31-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7ef31-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7ef31-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7ef31-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7ef31-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ef31-130">Request</span></span>
<span data-ttu-id="7ef31-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ef31-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="7ef31-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ef31-132">Response</span></span>
<span data-ttu-id="7ef31-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="7ef31-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



