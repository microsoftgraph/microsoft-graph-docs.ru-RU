---
title: Функция getManagedAppDiagnosticStatuses
description: Получает состояние диагностической проверки для определенного пользователя.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: af90cc194dc1e9c1a954a090c748ef679248d9d3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888587"
---
# <a name="getmanagedappdiagnosticstatuses-function"></a><span data-ttu-id="28d21-103">Функция getManagedAppDiagnosticStatuses</span><span class="sxs-lookup"><span data-stu-id="28d21-103">getManagedAppDiagnosticStatuses function</span></span>

> <span data-ttu-id="28d21-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="28d21-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28d21-105">Получает состояние диагностической проверки для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="28d21-105">Gets diagnostics validation status for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28d21-106">Предварительные условия</span><span class="sxs-lookup"><span data-stu-id="28d21-106">Prerequisites</span></span>
<span data-ttu-id="28d21-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28d21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28d21-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="28d21-109">Permission type</span></span>|<span data-ttu-id="28d21-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="28d21-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28d21-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="28d21-111">Delegated (work or school account)</span></span>| <span data-ttu-id="28d21-112">_изменяется в соответствии с контекста_</span><span class="sxs-lookup"><span data-stu-id="28d21-112">_varies by context_</span></span>|
| <span data-ttu-id="28d21-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="28d21-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="28d21-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="28d21-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="28d21-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="28d21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28d21-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d21-116">Not supported.</span></span>|
|<span data-ttu-id="28d21-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="28d21-117">Application</span></span>|<span data-ttu-id="28d21-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="28d21-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28d21-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="28d21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppDiagnosticStatuses
```

## <a name="request-headers"></a><span data-ttu-id="28d21-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="28d21-120">Request headers</span></span>
|<span data-ttu-id="28d21-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="28d21-121">Header</span></span>|<span data-ttu-id="28d21-122">Значение</span><span class="sxs-lookup"><span data-stu-id="28d21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28d21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28d21-123">Authorization</span></span>|<span data-ttu-id="28d21-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="28d21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28d21-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28d21-125">Accept</span></span>|<span data-ttu-id="28d21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28d21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28d21-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="28d21-127">Request body</span></span>
<span data-ttu-id="28d21-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="28d21-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28d21-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="28d21-129">Response</span></span>
<span data-ttu-id="28d21-130">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="28d21-130">If successful, this function returns a `200 OK` response code and a [managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28d21-131">Пример</span><span class="sxs-lookup"><span data-stu-id="28d21-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="28d21-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="28d21-132">Request</span></span>
<span data-ttu-id="28d21-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="28d21-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppDiagnosticStatuses
```

### <a name="response"></a><span data-ttu-id="28d21-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="28d21-134">Response</span></span>
<span data-ttu-id="28d21-p102">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="28d21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": [
    {
      "@odata.type": "microsoft.graph.managedAppDiagnosticStatus",
      "validationName": "Validation Name value",
      "state": "State value",
      "mitigationInstruction": "Mitigation Instruction value"
    }
  ]
}
```



