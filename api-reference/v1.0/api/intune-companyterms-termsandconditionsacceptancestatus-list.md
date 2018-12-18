---
title: Перечисление объектов termsAndConditionsAcceptanceStatus
description: Список свойств и связей объектов termsAndConditionsAcceptanceStatus.
author: tfitzmac
ms.openlocfilehash: c32cbde73a27ce88fdb6049cf2e3aacf869b1bdd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321114"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="9c4ab-103">Перечисление объектов termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="9c4ab-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="9c4ab-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9c4ab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c4ab-105">Список свойств и связей объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="9c4ab-105">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c4ab-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="9c4ab-106">Prerequisites</span></span>
<span data-ttu-id="9c4ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c4ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c4ab-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c4ab-109">Permission type</span></span>|<span data-ttu-id="9c4ab-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c4ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c4ab-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c4ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9c4ab-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c4ab-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="9c4ab-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c4ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c4ab-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c4ab-114">Not supported.</span></span>|
|<span data-ttu-id="9c4ab-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c4ab-115">Application</span></span>|<span data-ttu-id="9c4ab-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c4ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c4ab-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c4ab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="9c4ab-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c4ab-118">Request headers</span></span>
|<span data-ttu-id="9c4ab-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9c4ab-119">Header</span></span>|<span data-ttu-id="9c4ab-120">Значение</span><span class="sxs-lookup"><span data-stu-id="9c4ab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c4ab-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c4ab-121">Authorization</span></span>|<span data-ttu-id="9c4ab-122">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="9c4ab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c4ab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9c4ab-123">Accept</span></span>|<span data-ttu-id="9c4ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9c4ab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c4ab-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c4ab-125">Request body</span></span>
<span data-ttu-id="9c4ab-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c4ab-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c4ab-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c4ab-127">Response</span></span>
<span data-ttu-id="9c4ab-128">В случае успешного выполнения этот метод возвращает код отклика `200 OK` и коллекцию объектов [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9c4ab-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c4ab-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9c4ab-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c4ab-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c4ab-130">Request</span></span>
<span data-ttu-id="9c4ab-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c4ab-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="9c4ab-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c4ab-132">Response</span></span>
<span data-ttu-id="9c4ab-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="9c4ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



