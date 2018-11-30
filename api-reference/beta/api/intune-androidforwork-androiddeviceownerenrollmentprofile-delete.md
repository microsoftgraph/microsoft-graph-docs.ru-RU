---
title: Удаление androidDeviceOwnerEnrollmentProfile
description: Удаляет androidDeviceOwnerEnrollmentProfile.
ms.openlocfilehash: 0b434a97e65c38399f04a069167f2cd2840943b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075610"
---
# <a name="delete-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="6b287-103">Удаление androidDeviceOwnerEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b287-103">Delete androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="6b287-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6b287-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b287-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b287-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b287-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6b287-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b287-107">Удаляет [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6b287-107">Deletes a [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b287-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="6b287-108">Prerequisites</span></span>
<span data-ttu-id="6b287-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b287-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b287-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b287-111">Permission type</span></span>|<span data-ttu-id="6b287-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b287-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b287-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b287-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b287-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b287-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b287-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b287-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b287-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b287-116">Not supported.</span></span>|
|<span data-ttu-id="6b287-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b287-117">Application</span></span>|<span data-ttu-id="6b287-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b287-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b287-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b287-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="6b287-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b287-120">Request headers</span></span>
|<span data-ttu-id="6b287-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6b287-121">Header</span></span>|<span data-ttu-id="6b287-122">Значение</span><span class="sxs-lookup"><span data-stu-id="6b287-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b287-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b287-123">Authorization</span></span>|<span data-ttu-id="6b287-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="6b287-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b287-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6b287-125">Accept</span></span>|<span data-ttu-id="6b287-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b287-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b287-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b287-127">Request body</span></span>
<span data-ttu-id="6b287-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6b287-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b287-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b287-129">Response</span></span>
<span data-ttu-id="6b287-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6b287-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6b287-131">Пример</span><span class="sxs-lookup"><span data-stu-id="6b287-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b287-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b287-132">Request</span></span>
<span data-ttu-id="6b287-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b287-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="6b287-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="6b287-134">Response</span></span>
<span data-ttu-id="6b287-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="6b287-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





