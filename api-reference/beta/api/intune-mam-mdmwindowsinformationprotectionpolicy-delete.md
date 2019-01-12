---
title: Удаление объекта mdmWindowsInformationProtectionPolicy
description: Удаление объекта mdmWindowsInformationProtectionPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 22b5eb1392a31ed7d02be87d4fccc92e8e4280af
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974686"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="a4087-103">Удаление объекта mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a4087-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="a4087-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a4087-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a4087-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4087-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4087-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a4087-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a4087-107">Удаляет объект [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="a4087-107">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-mam-mdmwindowsinformationprotectionpolicy.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a4087-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a4087-108">Prerequisites</span></span>
<span data-ttu-id="a4087-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4087-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4087-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4087-111">Permission type</span></span>|<span data-ttu-id="a4087-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4087-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4087-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4087-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4087-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4087-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a4087-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4087-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4087-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4087-116">Not supported.</span></span>|
|<span data-ttu-id="a4087-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4087-117">Application</span></span>|<span data-ttu-id="a4087-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4087-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4087-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4087-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="a4087-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4087-120">Request headers</span></span>
|<span data-ttu-id="a4087-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a4087-121">Header</span></span>|<span data-ttu-id="a4087-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a4087-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4087-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4087-123">Authorization</span></span>|<span data-ttu-id="a4087-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a4087-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4087-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4087-125">Accept</span></span>|<span data-ttu-id="a4087-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4087-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4087-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4087-127">Request body</span></span>
<span data-ttu-id="a4087-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4087-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4087-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4087-129">Response</span></span>
<span data-ttu-id="a4087-130">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a4087-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a4087-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a4087-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a4087-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4087-132">Request</span></span>
<span data-ttu-id="a4087-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4087-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="a4087-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4087-134">Response</span></span>
<span data-ttu-id="a4087-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a4087-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





