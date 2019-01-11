---
title: Удаление объекта deviceManagementPartner
description: Удаляет объект deviceManagementPartner.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c3fec8ec5625fcf32557bdd8cb4a6bf0bce3f4c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844011"
---
# <a name="delete-devicemanagementpartner"></a><span data-ttu-id="fc867-103">Удаление объекта deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="fc867-103">Delete deviceManagementPartner</span></span>

> <span data-ttu-id="fc867-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fc867-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc867-105">Удаляет объект [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span><span class="sxs-lookup"><span data-stu-id="fc867-105">Deletes a [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc867-106">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="fc867-106">Prerequisites</span></span>
<span data-ttu-id="fc867-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc867-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc867-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc867-109">Permission type</span></span>|<span data-ttu-id="fc867-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc867-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc867-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc867-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc867-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc867-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fc867-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc867-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc867-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc867-114">Not supported.</span></span>|
|<span data-ttu-id="fc867-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc867-115">Application</span></span>|<span data-ttu-id="fc867-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc867-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc867-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc867-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="fc867-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc867-118">Request headers</span></span>
|<span data-ttu-id="fc867-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fc867-119">Header</span></span>|<span data-ttu-id="fc867-120">Значение</span><span class="sxs-lookup"><span data-stu-id="fc867-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc867-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc867-121">Authorization</span></span>|<span data-ttu-id="fc867-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="fc867-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc867-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fc867-123">Accept</span></span>|<span data-ttu-id="fc867-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fc867-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc867-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc867-125">Request body</span></span>
<span data-ttu-id="fc867-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fc867-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc867-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc867-127">Response</span></span>
<span data-ttu-id="fc867-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="fc867-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fc867-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fc867-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc867-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc867-130">Request</span></span>
<span data-ttu-id="fc867-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc867-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="fc867-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="fc867-132">Response</span></span>
<span data-ttu-id="fc867-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="fc867-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



