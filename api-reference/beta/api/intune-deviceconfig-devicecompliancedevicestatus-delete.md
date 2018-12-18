---
title: Удаление объекта deviceComplianceDeviceStatus
description: Удаляет объект deviceComplianceDeviceStatus.
author: tfitzmac
ms.openlocfilehash: 94f596050852334bd6a7ab35b85ea2954f55e268
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318573"
---
# <a name="delete-devicecompliancedevicestatus"></a><span data-ttu-id="68cfb-103">Удаление объекта deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="68cfb-103">Delete deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="68cfb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="68cfb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68cfb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68cfb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68cfb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="68cfb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68cfb-107">Удаляет объект [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span><span class="sxs-lookup"><span data-stu-id="68cfb-107">Deletes a [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="68cfb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="68cfb-108">Prerequisites</span></span>
<span data-ttu-id="68cfb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68cfb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68cfb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="68cfb-111">Permission type</span></span>|<span data-ttu-id="68cfb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="68cfb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68cfb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="68cfb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="68cfb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cfb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="68cfb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="68cfb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68cfb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68cfb-116">Not supported.</span></span>|
|<span data-ttu-id="68cfb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="68cfb-117">Application</span></span>|<span data-ttu-id="68cfb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="68cfb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68cfb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="68cfb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="68cfb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="68cfb-120">Request headers</span></span>
|<span data-ttu-id="68cfb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="68cfb-121">Header</span></span>|<span data-ttu-id="68cfb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="68cfb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68cfb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="68cfb-123">Authorization</span></span>|<span data-ttu-id="68cfb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="68cfb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68cfb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="68cfb-125">Accept</span></span>|<span data-ttu-id="68cfb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="68cfb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68cfb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="68cfb-127">Request body</span></span>
<span data-ttu-id="68cfb-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="68cfb-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68cfb-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="68cfb-129">Response</span></span>
<span data-ttu-id="68cfb-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="68cfb-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="68cfb-131">Пример</span><span class="sxs-lookup"><span data-stu-id="68cfb-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="68cfb-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="68cfb-132">Request</span></span>
<span data-ttu-id="68cfb-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="68cfb-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="68cfb-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="68cfb-134">Response</span></span>
<span data-ttu-id="68cfb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="68cfb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





