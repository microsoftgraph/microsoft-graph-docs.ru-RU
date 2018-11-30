---
title: Перечисление объектов termsAndConditionsAcceptanceStatus
description: Список свойств и связей объектов termsAndConditionsAcceptanceStatus.
ms.openlocfilehash: 0f519f399b1c13f227b0375270d45ca229c4081e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077858"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="ce2f4-103">Перечисление объектов termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="ce2f4-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="ce2f4-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ce2f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce2f4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce2f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce2f4-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ce2f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce2f4-107">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="ce2f4-107">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce2f4-108">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="ce2f4-108">Prerequisites</span></span>
<span data-ttu-id="ce2f4-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce2f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce2f4-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce2f4-111">Permission type</span></span>|<span data-ttu-id="ce2f4-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce2f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce2f4-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce2f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ce2f4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce2f4-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ce2f4-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce2f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce2f4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce2f4-116">Not supported.</span></span>|
|<span data-ttu-id="ce2f4-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce2f4-117">Application</span></span>|<span data-ttu-id="ce2f4-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce2f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce2f4-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce2f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ce2f4-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce2f4-120">Request headers</span></span>
|<span data-ttu-id="ce2f4-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ce2f4-121">Header</span></span>|<span data-ttu-id="ce2f4-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ce2f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce2f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce2f4-123">Authorization</span></span>|<span data-ttu-id="ce2f4-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="ce2f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce2f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ce2f4-125">Accept</span></span>|<span data-ttu-id="ce2f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ce2f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce2f4-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce2f4-127">Request body</span></span>
<span data-ttu-id="ce2f4-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce2f4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce2f4-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce2f4-129">Response</span></span>
<span data-ttu-id="ce2f4-130">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ce2f4-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce2f4-131">Пример</span><span class="sxs-lookup"><span data-stu-id="ce2f4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce2f4-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce2f4-132">Request</span></span>
<span data-ttu-id="ce2f4-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce2f4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="ce2f4-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ce2f4-134">Response</span></span>
<span data-ttu-id="ce2f4-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ce2f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
      "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
      "userDisplayName": "User Display Name value",
      "acceptedVersion": 15,
      "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
    }
  ]
}
```





